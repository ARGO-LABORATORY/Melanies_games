# Experiment: Masters-corpus vs Bots-corpus — decorrelated (book openings)

Same analogy engine, two corpora (MASTERS=human games, BOTS=CCRL engine games), played head-to-head
from **21 different balanced opening positions** (from `openings_book.json`), **each played
both colors**, so the sample spans many structures rather than one repeated line.
Engine speed lever: `R_QAP=16` on both sides (fair); analogy takes over right after the book.

## Score (run `masters_vs_bots_book_20260612_024941`)

**MASTERS 13 — 22 BOTS**  (draws: 6, games: 41)

Each game folder has `game.pgn` + both per-side report PDFs + reproducible `thoughts/`. A Stockfish
"move-quality verdict" (per-side ACPL) is appended after the match (referee only).

## Results by opening

| Opening | MASTERS as White | BOTS as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | 1-0 (MASTERS) | 0-1 (MASTERS) | +87 |
| Bogo-Indian | 0-1 (BOTS) | 1-0 (BOTS) | +52 |
| Caro-Kann, Panov | 1/2-1/2 (draw) | 0-1 (MASTERS) | +37 |
| Catalan | 0-1 (BOTS) | 1-0 (BOTS) | +32 |
| Dutch, Stonewall | 0-1 (BOTS) | 1-0 (BOTS) | +53 |
| English, Symmetrical | 1-0 (MASTERS) | 1/2-1/2 (draw) | +40 |
| French, Classical | 0-1 (BOTS) | 1-0 (BOTS) | +38 |
| French, Tarrasch | 1-0 (MASTERS) | 0-1 (MASTERS) | +46 |
| Grunfeld | 0-1 (BOTS) | 0-1 (MASTERS) | +32 |
| King's Indian, Classical | 1-0 (MASTERS) | 1-0 (BOTS) | +61 |
| London System | 0-1 (BOTS) | 0-1 (MASTERS) | +8 |
| Nimzo-Indian | 1/2-1/2 (draw) | 1-0 (BOTS) | +25 |
| QGD, Exchange | 0-1 (BOTS) | 1-0 (BOTS) | +36 |
| Queen's Gambit Accepted | 1/2-1/2 (draw) | 1-0 (BOTS) | +32 |
| Reti Opening | 0-1 (BOTS) | 0-1 (MASTERS) | +27 |
| Ruy Lopez, Closed | 1-0 (MASTERS) | 0-1 (MASTERS) | +38 |
| Scotch Game | 1-0 (MASTERS) | 1/2-1/2 (draw) | +0 |
| Semi-Slav | 0-1 (BOTS) | 1-0 (BOTS) | +31 |
| Sicilian, Alapin | 1/2-1/2 (draw) | 1-0 (BOTS) | +26 |
| Sicilian, Dragon | 0-1 (BOTS) | 1-0 (BOTS) | +61 |
| Sicilian, Najdorf | 0-1 (BOTS) | — | +36 |


---

## Stockfish verdict (move quality)

Stockfish (depth 14) scored every analogy-phase move (move 10+) of all 41 games.
**Centipawn-loss** = how much each move worsened the position vs Stockfish's best (lower = better play).
Stockfish is referee only — never in either engine's move choice.

| | MASTERS (human corpus) | BOTS (engine corpus) |
|---|---|---|
| Games won | 13 | 22 |
| Mean cp-loss | **113** | **112** |
| Median cp-loss | 51 | 44 |
| Blunders (≥300cp) | 219 | 235 |
| Moves analyzed | 2802 | 2804 |

Draws: 6. **BOTS played better** by mean centipawn-loss (112 vs 113 cp, gap 1).

| Game | Result | Winner | MASTERS ACPL | BOTS ACPL |
|---|---|---|---|---|
| game_01Bw | 0-1 | MASTERS | 84 | 94 |
| game_01Mw | 1-0 | MASTERS | 114 | 120 |
| game_02Bw | 1-0 | BOTS | 89 | 92 |
| game_02Mw | 0-1 | BOTS | 109 | 64 |
| game_03Bw | 0-1 | MASTERS | 167 | 145 |
| game_03Mw | 1/2-1/2 | draw | 61 | 60 |
| game_04Bw | 1-0 | BOTS | 77 | 84 |
| game_04Mw | 0-1 | BOTS | 126 | 144 |
| game_05Bw | 1-0 | BOTS | 70 | 60 |
| game_05Mw | 0-1 | BOTS | 116 | 138 |
| game_06Bw | 1/2-1/2 | draw | 45 | 45 |
| game_06Mw | 1-0 | MASTERS | 80 | 85 |
| game_07Bw | 1-0 | BOTS | 95 | 152 |
| game_07Mw | 0-1 | BOTS | 120 | 103 |
| game_08Bw | 0-1 | MASTERS | 42 | 120 |
| game_08Mw | 1-0 | MASTERS | 138 | 129 |
| game_09Bw | 0-1 | MASTERS | 55 | 135 |
| game_09Mw | 0-1 | BOTS | 69 | 76 |
| game_10Bw | 1-0 | BOTS | 132 | 104 |
| game_10Mw | 1-0 | MASTERS | 55 | 43 |
| game_11Bw | 0-1 | MASTERS | 117 | 104 |
| game_11Mw | 0-1 | BOTS | 115 | 88 |
| game_12Bw | 1-0 | BOTS | 94 | 75 |
| game_12Mw | 1/2-1/2 | draw | 113 | 95 |
| game_13Bw | 1-0 | BOTS | 206 | 201 |
| game_13Mw | 0-1 | BOTS | 158 | 196 |
| game_14Bw | 1-0 | BOTS | 120 | 28 |
| game_14Mw | 1/2-1/2 | draw | 86 | 89 |
| game_15Bw | 0-1 | MASTERS | 106 | 133 |
| game_15Mw | 0-1 | BOTS | 121 | 103 |
| game_16Bw | 0-1 | MASTERS | 79 | 100 |
| game_16Mw | 1-0 | MASTERS | 94 | 121 |
| game_17Bw | 1/2-1/2 | draw | 97 | 104 |
| game_17Mw | 1-0 | MASTERS | 171 | 133 |
| game_18Bw | 1-0 | BOTS | 110 | 104 |
| game_18Mw | 0-1 | BOTS | 119 | 129 |
| game_19Bw | 1-0 | BOTS | 139 | 139 |
| game_19Mw | 1/2-1/2 | draw | 146 | 108 |
| game_20Bw | 1-0 | BOTS | 104 | 134 |
| game_20Mw | 0-1 | BOTS | 132 | 148 |
| game_21Mw | 0-1 | BOTS | 127 | 99 |
