# IEM Cologne Major 2026 -- Stage 1 Final Outcome

_Scored: 2026-06-06 10:40 UTC_

---

## Final Standings

| Team               | Record | Status         |
| ------------------ | ------ | -------------- |
| B8                 | 3-0    | 3-0            |
| BetBoom_Team       | 3-0    | 3-0            |
| GamerLegion        | 3-1    | advanced-3-1   |
| M80                | 3-1    | advanced-3-1   |
| MIBR               | 3-1    | advanced-3-1   |
| BIG                | 3-2    | advanced-3-2   |
| FlyQuest           | 3-2    | advanced-3-2   |
| TYLOO              | 3-2    | advanced-3-2   |
| Lynn_Vision_Gaming | 2-3    | eliminated-2-3 |
| NRG                | 2-3    | eliminated-2-3 |
| Team_Liquid        | 2-3    | eliminated-2-3 |
| HEROIC             | 1-3    | eliminated-1-3 |
| Sharks_Esports     | 1-3    | eliminated-1-3 |
| THUNDERdOWNUNDER   | 1-3    | eliminated-1-3 |
| Gaimin_Gladiators  | 0-3    | eliminated-0-3 |
| SINNERS_Esports    | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team       | Result  |
| ---------- | ----------------- | ------- |
| 0-3_pick_1 | NRG               | MISS    |
| 0-3_pick_2 | Gaimin Gladiators | CORRECT |
| 3-0_pick_1 | GamerLegion       | MISS    |
| 3-0_pick_2 | BetBoom Team      | CORRECT |
| advance_1  | B8                | MISS    |
| advance_2  | MIBR              | CORRECT |
| advance_3  | M80               | CORRECT |
| advance_4  | BIG               | CORRECT |
| advance_5  | Sharks Esports    | MISS    |
| advance_6  | TYLOO             | CORRECT |

**Total: 6 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.163 | 0.250                 |
| Advance Log-loss     | 0.509 | 0.693                 |
| Advance Accuracy     | 87.5% | 50.0%                 |
| Pick'em Hits (total) | 7     | —                     |

---

## Model Misses

- **NRG** (slot 0-3_pick_1): model gave 23.9% confidence -- did not hit.
- **GamerLegion** (slot 3-0_pick_1): model gave 31.9% confidence -- did not hit.
- **Sharks Esports** (slot advance_5): model gave 51.6% confidence -- did not hit.

---

Locked prediction: [Locked prediction snapshot](https://github.com/DenislavDenev/cs2-pickem-archive/commit/9e56f49e6bfbbc7fdc1b939581800cb879f7012b)

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
