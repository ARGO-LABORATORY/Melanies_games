# Experiment: ANALOGY vs SEARCH (decorrelated book openings)

Head-to-head between two Melanie variants over **16 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `analogy_vs_search_20260615_202149`)

**ANALOGY 11 — 9 SEARCH**  (draws: 11, games: 31)

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
| Ruy Lopez, Closed | ANALOGY | — | +38 |
