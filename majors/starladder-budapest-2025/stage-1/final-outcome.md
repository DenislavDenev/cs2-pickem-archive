> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-11-23, with the same model that powers the current Major's live predictions (bo1_edge_v6.1). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# StarLadder Budapest Major 2025 -- Stage 1 Final Outcome

_Scored: 2026-06-09 23:57 UTC_

---

## Final Standings

| Team               | Record | Status         |
| ------------------ | ------ | -------------- |
| FlyQuest           | 3-0    | 3-0            |
| M80                | 3-0    | 3-0            |
| B8                 | 3-1    | advanced-3-1   |
| Fnatic             | 3-1    | advanced-3-1   |
| Ninjas_in_Pyjamas  | 3-1    | advanced-3-1   |
| FaZe_Clan          | 3-2    | advanced-3-2   |
| Imperial_Esports   | 3-2    | advanced-3-2   |
| PARIVISION         | 3-2    | advanced-3-2   |
| Fluxo              | 2-3    | eliminated-2-3 |
| Legacy             | 2-3    | eliminated-2-3 |
| NRG                | 2-3    | eliminated-2-3 |
| GamerLegion        | 1-3    | eliminated-1-3 |
| RED_Canids         | 1-3    | eliminated-1-3 |
| The_Huns_Esports   | 1-3    | eliminated-1-3 |
| Lynn_Vision_Gaming | 0-3    | eliminated-0-3 |
| Rare_Atom          | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team        | Result  |
| ---------- | ------------------ | ------- |
| 0-3_pick_1 | FlyQuest           | MISS    |
| 0-3_pick_2 | RED_Canids         | MISS    |
| 3-0_pick_1 | Legacy             | MISS    |
| 3-0_pick_2 | FaZe_Clan          | MISS    |
| advance_1  | PARIVISION         | CORRECT |
| advance_2  | Rare_Atom          | MISS    |
| advance_3  | GamerLegion        | MISS    |
| advance_4  | Lynn_Vision_Gaming | MISS    |
| advance_5  | The_Huns_Esports   | MISS    |
| advance_6  | M80                | MISS    |

**Total: 1 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.288 | 0.250                 |
| Advance Log-loss     | 0.774 | 0.693                 |
| Advance Accuracy     | 31.2% | 50.0%                 |
| Pick'em Hits (total) | 1     | —                     |

---

## Model Misses

- **FlyQuest** (slot 0-3_pick_1): model gave 21.9% confidence -- did not hit.
- **RED_Canids** (slot 0-3_pick_2): model gave 18.5% confidence -- did not hit.
- **Legacy** (slot 3-0_pick_1): model gave 26.3% confidence -- did not hit.
- **FaZe_Clan** (slot 3-0_pick_2): model gave 25.0% confidence -- did not hit.
- **Rare_Atom** (slot advance_2): model gave 60.7% confidence -- did not hit.
- **GamerLegion** (slot advance_3): model gave 56.5% confidence -- did not hit.
- **Lynn_Vision_Gaming** (slot advance_4): model gave 53.0% confidence -- did not hit.
- **The_Huns_Esports** (slot advance_5): model gave 52.7% confidence -- did not hit.
- **M80** (slot advance_6): model gave 46.6% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
