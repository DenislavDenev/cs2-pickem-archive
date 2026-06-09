> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-12-03, with the same model that powers the current Major's live predictions (bo1_edge_v6). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# StarLadder Budapest Major 2025 -- Stage 3 Final Outcome

_Scored: 2026-06-09 23:08 UTC_

---

## Final Standings

| Team             | Record | Status         |
| ---------------- | ------ | -------------- |
| FURIA            | 3-0    | 3-0            |
| Team_Spirit      | 3-0    | 3-0            |
| MOUZ             | 3-1    | advanced-3-1   |
| Team_Vitality    | 3-1    | advanced-3-1   |
| The_MongolZ      | 3-1    | advanced-3-1   |
| FaZe_Clan        | 3-2    | advanced-3-2   |
| Natus_Vincere    | 3-2    | advanced-3-2   |
| Team_Falcons     | 3-2    | advanced-3-2   |
| B8               | 2-3    | eliminated-2-3 |
| G2_Esports       | 2-3    | eliminated-2-3 |
| Passion_UA       | 2-3    | eliminated-2-3 |
| 3DMAX            | 1-3    | eliminated-1-3 |
| Imperial_Esports | 1-3    | eliminated-1-3 |
| paiN_Gaming      | 1-3    | eliminated-1-3 |
| PARIVISION       | 0-3    | eliminated-0-3 |
| Team_Liquid      | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team      | Result  |
| ---------- | ---------------- | ------- |
| 0-3_pick_1 | paiN_Gaming      | MISS    |
| 0-3_pick_2 | Imperial_Esports | MISS    |
| 3-0_pick_1 | Team_Vitality    | MISS    |
| 3-0_pick_2 | FURIA            | CORRECT |
| advance_1  | MOUZ             | CORRECT |
| advance_2  | Team_Falcons     | CORRECT |
| advance_3  | Team_Spirit      | MISS    |
| advance_4  | Natus_Vincere    | CORRECT |
| advance_5  | G2_Esports       | MISS    |
| advance_6  | The_MongolZ      | CORRECT |

**Total: 5 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.123 | 0.250                 |
| Advance Log-loss     | 0.410 | 0.693                 |
| Advance Accuracy     | 87.5% | 50.0%                 |
| Pick'em Hits (total) | 5     | —                     |

---

## Model Misses

- **paiN_Gaming** (slot 0-3_pick_1): model gave 28.3% confidence -- did not hit.
- **Imperial_Esports** (slot 0-3_pick_2): model gave 27.5% confidence -- did not hit.
- **Team_Vitality** (slot 3-0_pick_1): model gave 43.0% confidence -- did not hit.
- **Team_Spirit** (slot advance_3): model gave 75.6% confidence -- did not hit.
- **G2_Esports** (slot advance_5): model gave 57.3% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
