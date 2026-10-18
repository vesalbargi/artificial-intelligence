# Sliding Puzzle Search

This assignment explores **state-space search algorithms** by solving the 8-puzzle, a sliding tile puzzle in which numbered tiles must be arranged into a target configuration. The goal is to find a valid solution while minimizing search effort.

## Part 1: Uninformed Search

Implement **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** to find a sequence of moves that solves the puzzle.

**Key concepts:**

* State representation and successor generation.
* Using queues and stacks to manage the search frontier.
* Tracking explored states to avoid unnecessary revisits.
* Comparing explored nodes, memory consumption, and solution optimality.

## Part 2: Informed Search with A*

Implement **A* search** using the Manhattan distance heuristic to guide the search toward the goal state.

**Key concepts:**

* Combining path cost and heuristic estimates to prioritize states.
* Using a priority queue to expand promising states first.
* Measuring search performance by the number of explored states and maximum frontier size.
* Reconstructing and displaying the solution path.

## Part 3: Search Algorithm Analysis

Explore theoretical properties and compare search strategies based on their behavior and performance.

**Topics covered:**

* How goal-testing timing affects solution optimality.
* Differences between informed and uninformed search.
* Estimating frontier growth and distinguishing tree search from graph search.
* Heuristic admissibility and consistency, and their role in A* optimality.
* Comparing BFS, DFS, Uniform-Cost Search (UCS), Iterative Deepening DFS (IDDFS), and A* in terms of memory usage, execution time, completeness, and optimality.
