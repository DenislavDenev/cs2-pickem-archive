> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-06-11, with the same model that powers the current Major's live predictions (bo1_edge_v7). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# BLAST.tv Austin Major 2025 -- Stage 3 Final Outcome

_Scored: 2026-06-10 12:29 UTC_

---

## Final Standings

| Team               | Record | Status         |
| ------------------ | ------ | -------------- |
| FURIA              | 3-0    | 3-0            |
| Team_Spirit        | 3-0    | 3-0            |
| FaZe_Clan          | 3-1    | advanced-3-1   |
| Natus_Vincere      | 3-1    | advanced-3-1   |
| Team_Vitality      | 3-1    | advanced-3-1   |
| MOUZ               | 3-2    | advanced-3-2   |
| The_MongolZ        | 3-2    | advanced-3-2   |
| paiN_Gaming        | 3-2    | advanced-3-2   |
| G2_Esports         | 2-3    | eliminated-2-3 |
| Legacy             | 2-3    | eliminated-2-3 |
| Virtus.pro         | 2-3    | eliminated-2-3 |
| 3DMAX              | 1-3    | eliminated-1-3 |
| Aurora_Gaming      | 1-3    | eliminated-1-3 |
| Lynn_Vision_Gaming | 1-3    | eliminated-1-3 |
| Nemiga_Gaming      | 0-3    | eliminated-0-3 |
| Team_Liquid        | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team   | Result  |
| ---------- | ------------- | ------- |
| 0-3_pick_1 | FURIA         | MISS    |
| 0-3_pick_2 | paiN_Gaming   | MISS    |
| 3-0_pick_1 | Team_Vitality | MISS    |
| 3-0_pick_2 | Team_Spirit   | CORRECT |
| advance_1  | MOUZ          | CORRECT |
| advance_2  | Natus_Vincere | CORRECT |
| advance_3  | G2_Esports    | MISS    |
| advance_4  | The_MongolZ   | CORRECT |
| advance_5  | FaZe_Clan     | CORRECT |
| advance_6  | Legacy        | MISS    |

**Total: 5 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.201 | 0.250                 |
| Advance Log-loss     | 0.590 | 0.693                 |
| Advance Accuracy     | 75.0% | 50.0%                 |
| Pick'em Hits (total) | 5     | —                     |

---

## Model Misses

- **FURIA** (slot 0-3_pick_1): model gave 29.4% confidence -- did not hit.
- **paiN_Gaming** (slot 0-3_pick_2): model gave 26.0% confidence -- did not hit.
- **Team_Vitality** (slot 3-0_pick_1): model gave 47.0% confidence -- did not hit.
- **G2_Esports** (slot advance_3): model gave 63.9% confidence -- did not hit.
- **Legacy** (slot advance_6): model gave 40.9% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
