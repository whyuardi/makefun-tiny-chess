# Tiny Chess 01 — engine v23

A 4,096-byte Python chess engine for the make.fun tiny-chess-01 bounty.

v23 builds on v5: late-move reductions (LMR) for quiet moves, plus a
speed fix that computes the attack map once per node instead of 3x.

Full trial-0 (16 games, 75k nodes): Elo 1430 vs the ~1360 sunfish
baseline — 7 wins, 3 draws, 6 losses, no timeouts.

Packed with lzma + base85 to 4,081 bytes (limit 4,096).
Run with: python3 main.py
Entry by @nouzeenn.
