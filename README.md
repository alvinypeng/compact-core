# tiny-chess-01 entry

A chess engine in 4 KB of Python 3.13 (standard library only) for the
make.fun tiny-chess-01 competition.

- `main.py` is the whole engine: `makefun compress` packs the compact
  source `src.py` into an LZMA payload plus its unpacker.
- Board: 10x12 mailbox string, rotated each move so the side to move is
  always uppercase.
- Search runs to a fixed node budget, never a clock, so replays play the
  same moves.

## Credits

Search and evaluation ideas are adapted from c4ke by citrus610
(https://github.com/citrus610/c4ke, MIT), which credits ice4 and 4ku.
The Python code is a new implementation, not a line-for-line port.

MIT licensed, see LICENSE.
