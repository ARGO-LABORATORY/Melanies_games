# Experiment: Masters-corpus vs Bots-corpus Melanie — overnight match

Same analogy engine, two corpora, played head-to-head over many full games (colors alternate each game).
The **only** difference between the sides is which games they retrieve analogies from:

- **MASTERS** — human games only (`lichess_elite`, `twic`).
- **BOTS** — CCRL top-engine games only (`ccrl_top`).

Everything else (the 2-ply analogy-guided search, the μ correspondence, translation) is identical. Each
game folder has `game.pgn`, both per-side thought-report PDFs (`masters_report.pdf`, `bots_report.pdf`)
showing every move's source game + role correspondence, and the reproducible `thoughts/` source.

## Score (run `masters_vs_bots_overnight_20260611_232406`)

**MASTERS 0 — 4 BOTS**  (draws: 1, games: 5)

| | |
|---|---|
| MASTERS (human corpus) wins | 0 |
| BOTS (engine corpus) wins | 4 |
| Draws | 1 |

Games adjudicated naturally (mate / 50-move / threefold / insufficient); ply-capped games are refereed
by Stockfish (referee only — never in either engine's move choice).

## Games

| # | White | Black | Result | Winner | Plies | Game |
|---|---|---|---|---|---|---|
| 1 | MASTERS | BOTS | 0-1 | BOTS | 192 | [g01](game_01/) |
| 2 | BOTS | MASTERS | 1-0 | BOTS | 103 | [g02](game_02/) |
| 3 | MASTERS | BOTS | 0-1 | BOTS | 162 | [g03](game_03/) |
| 4 | BOTS | MASTERS | 1-0 | BOTS | 103 | [g04](game_04/) |
| 5 | MASTERS | BOTS | 1/2-1/2 | draw | 93 | [g05](game_05/) |
