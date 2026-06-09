> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-06-02, with the same model that powers the current Major's live predictions (bo1_edge_v6.1). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# BLAST.tv Austin Major 2025 -- Stage 1 Final Outcome

_Scored: 2026-06-09 23:57 UTC_

---

## Final Standings

| Team               | Record | Status         |
| ------------------ | ------ | -------------- |
| B8                 | 3-0    | 3-0            |
| HEROIC             | 3-0    | 3-0            |
| BetBoom_Team       | 3-1    | advanced-3-1   |
| Nemiga_Gaming      | 3-1    | advanced-3-1   |
| OG                 | 3-1    | advanced-3-1   |
| Legacy             | 3-2    | advanced-3-2   |
| Lynn_Vision_Gaming | 3-2    | advanced-3-2   |
| TYLOO              | 3-2    | advanced-3-2   |
| FlyQuest           | 2-3    | eliminated-2-3 |
| NRG                | 2-3    | eliminated-2-3 |
| Wildcard           | 2-3    | eliminated-2-3 |
| Chinggis_Warriors  | 1-3    | eliminated-1-3 |
| Complexity         | 1-3    | eliminated-1-3 |
| Imperial_Esports   | 1-3    | eliminated-1-3 |
| Fluxo              | 0-3    | eliminated-0-3 |
| Metizport          | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team        | Result  |
| ---------- | ------------------ | ------- |
| 0-3_pick_1 | HEROIC             | MISS    |
| 0-3_pick_2 | FlyQuest           | MISS    |
| 3-0_pick_1 | TYLOO              | MISS    |
| 3-0_pick_2 | Fluxo              | MISS    |
| advance_1  | B8                 | MISS    |
| advance_2  | Legacy             | CORRECT |
| advance_3  | NRG                | MISS    |
| advance_4  | Imperial_Esports   | MISS    |
| advance_5  | BetBoom_Team       | CORRECT |
| advance_6  | Lynn_Vision_Gaming | CORRECT |

**Total: 3 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.251 | 0.250                 |
| Advance Log-loss     | 0.699 | 0.693                 |
| Advance Accuracy     | 62.5% | 50.0%                 |
| Pick'em Hits (total) | 3     | —                     |

---

## Model Misses

- **HEROIC** (slot 0-3_pick_1): model gave 27.5% confidence -- did not hit.
- **FlyQuest** (slot 0-3_pick_2): model gave 18.8% confidence -- did not hit.
- **TYLOO** (slot 3-0_pick_1): model gave 25.4% confidence -- did not hit.
- **Fluxo** (slot 3-0_pick_2): model gave 19.9% confidence -- did not hit.
- **B8** (slot advance_1): model gave 66.1% confidence -- did not hit.
- **NRG** (slot advance_3): model gave 57.1% confidence -- did not hit.
- **Imperial_Esports** (slot advance_4): model gave 53.6% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
