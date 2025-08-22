<h1 align="center"> UC Berkeley CS188 Intro to AI - Pac-Man Project </h1>

<p align="center"> This project implements various search algorithms to solve maze navigation problems for Pac-Man. Based on UC Berkeley's CS188 Introduction to Artificial Intelligence course, it demonstrates practical applications of algorithms like BFS, DFS, A*, and others in an AI pathfinding context. The implementation covers solutions to Questions 1-4 of Project 1 from the course.</p>
<div align="center">
  <img src="https://raw.githubusercontent.com/PeymanRM/Pac-Man/refs/heads/main/imgs/Banner.gif" alt="screenshot" />
</div>

## Implemented Algorithms

1. Breadth-First Search (BFS)
2. Non-recursive Depth-First Search (DFS)
3. Recursive Depth-First Search (DFS)
4. Uniform-Cost Search (UCS)
5. Greedy Search (GS)
6. A* Search (with Manhattan heuristic)

## How to Use

To run the Pac-Man game with different search algorithms, use the command line interface as follows:
```bash
python pacman.py -l <layout> -p SearchAgent -a fn=<algorithm>
```
### Parameters:
- `layout`: The maze layout you want to use. Examples include:
  - `tinyMaze`
  - `mediumMaze`
  - `bigMaze`
- `algorithm`: The search algorithm to apply. Options include:
  - `bfs`: Breadth-First Search
  - `dfs`: Depth-First Search, non-recursive
  - `astar,heuristic=manhattanHeuristic`: A* Search, with manhattanHeuristic
  - `ucs`: Uniform-Cost Search
  - `gs,heuristic=manhattanHeuristic`: Greedy Search, with manhattanHeuristic

### Examples:
1. Running BFS on a tiny maze:
      ```bash
      python pacman.py -l tinyMaze -p SearchAgent -a fn=bfs
      ```
2. Running A* search on a big maze with Manhattan heuristic:
      ```bash
     python pacman.py -l bigMaze -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
      ```

## Acknowledgments

- UC Berkeley's [CS188 Intro to AI](http://ai.berkeley.edu/) course materials.
- The Pac-Man framework provided by the course staff.
