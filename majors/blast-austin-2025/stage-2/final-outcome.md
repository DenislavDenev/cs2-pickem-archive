> **RETROACTIVE RELIABILITY TEST** -- This outcome grades a point-in-time reconstruction: the prediction above it was generated retroactively using only data available on 2025-06-06, with the same model that powers the current Major's live predictions (bo1_edge_v6). It exists to test that model's reliability on resolved results. It is not a pre-tournament prediction.

# BLAST.tv Austin Major 2025 -- Stage 2 Final Outcome

_Scored: 2026-06-09 23:08 UTC_

---

## Final Standings

| Team               | Record | Status         |
| ------------------ | ------ | -------------- |
| Legacy             | 3-0    | 3-0            |
| Virtus.pro         | 3-0    | 3-0            |
| 3DMAX              | 3-1    | advanced-3-1   |
| FURIA              | 3-1    | advanced-3-1   |
| paiN_Gaming        | 3-1    | advanced-3-1   |
| FaZe_Clan          | 3-2    | advanced-3-2   |
| Lynn_Vision_Gaming | 3-2    | advanced-3-2   |
| Nemiga_Gaming      | 3-2    | advanced-3-2   |
| B8                 | 2-3    | eliminated-2-3 |
| HEROIC             | 2-3    | eliminated-2-3 |
| MIBR               | 2-3    | eliminated-2-3 |
| M80                | 1-3    | eliminated-1-3 |
| TYLOO              | 1-3    | eliminated-1-3 |
| Team_Falcons       | 1-3    | eliminated-1-3 |
| BetBoom_Team       | 0-3    | eliminated-0-3 |
| OG                 | 0-3    | eliminated-0-3 |

---

## Pick'em Scorecard

| Slot       | Picked Team  | Result  |
| ---------- | ------------ | ------- |
| 0-3_pick_1 | HEROIC       | MISS    |
| 0-3_pick_2 | paiN_Gaming  | MISS    |
| 3-0_pick_1 | Team_Falcons | MISS    |
| 3-0_pick_2 | TYLOO        | MISS    |
| advance_1  | B8           | MISS    |
| advance_2  | FaZe_Clan    | CORRECT |
| advance_3  | 3DMAX        | CORRECT |
| advance_4  | BetBoom_Team | MISS    |
| advance_5  | Legacy       | MISS    |
| advance_6  | OG           | MISS    |

**Total: 2 / 10**

---

## Calibration

| Metric               | Value | Reference (coin-flip) |
| -------------------- | ----- | --------------------- |
| Advance Brier        | 0.301 | 0.250                 |
| Advance Log-loss     | 0.805 | 0.693                 |
| Advance Accuracy     | 37.5% | 50.0%                 |
| Pick'em Hits (total) | 2     | —                     |

---

## Model Misses

- **HEROIC** (slot 0-3_pick_1): model gave 26.7% confidence -- did not hit.
- **paiN_Gaming** (slot 0-3_pick_2): model gave 23.1% confidence -- did not hit.
- **Team_Falcons** (slot 3-0_pick_1): model gave 29.6% confidence -- did not hit.
- **TYLOO** (slot 3-0_pick_2): model gave 19.9% confidence -- did not hit.
- **B8** (slot advance_1): model gave 66.1% confidence -- did not hit.
- **BetBoom_Team** (slot advance_4): model gave 54.6% confidence -- did not hit.
- **Legacy** (slot advance_5): model gave 52.7% confidence -- did not hit.
- **OG** (slot advance_6): model gave 51.2% confidence -- did not hit.

---

Locked prediction: _Prediction commit SHA not recorded._

> **Attribution:** Team and tournament data sourced from [Liquipedia](https://liquipedia.net/counterstrike) under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Market data from [Polymarket](https://polymarket.com) public API.

> **Data boundary:** This file contains derived model outputs only. DAGs, scraper code, raw match rows, player rows, roster rows, raw market history, BigQuery staging tables, and credentials are never published. See [DATA_BOUNDARY.md](../../DATA_BOUNDARY.md).
