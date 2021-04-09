[![docker](https://github.com/karlbateman/pandora/actions/workflows/docker.yaml/badge.svg)](https://github.com/karlbateman/pandora/actions/workflows/docker.yaml)

# Pandora

> [Sudoku] Solver.

## Introduction

A toy solver which generates solutions for the following board configurations:

* 4x4 board with 2x2 regions
* 9x9 board with 3x3 regions

For simplicity no other types of board are supported!

## Getting Started

The Sudoku board state is read from `stdin`, the solver expects a 2D grid of numbers in a square, where blank spots are
represented by `.` (dots). For example inputs, please see the `examples/` directory. Whitespace is ignored when reading
in the initial board.

```bash
cat examples/9x9example_1.txt | docker run --rm -i karlbateman/pandora
```

## License

[BSD] © [@karlbateman]

[Sudoku]: https://en.wikipedia.org/wiki/Sudoku
[Boost]: https://www.boost.org/
[Ubuntu]: https://ubuntu.com
[BSD]: LICENSE
[@karlbateman]: https://github.com/karlbateman
