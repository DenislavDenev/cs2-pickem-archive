# Methodology

## Goal

Predict the 10-slot CS2 Major Swiss stage pick'em: 2 teams to go 3-0, 6 to advance, 2 to go 0-3.

---

## Model Version

Current: `bo1_edge_v7` (June 2026)

- **v7** (2026-06-10): per-map results scraped from stage-page match popups
  (new data layer, backfilled across all 5 covered Majors) and a map-pool
  depth adjustment (see below). The same study documented two nulls:
  optimal-assignment pick sheets (greedy is ~99.8% optimal) and
  P(hits ≥ 5) threshold sheets (Swiss correlations too weak to exploit).

- **v6** (2026-06-10): sigmoid scale 2.197 → 3.0, justified by a
  192-observation reliability study on resolved results (see Calibration).
- **v6.1** (2026-06-10): punch-up adjustment — a signed post-blend edge
  shift from each team's record against stronger opposition (see below).

---

## Signal Table

| Signal | Weight | Source | Notes |
|--------|--------|--------|-------|
| Elo | 0.28 | CS2-era match history | Opponent-adjusted; connectivity haircut for isolated pools |
| Baseline WR | 0.15 | Roster-stable match history | LAN-preferred, S-Tier-weighted, recency-decayed |
| Market | 0.15 | Polymarket winner odds | Volume-gated: <$10k → neutral 0.5; $200k+ → full trust |
| VRS rank | 0.12 | Valve Regional Standings | Official Valve global rank, cohort-relative |
| Roster stability | 0.10 | Roster history | Penalises stand-ins, inactive starters |
| Live form | 0.10 | Stage standings W/L | Defaults to 0.5 pre-tournament |
| Stage entry tier | 0.05 | Stage entry (1/2/3) | Stage 3 invites = strongest seed |
| Momentum | 0.05 | Last 30d vs older form | Trend bucket (improving/stable/declining) |
| Region | 0.00 | Removed in v4 | Elo encodes strength-of-schedule |

**Punch-up adjustment (v6.1, applied after the blend):** `edge += 0.10 × residual`,
where the residual is the recency-weighted mean of (actual − Elo-expected)
outcome against opposition rated 25+ Elo higher, over the trailing 540 days
(180-day half-life, minimum 8 effective matches, else no adjustment).
Derived from the full CS2-era match graph (~40k matches), not just Major
history: it credits teams that systematically beat their rating against
stronger opposition and docks teams that fold upward. Validated
point-in-time on 8 modern-format stages: advance Brier 0.2172 → 0.2141,
improvement on 6 of 8 stages.

**Map-pool depth adjustment (v7, applied after the blend):** `edge += 0.10 × depth`
on all-BO3 stages (Stage 3, Playoffs) and `0.05 × depth` otherwise, where
depth is the cohort-centered fraction of the window's 7 most-played maps on
which the team holds a recency-weighted map win rate ≥ 0.5 (365-day window,
180-day half-life, minimum effective sample per map). Derived from per-map
results parsed from Liquipedia match popups. Gate test at the
pre-registered weight: advance Brier 0.2170 → 0.2157, log-loss
0.6210 → 0.6187, monotone in the weight. Coverage at gate time was
Majors-only; an event-page scraper extends coverage between Majors and the
weight is re-tested before the next event.

---

## Swiss Simulation

5-round Swiss bracket (3 wins = advance, 3 losses = eliminated).

- Round 1: seeded by edge score (1v9, 2v10, ..., 8v16)
- Rounds 2-5: paired within same-record Buchholz buckets; rematch avoidance
- Match format: BO1 for rounds 1-2; BO3 when match decides advance or elimination
- Win probability per map: `sigmoid(3.0 × (edge_a − edge_b))` (v6: calibrated against 192 resolved team-stage results so 0.5 edge gap → ~82% win rate; v5 used 2.197 → 75%, which a reliability study showed was too compressed — teams predicted 65–80% to advance did so 84% of the time)
- BO3 probability: `P² × (3 − 2P)`
- H2H blending: if ≥ 3 historical current-roster matches exist, blends H2H win rate with sigmoid prior (weight = √n / (√n + 5))
- Simulations: 10,000–20,000 iterations per run

## Playoff Simulation

Single-elimination BO3 (8 teams from Stage 3).

- Bracket: QF (1v8, 2v7, 3v6, 4v5) → SF → Final
- Same sigmoid + BO3 probability function as Swiss
- Outputs: P(champion), P(finalist), P(semifinalist), P(quarterfinalist)

---

## Pick Selection

Greedy slot-priority fill across 10 slots (2 × 3-0, 6 × advance, 2 × 0-3):

1. Fill 3-0 slots: top teams by P(3-0)
2. Fill advance slots: top remaining teams by P(advance) − P(3-0)
3. Fill 0-3 slots: top remaining teams by P(0-3)

Confidence band: High / Medium / Low based on slot-relative probability thresholds.

---

## Calibration

After each stage resolves, the model is graded against actual outcomes:

- **Advance Brier score**: mean((P(advance) − actual)²) — reference: 0.25 = coin flip
- **Advance log-loss**: mean −log(P | outcome) — reference: 0.693 = coin flip
- **Advance accuracy**: fraction of P(advance) > 0.5 calls that were correct
- **Pick'em hit counts**: correct picks per slot type (3-0 / advance / 0-3) out of 10

Calibration data accumulates across Majors to enable future grid-search weight tuning.

### Backtest (v5, 3,938 CS2 matches, train/test split)

| Hold-out | Accuracy | Log-loss | Brier |
|----------|----------|----------|-------|
| 30d | 63.0% | 0.651 | 0.229 |
| 60d | 67.4% | 0.644 | 0.226 |
| 90d | 67.2% | 0.655 | 0.231 |
| Coin flip | 50.0% | 0.693 | 0.250 |

---

## Limitations

- Sparse history: teams with < 5 current-roster matches use Bayesian shrinkage toward a prior
- Market signal: Polymarket has non-trivial overround and liquidity varies by team
- Region pools: Asian and Oceanic teams have limited top-tier cross-regional matches; Elo connectivity haircut partially compensates
- Model weights are evidence-informed estimates, not grid-search optimised (calibration data accumulating for future tuning)

---

## Decision Records

| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-05-30 | Publish derived outputs only | Raw scraped data and model code stay private |
| 2026-05-30 | Prediction lock at `stage_start_at` | Prevents retroactive editing; archive credibility |
| 2026-05-30 | Final outcome write-once | Immutable record after resolution |
| 2026-05-30 | Screenshots manual-only | Automation never writes to `screenshots/` |
| 2026-05-30 | Option A discovery | Curated page slugs instead of open-ended crawl; fail-closed |
| 2026-06-10 | v6: sigmoid scale 2.197 → 3.0 | Reliability study on 192 resolved results showed compressed probabilities; Brier-optimal interior minimum at 3.0 on 3-stage-format Majors. Slot picks unaffected (ranking is scale-invariant) |
| 2026-06-10 | v6.1: punch-up adjustment (w=0.10) | Elo residual vs stronger opposition from the full match graph; Brier 0.2172 → 0.2141 on 8 stages, 6/8 improved. Same study rejected a BO3/BO1 format split and a recent-form resume blend (both flat or worse) |
| 2026-06-10 | v7: map-pool depth (w=0.10 BO3 stages / 0.05 otherwise) | Per-map data parsed from stage-page popups (691 rows, 5 Majors); Brier 0.2170 → 0.2157 at the pre-registered weight. Same study rejected optimal-assignment pick sheets (greedy ~99.8% optimal) and P(hits≥5) threshold sheets (correlations too weak) |
