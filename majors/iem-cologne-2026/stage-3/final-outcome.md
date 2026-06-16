# Intel Extreme Masters/2026/Cologne -- Stage 3 Final Outcome

_Scored: 2026-06-16 11:17 UTC_

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
| 0-3_pick_2 | G2 Esports    | MISS    |
| 3-0_pick_1 | Team Vitality | MISS    |
| 3-0_pick_2 | Team Falcons  | MISS    |
| advance_1  | Team Spirit   | MISS    |
| advance_2  | Natus Vincere | MISS    |
| advance_3  | FURIA         | MISS    |
| advance_4  | The MongolZ   | MISS    |
| advance_5  | MOUZ          | MISS    |
| advance_6  | Aurora Gaming | CORRECT |

**Total: 1 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.210 | 0.250                 |
| Advance Log-loss     | 0.592 | 0.693                 |
| Advance Accuracy     | 56.2% | 50.0%                 |
| Pick'em Hits (total) | 1     | —                     |

---

## Model Misses

- **Monte** (slot 0-3_pick_1): model gave 36.6% confidence -- did not hit.
- **G2 Esports** (slot 0-3_pick_2): model gave 21.3% confidence -- did not hit.
- **Team Vitality** (slot 3-0_pick_1): model gave 58.2% confidence -- did not hit.
- **Team Falcons** (slot 3-0_pick_2): model gave 29.9% confidence -- did not hit.
- **Team Spirit** (slot advance_1): model gave 87.8% confidence -- did not hit.
- **Natus Vincere** (slot advance_2): model gave 73.1% confidence -- did not hit.
- **FURIA** (slot advance_3): model gave 68.7% confidence -- did not hit.
- **The MongolZ** (slot advance_4): model gave 50.5% confidence -- did not hit.
- **MOUZ** (slot advance_5): model gave 50.1% confidence -- did not hit.

---

Locked prediction: [Locked prediction snapshot](https://github.com/DenislavDenev/cs2-pickem-archive/commit/1b8bbf0bae2c1ccf2bd3995e926ef2f7581387ab)

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
