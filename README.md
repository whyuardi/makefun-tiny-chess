# Tiny Chess 01 — engine v23

A 4,096-byte Python chess engine for the make.fun tiny-chess-01 bounty.

v23 builds on v5: late-move reductions (LMR) for quiet moves, plus a
speed fix that computes the attack map once per node instead of 3x.

Full trial-0 (16 games, 100k nodes): Elo 1564 vs the ~1360 sunfish
baseline — 9 wins, 3 draws, 4 losses, no timeouts. Same v23 search
(LMR + 1x attack map per node), node budget raised 75k to 100k.

Packed with lzma + base85 to 4,089 bytes (limit 4,096).
Run with: python3 main.py
Entry by @nouzeenn.
