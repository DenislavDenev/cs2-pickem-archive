# Intel Extreme Masters/2026/Cologne -- Stage 2 Final Outcome

_Scored: 2026-06-09 20:08 UTC_

---

## Final Standings

| Team         | Record | Status         |
| ------------ | ------ | -------------- |
| FUT_Esports  | 3-0    | 3-0            |
| Team_Spirit  | 3-0    | 3-0            |
| 9z_Team      | 3-1    | advanced-3-1   |
| BetBoom_Team | 3-1    | advanced-3-1   |
| G2_Esports   | 3-1    | advanced-3-1   |
| B8           | 3-2    | advanced-3-2   |
| Legacy       | 3-2    | advanced-3-2   |
| Monte        | 3-2    | advanced-3-2   |
| BIG          | 2-3    | eliminated-2-3 |
| TYLOO        | 2-3    | eliminated-2-3 |
| paiN_Gaming  | 2-3    | eliminated-2-3 |
| Astralis     | 1-3    | eliminated-1-3 |
| M80          | 1-3    | eliminated-1-3 |
| MIBR         | 1-3    | eliminated-1-3 |
| FlyQuest     | 0-3    | eliminated-0-3 |
| GamerLegion  | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team  | Result  |
| ---------- | ------------ | ------- |
| 0-3_pick_1 | FlyQuest     | CORRECT |
| 0-3_pick_2 | M80          | MISS    |
| 3-0_pick_1 | Team Spirit  | CORRECT |
| 3-0_pick_2 | G2 Esports   | MISS    |
| advance_1  | FUT Esports  | MISS    |
| advance_2  | 9z Team      | CORRECT |
| advance_3  | GamerLegion  | MISS    |
| advance_4  | Legacy       | CORRECT |
| advance_5  | BetBoom Team | CORRECT |
| advance_6  | B8           | CORRECT |

**Total: 6 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.175 | 0.250                 |
| Advance Log-loss     | 0.533 | 0.693                 |
| Advance Accuracy     | 80.0% | 50.0%                 |
| Pick'em Hits (total) | 6     | —                     |

---

## Model Misses

- **M80** (slot 0-3_pick_2): model gave 21.3% confidence -- did not hit.
- **G2 Esports** (slot 3-0_pick_2): model gave 19.7% confidence -- did not hit.
- **FUT Esports** (slot advance_1): model gave 63.5% confidence -- did not hit.
- **GamerLegion** (slot advance_3): model gave 56.2% confidence -- did not hit.

---

Locked prediction: [Locked prediction snapshot](https://github.com/DenislavDenev/cs2-pickem-archive/commit/92de95f0141301ddc7e25e137c79b6de58a7abe1)

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
