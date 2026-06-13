# Experiment: BASE vs XRAY (decorrelated book openings)

Head-to-head between two Melanie variants over **1 balanced opening positions**
(`openings_book.json`), **each played both colors**. `R_QAP=64` on both sides; analogy takes
over right after the book. Each game folder has `game.pgn` + both per-side report PDFs + reproducible
`thoughts/`. A Stockfish move-quality verdict (per-side ACPL) is appended after the match.

## Score (run `xray_ablation_bots_20260613_232536`)

**BASE 1 — 0 XRAY**  (draws: 1, games: 2)

## Results by opening (cell = winner, or "draw")

| Opening | BASE as White | XRAY as White | Eval@book |
|---|---|---|---|
| Alekhine Defense | draw | BASE | +87 |
