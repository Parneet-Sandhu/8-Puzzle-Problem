# 8-Puzzle-Problem
# Solving the 8-Puzzle Problem Using BFS
## Overview
This code demonstrates solving the 8-puzzle problem using Breadth-First Search (BFS) as a state-space search technique. The 8-puzzle is a classic problem that involves sliding tiles in a 3x3 grid to match a desired goal configuration.

The algorithm explores the shortest path from an initial configuration to the goal state and visualizes the steps involved in solving the puzzle.

## What is the 8-Puzzle Problem?
The 8-puzzle consists of:

- A 3x3 grid with 8 numbered tiles (1 to 8) and one blank space (0).
- A goal to rearrange the tiles from a starting configuration to the desired target state by sliding adjacent tiles into the blank space.
## Example
- Initial State
```bash
1  2  3
4  5  6
0  7  8
```
- Goal State
```bash
1  2  3
4  5  6
7  8  0
```

## How the Code Works
### Breadth-First Search (BFS)
BFS is used to find the shortest solution path:

1. Start from the initial state.
2. Explore all possible moves (Up, Down, Left, Right) from the current state.
3. Add new states to a queue and mark visited states to avoid loops.
4. Stop when the goal state is reached.

### Visualization
Each step of the solution path is visualized using Matplotlib to show how the tiles are rearranged until the goal state is achieved.

## Key Functions
1. bfs_solve:
- Implements BFS to find the solution path.
- Returns a list of states from the initial to the goal configuration.
2. visualize_puzzle:
- Visualizes the solution path as a sequence of grids, showing how the tiles move.

## Output
- **Visualization:** Displays the step-by-step solution in a series of grids.
- **Textual Output:** If no solution exists, the program prints No solution found.
## Why BFS?
- **Guarantees Shortest Path:** BFS explores all states level-by-level.
- **Complete:** Ensures that a solution is found if one exists.

## Use Cases
- Understanding search algorithms in AI.
- Practicing state-space search problems.
- Visualizing problem-solving processes.

Enjoy solving puzzles programmatically! 🎉
