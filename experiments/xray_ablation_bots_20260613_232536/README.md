# Experiment: BASE vs XRAY (decorrelated book openings)

Head-to-head between two Melanie variants over **7 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `xray_ablation_bots_20260613_232536`)

**BASE 5 — 3 XRAY**  (draws: 6, games: 14)

## Results by opening (cell = winner, or "draw")

| Opening | BASE as White | XRAY as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | draw | BASE | +87 |
| Bogo-Indian | draw | XRAY | +52 |
| Caro-Kann, Panov | BASE | draw | +37 |
| Catalan | XRAY | BASE | +32 |
| Dutch, Stonewall | draw | BASE | +53 |
| English, Symmetrical | XRAY | BASE | +40 |
| French, Classical | draw | draw | +38 |


---

## Stockfish verdict (move quality)

Stockfish (depth 14) scored every analogy-phase move of all 14 games. **Centipawn-loss**
= how much each move worsened the position vs Stockfish's best (lower = better play). Referee only.

| | BASE | XRAY |
|---|---|---|
| Games won | 5 | 3 |
| Mean cp-loss | **117** | **113** |
| Median cp-loss | 52 | 57 |
| Blunders (>=300cp) | 48 | 45 |
| Moves analyzed | 638 | 636 |

Draws: 6. **XRAY played more accurately** by mean centipawn-loss (113 vs 117 cp, gap 4).

| Game | Result | Winner | BASE ACPL | XRAY ACPL |
|---|---|---|---|---|
| game_01Aw | 1/2-1/2 | draw | 100 | 101 |
| game_01Bw | 0-1 | BASE | 53 | 71 |
| game_02Aw | 1/2-1/2 | draw | 69 | 69 |
| game_02Bw | 1-0 | XRAY | 156 | 162 |
| game_03Aw | 1-0 | BASE | 39 | 103 |
| game_03Bw | 1/2-1/2 | draw | 52 | 52 |
| game_04Aw | 0-1 | XRAY | 90 | 101 |
| game_04Bw | 0-1 | BASE | 157 | 169 |
| game_05Aw | 1/2-1/2 | draw | 46 | 52 |
| game_05Bw | 0-1 | BASE | 112 | 119 |
| game_06Aw | 0-1 | XRAY | 153 | 125 |
| game_06Bw | 0-1 | BASE | 154 | 104 |
| game_07Aw | 1/2-1/2 | draw | 101 | 102 |
| game_07Bw | 1/2-1/2 | draw | 161 | 139 |
