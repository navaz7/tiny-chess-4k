# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/navaz7/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/navaz7/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 4 KB of Python: negamax alpha-beta search with quiescence, a transposition table, null-move pruning, late-move reductions, killer ordering and tapered piece-square evaluation, packed as an lzma payload in `main.py`. It plays the make.fun gauntlet through the env at a fixed budget of 50,000 nodes per move — no clock, no randomness, so every trial replays move for move.

## Run it

The engine is driven by the competition env: set `MAKEFUN_ENV_URL` to the env's origin and run

```sh
python3 -P -s main.py
```

It plays every game the env serves, then exits.
