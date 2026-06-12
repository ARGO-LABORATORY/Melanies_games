# Experiment: Masters-corpus vs Bots-corpus — decorrelated (book openings)

Same analogy engine, two corpora (MASTERS=human games, BOTS=CCRL engine games), played head-to-head
from **9 different balanced opening positions** (from `openings_book.json`), **each played
both colors**, so the sample spans many structures rather than one repeated line.
Engine speed lever: `R_QAP=16` on both sides (fair); analogy takes over right after the book.

## Score (run `masters_vs_bots_book_20260612_024941`)

**MASTERS 6 — 9 BOTS**  (draws: 2, games: 17)

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
| Grunfeld | 0-1 (BOTS) | — | +32 |
