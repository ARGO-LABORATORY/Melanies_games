# Experiment: Masters-corpus vs Bots-corpus — decorrelated (book openings)

Same analogy engine, two corpora (MASTERS=human games, BOTS=CCRL engine games), played head-to-head
from **4 different balanced opening positions** (from `openings_book.json`), **each played
both colors**, so the sample spans many structures rather than one repeated line.
Engine speed lever: `R_QAP=16` on both sides (fair); analogy takes over right after the book.

## Score (run `masters_vs_bots_book_20260612_024941`)

**MASTERS 3 — 4 BOTS**  (draws: 1, games: 8)

Each game folder has `game.pgn` + both per-side report PDFs + reproducible `thoughts/`. A Stockfish
"move-quality verdict" (per-side ACPL) is appended after the match (referee only).

## Results by opening

| Opening | MASTERS as White | BOTS as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | 1-0 (MASTERS) | 0-1 (MASTERS) | +87 |
| Bogo-Indian | 0-1 (BOTS) | 1-0 (BOTS) | +52 |
| Caro-Kann, Panov | 1/2-1/2 (draw) | 0-1 (MASTERS) | +37 |
| Catalan | 0-1 (BOTS) | 1-0 (BOTS) | +32 |
