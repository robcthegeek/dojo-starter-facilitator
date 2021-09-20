# Sudoku 数独 Validator

> This Kata was inspired by a puzzle on [CodinGame](https://www.codingame.com/ide/puzzle/sudoku-validator).

![Sudoku Puzzle](img/sudoku.png)

Inspired by the classic Japanese logic puzzle - this challenge is simple:

**Create a program that _validates_ a solution to a Sudoku puzzle.**

* Given a 9x9 grid
* Each _row_, _column_ and _subgrid_ should contain the digits 1-9 with **no duplicates**.
* A 'subgrid' is a 3x3 block created when dividing the grid into thirds.
* Depending on difficulty - some of the numbers will be pre-filled (the more, the easier the puzzle).
* **Complete the grid!**

The completed sample puzzle looks like:

![Completed Sudoku Puzzle](img/sudoku-solution.png)

These puzzles can be _very_ challenging - _unless you're a programmer!_ 💪👩‍💻👨‍💻

## The Challenge

We need to be able to **_validate_ if a solution is correct**.

* Given a string of `81` digits (as it's a `9x9`) grid - determine if the solution is valid given the rules above.
* Treat the string as printed from 'top-left to bottom-right'. The first 9 digits being the first row, the second the second and so on.
* Return `true` if the solution is valid, `false` if otherwise.

### Tests

_Taken from [CodinGame](https://www.codingame.com/ide/puzzle/sudoku-validator):_

| # | Input | Output |
| --- | --- | --- |
| 1 | `123456789456789123789123456912345678345678912678912345891234567234567891567891234` | `true` |
| 2 | `435269781682571493197834562826195347374682915951743628519326874248957136763418259` | `true` |
| 3 | `432269781685571493197834562826195347374682915951743628519326874248957136763418259` | `false` (Row Error) |
| 4 | `435269781682571493197834562826195347374682915159743628519326874248957136763418259` | `false` (Column Error) |
| 5 | `435269781682571493897134562126895347374682915951743628519326874248957136763418259` | `false` (Subgrid Error) |
| 6 | `596142537614358248569412536195368416593634821595321456136486525412368492368741563` | `false` (Incorrect Grid) 
| 7 | `133456779456779133779133456913345677345677913677913345791334567334567791567791334` | `false` (?? _Spoiler_) |

## Stars

* ⭐ Tests 1-6 Passing
* ⭐⭐ Test 7 Passing
* ⭐⭐⭐ Discuss, model and _seamlessly_ implement a _Super_-Sudoku validator. The same rules, a `16x16` grid (with `4x4` subgrids). This means numbers will go from 1-16 - for simplicity in parsing, you may want to use [hex values](https://en.wikipedia.org/wiki/Hexadecimal#Representation).

## Considerations

* As always - consider the DevX of working with your code! How easy is it to determine if there's a problem with the validator?

---

## Additional

* Puzzles (and solutions) can be found by creating a `GET` request to Sudoku.com ([easy](https://sudoku.com/api/getLevel/easy) / [medium](https://sudoku.com/api/getLevel/medium) / [hard](https://sudoku.com/api/getLevel/hard) / [expert](https://sudoku.com/api/getLevel/expert)).
* Done? Now create a [Sudoku Solver](Sudoku-Solver.md)!