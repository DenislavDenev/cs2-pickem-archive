> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-11-28, with the same model that powers the current Major's live predictions (bo1_edge_v7). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# StarLadder Budapest Major 2025 -- Stage 2 Final Outcome

_Scored: 2026-06-10 12:29 UTC_

---

## Final Standings

| Team              | Record | Status         |
| ----------------- | ------ | -------------- |
| FaZe_Clan         | 3-0    | 3-0            |
| Natus_Vincere     | 3-0    | 3-0            |
| B8                | 3-1    | advanced-3-1   |
| Imperial_Esports  | 3-1    | advanced-3-1   |
| PARIVISION        | 3-1    | advanced-3-1   |
| 3DMAX             | 3-2    | advanced-3-2   |
| Passion_UA        | 3-2    | advanced-3-2   |
| Team_Liquid       | 3-2    | advanced-3-2   |
| Astralis          | 2-3    | eliminated-2-3 |
| M80               | 2-3    | eliminated-2-3 |
| Ninjas_in_Pyjamas | 2-3    | eliminated-2-3 |
| Aurora_Gaming     | 1-3    | eliminated-1-3 |
| Fnatic            | 1-3    | eliminated-1-3 |
| TYLOO             | 1-3    | eliminated-1-3 |
| FlyQuest          | 0-3    | eliminated-0-3 |
| MIBR              | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team      | Result  |
| ---------- | ---------------- | ------- |
| 0-3_pick_1 | Imperial_Esports | MISS    |
| 0-3_pick_2 | MIBR             | CORRECT |
| 3-0_pick_1 | Natus_Vincere    | CORRECT |
| 3-0_pick_2 | Aurora_Gaming    | MISS    |
| advance_1  | Team_Liquid      | CORRECT |
| advance_2  | FaZe_Clan        | MISS    |
| advance_3  | M80              | MISS    |
| advance_4  | B8               | CORRECT |
| advance_5  | 3DMAX            | CORRECT |
| advance_6  | PARIVISION       | CORRECT |

**Total: 6 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.222 | 0.250                 |
| Advance Log-loss     | 0.634 | 0.693                 |
| Advance Accuracy     | 75.0% | 50.0%                 |
| Pick'em Hits (total) | 6     | —                     |

---

## Model Misses

- **Imperial_Esports** (slot 0-3_pick_1): model gave 21.3% confidence -- did not hit.
- **Aurora_Gaming** (slot 3-0_pick_2): model gave 18.5% confidence -- did not hit.
- **FaZe_Clan** (slot advance_2): model gave 61.6% confidence -- did not hit.
- **M80** (slot advance_3): model gave 60.5% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
