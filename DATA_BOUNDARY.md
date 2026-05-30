# Data Boundary

This repository contains only derived model outputs. The following lists are exhaustive.

---

## Published in this repo

- Per-team Monte Carlo probabilities: P(3-0), P(advance), P(0-3)
- 10-slot pick'em recommendations with confidence bands and key drivers
- Sanitized decision metrics: normalized Elo, VRS rank, market signal value, roster stability score, live form record, momentum score, baseline source
- Final stage standings: record and terminal status per team
- Pick'em scorecards: correct/miss per slot
- Calibration metrics: Brier score, log-loss, accuracy, hit counts
- Screenshots (added manually before stage start)

---

## Never published here

- Airflow DAG source code
- Scraper source code
- Raw match rows (match_id, scores, individual match results)
- Player rows (player_id, nationality, career rows)
- Raw roster rows
- Raw market price history or snapshots
- BigQuery staging table contents
- Google Cloud credentials or service account keys
- Liquipedia raw HTML or API responses
- Internal model intermediates (Elo ratings per match iteration, baseline computation details)
