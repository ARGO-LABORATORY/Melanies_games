# Experiment: ANALOGY vs SEARCH (decorrelated book openings)

Head-to-head between two Melanie variants over **9 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `analogy_vs_search_nightly`)

**ANALOGY 7 — 7 SEARCH**  (draws: 4, games: 18)

## Results by opening (cell = winner, or "draw")

| Opening | ANALOGY as White | SEARCH as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | ANALOGY | draw | +87 |
| Benko Gambit | SEARCH | SEARCH | +83 |
| Bogo-Indian | draw | ANALOGY | +52 |
| Caro-Kann, Advance | SEARCH | draw | +18 |
| Caro-Kann, Classical | ANALOGY | SEARCH | +41 |
| Caro-Kann, Panov | ANALOGY | SEARCH | +37 |
| Caro-Kann, Two Knights | ANALOGY | ANALOGY | +26 |
| Catalan | draw | SEARCH | +32 |
| Dutch, Leningrad | ANALOGY | SEARCH | +66 |
