# Experiment: Masters-corpus Melanie vs Bots-corpus Melanie

Same analogy engine, two different "minds": one allowed to reason **only from human master games**, the other **only from top-engine (CCRL) games** — played head to head.

Melanie chooses moves by relational analogy to a corpus of named games. Here we split that corpus by provenance and pit the two halves against each other. **Everything else is identical** (the 2-ply analogy-guided search, the piece-role correspondence μ, the translation); the *only* difference is which games each side may retrieve its analogies from:

- **MASTERS** — human games only (`lichess_elite`, `twic`). → [masters_report.pdf](masters_report.pdf)
- **BOTS** — CCRL top-engine games only (`ccrl_top`). → [bots_report.pdf](bots_report.pdf)

The two PDFs show, **move by move**, the positions each side retrieved and the exact source game + ply + piece-role correspondence (μ) behind every move — so you can read the *same* engine "thinking" in two different worlds. Reports are generated purely programmatically from the engine's own move records (no human or LLM writes the prose).

## This game

- A Berlin Ruy Lopez (moves 1–9 are a shared Stockfish opening; analogy reasoning begins at move 10).
- MASTERS played White, BOTS played Black.
- **A 25-move snapshot** from a capped demo run (result unfinished, `*`) — the point is the *reasoning*, not the result. 16 analogy moves per side. `game.pgn` has the moves.

## What to look for

- Every MASTERS move cites a **human** game (`lichess_elite_…`, `twic…`); every BOTS move cites a **CCRL engine** game (`ccrl_top_…`). The provenance split is total.
- **Cross-type analogies abound on both sides** — e.g. a pawn push transferred from a game where the master moved a *bishop*, a knight maneuver from a *pawn* move. The role, not the piece type, carries the analogy (the project's thesis).

`masters/` and `bots/` hold the per-move JSON records + the generated `report.tex` so each PDF is fully reproducible.
