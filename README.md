# tiny-chess-riegan

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/rikyansyah/tiny-chess-riegan/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/rikyansyah/tiny-chess-riegan/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in a single Python file. The board is a 0x88 array kept from the side to move's point of view, flipped after every move; the search is negamax alpha-beta with a transposition table, killer-free MVV-LVA ordering and a quiescence search over captures, promotions and check evasions; the evaluation is material plus piece-square tables. It searches to a fixed node budget, never to a clock, so every move is deterministic. The readable source is `engine.py`; `main.py` is its compressed form, packed with `makefun compress`.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 -P -s main.py
```

Point `MAKEFUN_ENV_URL` at a tiny-chess env and the engine plays the whole gauntlet, one game after another, then exits.

---

Entered on [make.fun](https://make.fun/?ref=vrsa6rr4&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards
