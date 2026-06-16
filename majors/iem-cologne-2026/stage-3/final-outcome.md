# Intel Extreme Masters/2026/Cologne -- Stage 3 Final Outcome

_Scored: 2026-06-16 01:00 UTC_

---

## Final Standings

| Team          | Record | Status         |
| ------------- | ------ | -------------- |
| FURIA         | 3-0    | 3-0            |
| Team_Spirit   | 3-0    | 3-0            |
| Aurora_Gaming | 3-1    | advanced-3-1   |
| Team_Falcons  | 3-1    | advanced-3-1   |
| Team_Vitality | 3-1    | advanced-3-1   |
| 9z_Team       | 3-2    | advanced-3-2   |
| BetBoom_Team  | 3-2    | advanced-3-2   |
| G2_Esports    | 3-2    | advanced-3-2   |
| FUT_Esports   | 2-3    | eliminated-2-3 |
| Natus_Vincere | 2-3    | eliminated-2-3 |
| The_MongolZ   | 2-3    | eliminated-2-3 |
| Legacy        | 1-3    | eliminated-1-3 |
| MOUZ          | 1-3    | eliminated-1-3 |
| Monte         | 1-3    | eliminated-1-3 |
| B8            | 0-3    | eliminated-0-3 |
| PARIVISION    | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team   | Result  |
| ---------- | ------------- | ------- |
| 0-3_pick_1 | Monte         | MISS    |
| 0-3_pick_2 | PARIVISION    | CORRECT |
| 3-0_pick_1 | Team Vitality | MISS    |
| 3-0_pick_2 | Team Falcons  | MISS    |
| advance_1  | Team Spirit   | MISS    |
| advance_2  | FURIA         | MISS    |
| advance_3  | Aurora Gaming | CORRECT |
| advance_4  | Natus Vincere | MISS    |
| advance_5  | MOUZ          | MISS    |
| advance_6  | 9z Team       | CORRECT |

**Total: 3 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.140 | 0.250                 |
| Advance Log-loss     | 0.426 | 0.693                 |
| Advance Accuracy     | 75.0% | 50.0%                 |
| Pick'em Hits (total) | 3     | —                     |

---

## Model Misses

- **Monte** (slot 0-3_pick_1): model gave 39.8% confidence -- did not hit.
- **Team Vitality** (slot 3-0_pick_1): model gave 57.9% confidence -- did not hit.
- **Team Falcons** (slot 3-0_pick_2): model gave 32.2% confidence -- did not hit.
- **Team Spirit** (slot advance_1): model gave 95.4% confidence -- did not hit.
- **FURIA** (slot advance_2): model gave 84.2% confidence -- did not hit.
- **Natus Vincere** (slot advance_4): model gave 56.0% confidence -- did not hit.
- **MOUZ** (slot advance_5): model gave 52.4% confidence -- did not hit.

---

Locked prediction: [Locked prediction snapshot](https://github.com/DenislavDenev/cs2-pickem-archive/commit/1b8bbf0bae2c1ccf2bd3995e926ef2f7581387ab)

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
