#  Sudoku CSP Solver

## Project Overview
This project implements a Constraint Satisfaction Problem (CSP) solver to tackle Sudoku puzzles of varying difficulties[cite: 75, 78]. [cite_start]The solver utilizes core Artificial Intelligence techniques to find valid assignments while minimizing computational search space[cite: 78].

## Technical Implementation
The solver is built using Python and implements the following CSP strategies:
**Backtracking Search:** A depth-first search algorithm that builds solutions incrementally
**AC-3 (Arc Consistency):** A pre-processing algorithm used to prune the domains of variables by enforcing consistency between neighboring cells[cite: 78, 196].
- **Forward Checking:** Monitors the domains of unassigned variables and terminates branches early if a domain becomes empty[cite: 78].
- **MRV Heuristic:** Implements the 'Minimum Remaining Values' heuristic to select the most constrained variable first, improving search efficiency.

## Deliverables Included
1. **Source Code:** Well-commented implementation of the CSP solver.
2. **Puzzle Solutions:** Solved grids for Easy, Medium, Hard, and Very Hard boards.
3. **Performance Analysis:** Statistics regarding the number of times `BACKTRACK` was called and the frequency of failures.

## Input Format
The program reads `.txt` files where:
* The file contains exactly 9 lines.
* Each line contains 9 digits (0-9).
* `0` represents an empty cell.
