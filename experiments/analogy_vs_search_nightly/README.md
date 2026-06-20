# Experiment: ANALOGY vs SEARCH (decorrelated book openings)

Head-to-head between two Melanie variants over **32 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `analogy_vs_search_nightly`)

**ANALOGY 17 — 23 SEARCH**  (draws: 23, games: 63)

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
| Dutch, Stonewall | SEARCH | draw | +53 |
| English, Reversed Sicilian | SEARCH | SEARCH | +19 |
| English, Symmetrical | ANALOGY | draw | +40 |
| Four Knights | draw | SEARCH | +35 |
| French, Advance | draw | draw | +59 |
| French, Classical | SEARCH | SEARCH | +38 |
| French, Rubinstein | draw | SEARCH | +53 |
| French, Tarrasch | SEARCH | SEARCH | +46 |
| French, Winawer | SEARCH | draw | +69 |
| Grunfeld | ANALOGY | ANALOGY | +32 |
| Italian, Giuoco Pianissimo | ANALOGY | ANALOGY | +24 |
| King's Indian Attack | ANALOGY | SEARCH | +3 |
| King's Indian, Classical | draw | ANALOGY | +61 |
| King's Indian, Fianchetto | SEARCH | ANALOGY | +59 |
| London System | SEARCH | draw | +8 |
| Modern Benoni | ANALOGY | SEARCH | +79 |
| Nimzo-Indian | draw | SEARCH | +25 |
| Petroff Defense | draw | draw | +52 |
| Pirc Defense | draw | SEARCH | +62 |
| QGD, Exchange | ANALOGY | draw | +36 |
| QGD, Orthodox | draw | draw | +19 |
| Queen's Gambit Accepted | draw | draw | +32 |
| Queen's Indian | draw | — | +36 |
