# Sudoku 数独 Solver

> If you've not yet completed the [Sudoku Validator](Sudoku-Validator.md) - it's **strongly** recommended to start there.

![Sudoku Puzzle](img/sudoku.png)

Inspired by the classic Japanese logic puzzle - this challenge is simple, but will take time to solve:

**Create a program that _completes_ a solution to a Sudoku puzzle.**

> ⚠ It's _highly_ recommended to either run this as a long Dojo (min 2 hours) and/or across a series to allow people to work on and evolve their codebase.

* Given a 9x9 grid
* Each _row_, _column_ and _subgrid_ should contain the digits 1-9 with **no duplicates**.
* A 'subgrid' is a 3x3 block created when dividing the grid into thirds.
* Depending on difficulty - some of the numbers will be pre-filled (the more, the easier the puzzle).
* **Complete the grid!**

The completed sample puzzle looks like:

![Completed Sudoku Puzzle](img/sudoku-solution.png)

These puzzles can be _very_ challenging - _unless you're a programmer!_ 💪👩‍💻👨‍💻

## The Challenge

Create a solution finder that takes the digits of the grid, reading top-left to bottom-right. Incomplete digits will be marked as a `0`.

Complete the grid, and return a string with the no zeroes - and a **valid** solution to the puzzle.

For example - given the first line of input - the program should return the second line as output:

```
010902087063085000020070516057096003306210704004703000002030040800049005000800031
415962387763185492928374516157496823396218754284753169672531948831649275549827631
```

```
580102040000000216910704003000020000203910700790003405600001504150040672300200089
586132947437598216912764853865427391243915768791683425629871534158349672374256189
```

```
000003060080050700015080040800300009349006000206090370000400506700008002090000430
427913865683254791915687243871345629349726158256891374132479586764538912598162437
```

```
008090400302760000100020008600000020000010000200803000000500807000600004070089005
568391472342768951197425638685947123734216589219853746926534817851672394473189265
```

This Dojo is less about the solution, and more about how we design, model and test possible solutions.

* Ideally, work in a pair/mob.
* Document design discussions - what hypotheses do you have to solve?
* How did those solutions work out?
* How _easy_ was it to test hypotheses?
* What trade-offs did you notice about "easy to code" vs. "hard to compute" (if any)?
* **Write up a short narrative and present your findings to the rest of Dojo.**

> 😩 **Struggling to come up with approaches to solve the problem?** Try to avoid searching for algorithms that solve puzzles. The goal isn't to get to 'best' approach quickly - it's how you design and iterate towards it.


## Stars

* ⭐ Able to form a hypotheses - pick the 'simplest' (or first! 😁), and get it running.
* ⭐⭐ Tested multiple hypotheses - and picked the fastest.
* ⭐⭐⭐ Code is highly optimised _and_ readable - considering such (but not limited to):
    1.  There's limited answers _possible_.
    2.  Not all _possible_ answers are _correct_.
    3.  Different _possibilities_ may require different _algorithms_.
    4.  Different puzzle _difficulties_ may require different _algorithms_.
    5.  👑 Data is royal. Can you measure/track/prove performance?
  

## Additional

* Puzzles (and solutions) can be found by creating a `GET` request to Sudoku.com ([easy](https://sudoku.com/api/getLevel/easy) / [medium](https://sudoku.com/api/getLevel/medium) / [hard](https://sudoku.com/api/getLevel/hard) / [expert](https://sudoku.com/api/getLevel/expert)).