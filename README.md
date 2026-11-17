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

Ideas (not code) from c4ke (github.com/citrus610/c4ke), ice4
(github.com/MinusKelvin/ice4), 4ku (github.com/kz04px/4ku) and
Stockfish (github.com/official-stockfish/Stockfish). Eval weights
Texel-tuned on the lichess-big3-resolved positions (ct800.net).

MIT licensed, see LICENSE.
