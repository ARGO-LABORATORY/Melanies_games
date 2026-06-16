# Experiment: ANALOGY vs SEARCH (decorrelated book openings)

Head-to-head between two Melanie variants over **17 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `analogy_vs_search_20260615_202149`)

**ANALOGY 12 — 9 SEARCH**  (draws: 12, games: 33)

## Results by opening (cell = winner, or "draw")

| Opening | ANALOGY as White | SEARCH as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | ANALOGY | draw | +87 |
| Bogo-Indian | SEARCH | ANALOGY | +52 |
| Caro-Kann, Panov | ANALOGY | SEARCH | +37 |
| Catalan | draw | SEARCH | +32 |
| Dutch, Stonewall | SEARCH | ANALOGY | +53 |
| English, Symmetrical | ANALOGY | draw | +40 |
| French, Classical | ANALOGY | SEARCH | +38 |
| French, Tarrasch | SEARCH | SEARCH | +46 |
| Grunfeld | ANALOGY | ANALOGY | +32 |
| King's Indian, Classical | draw | draw | +61 |
| London System | SEARCH | draw | +8 |
| Nimzo-Indian | draw | SEARCH | +25 |
| QGD, Exchange | ANALOGY | draw | +36 |
| Queen's Gambit Accepted | draw | draw | +32 |
| Reti Opening | draw | ANALOGY | +27 |
| Ruy Lopez, Closed | ANALOGY | draw | +38 |
| Scotch Game | ANALOGY | — | +0 |


---

## Stockfish verdict (move quality)

Stockfish (depth 14) scored every analogy-phase move of all 33 games. **Centipawn-loss**
= how much each move worsened the position vs Stockfish's best (lower = better play). Referee only.

| | ANALOGY | SEARCH |
|---|---|---|
| Games won | 12 | 9 |
| Mean cp-loss | **136** | **131** |
| Median cp-loss | 43 | 47 |
| Blunders (>=300cp) | 207 | 190 |
| Moves analyzed | 1772 | 1774 |

Draws: 12. **SEARCH played more accurately** by mean centipawn-loss (131 vs 136 cp, gap 5).

| Game | Result | Winner | ANALOGY ACPL | SEARCH ACPL |
|---|---|---|---|---|
| game_01Aw | 1-0 | ANALOGY | 151 | 155 |
| game_01Bw | 1/2-1/2 | draw | 37 | 44 |
| game_02Aw | 0-1 | SEARCH | 117 | 104 |
| game_02Bw | 0-1 | ANALOGY | 43 | 97 |
| game_03Aw | 1-0 | ANALOGY | 180 | 161 |
| game_03Bw | 1-0 | SEARCH | 84 | 81 |
| game_04Aw | 1/2-1/2 | draw | 75 | 80 |
| game_04Bw | 1-0 | SEARCH | 176 | 113 |
| game_05Aw | 0-1 | SEARCH | 123 | 101 |
| game_05Bw | 0-1 | ANALOGY | 184 | 129 |
| game_06Aw | 1-0 | ANALOGY | 173 | 174 |
| game_06Bw | 1/2-1/2 | draw | 115 | 151 |
| game_07Aw | 1-0 | ANALOGY | 123 | 135 |
| game_07Bw | 1-0 | SEARCH | 152 | 110 |
| game_08Aw | 0-1 | SEARCH | 93 | 62 |
| game_08Bw | 1-0 | SEARCH | 97 | 74 |
| game_09Aw | 1-0 | ANALOGY | 368 | 373 |
| game_09Bw | 0-1 | ANALOGY | 140 | 132 |
| game_10Aw | 1/2-1/2 | draw | 70 | 70 |
| game_10Bw | 1/2-1/2 | draw | 103 | 108 |
| game_11Aw | 0-1 | SEARCH | 136 | 190 |
| game_11Bw | 1/2-1/2 | draw | 91 | 74 |
| game_12Aw | 1/2-1/2 | draw | 97 | 78 |
| game_12Bw | 1-0 | SEARCH | 209 | 176 |
| game_13Aw | 1-0 | ANALOGY | 60 | 89 |
| game_13Bw | 1/2-1/2 | draw | 88 | 85 |
| game_14Aw | 1/2-1/2 | draw | 119 | 123 |
| game_14Bw | 1/2-1/2 | draw | 95 | 97 |
| game_15Aw | 1/2-1/2 | draw | 76 | 74 |
| game_15Bw | 0-1 | ANALOGY | 156 | 158 |
| game_16Aw | 1-0 | ANALOGY | 78 | 92 |
| game_16Bw | 1/2-1/2 | draw | 152 | 142 |
| game_17Aw | 1-0 | ANALOGY | 131 | 106 |
