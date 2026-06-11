# Melanies_games

Chess games by analogy of our [Melanie Bot on lichess](https://lichess.org/?user=argolab_org_Melanie#friend).

Melanie picks her moves by **relational analogy to named master games** — no material evaluation, no
search-driven heuristics in the analogy itself. For every move (from move 10 on; moves 1–9 are a
Stockfish opening), each game folder includes a **thought report** (PDF) that shows, move by move,
the board positions she retrieved and the exact source game, ply, and piece-role correspondence (μ)
that produced the move. The reports are generated **purely programmatically** from her own move
records — no human or LLM writes any of the prose.

## Games

| Date (UTC) | Opponent | Result | Game | Report |
|---|---|---|---|---|
| 2026-06-11 20:23 | eraoul | 1–0 | [lichess](https://lichess.org/imTGIp02) | [thought report (PDF)](games/2026-06-11_vs_eraoul_imTGIp02/report.pdf) |
| 2026-06-11 19:54 | alex-linhares | 1–0 | [lichess](https://lichess.org/BCsz4MpS) | [thought report (PDF)](games/2026-06-11_vs_alex-linhares_BCsz4MpS/report.pdf) |

_Games are unranked; player ratings are omitted from the reports and this index._

Each game folder contains the `game.pgn`, the `report.pdf`, and the `thoughts/` source
(per-move JSON records + the generated `report.tex`) so every report is fully reproducible.
