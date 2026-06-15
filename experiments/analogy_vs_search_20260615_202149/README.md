# Experiment: ANALOGY vs SEARCH (decorrelated book openings)

Head-to-head between two Melanie variants over **4 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `analogy_vs_search_20260615_202149`)

**ANALOGY 3 — 2 SEARCH**  (draws: 2, games: 7)

## Results by opening (cell = winner, or "draw")

| Opening | ANALOGY as White | SEARCH as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | ANALOGY | draw | +87 |
| Bogo-Indian | SEARCH | ANALOGY | +52 |
| Caro-Kann, Panov | ANALOGY | SEARCH | +37 |
| Catalan | draw | — | +32 |
