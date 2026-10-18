# Constraint Satisfaction and Search Algorithms

This assignment explores how to assign **200 chemicals to storage cabinets** while satisfying pairwise placement constraints. The objective is to find a conflict-free configuration and compare different optimization and search strategies in a large combinatorial state space.

## Part 1: Local Search and Optimization

Implement and evaluate algorithms that iteratively improve chemical assignments by reducing constraint violations.

**Algorithms covered:**

* **Hill Climbing:** Accepts changes that reduce the number of conflicts.
* **Simulated Annealing:** Uses probabilistic acceptance to help escape local minima.
* **Genetic Algorithm:** Evolves a population of candidate assignments through selection, crossover, and mutation.
* **Iterative Min-Conflicts:** Selects a highly conflicted chemical and changes its cabinet.
* **Beam Search:** Maintains multiple candidate states and selects promising successors using a heuristic.

The algorithms are evaluated by tracking conflict counts across iterations and comparing their search performance.

## Part 2: Backtracking Search

Implement depth-first search (DFS) to construct a valid assignment incrementally.

**Key concepts:**

* Representing the problem as a constraint satisfaction problem (CSP).
* Assigning chemicals one at a time and rejecting conflicting assignments.
* Using backtracking to explore alternative cabinet assignments.
* Counting visited states and checking whether a valid solution exists.

## Part 3: Feasible State Space

Estimate the proportion of valid assignments by sampling random configurations and checking whether they satisfy all constraints.

The assignment also examines the size of the overall state space and the difficulty of finding feasible solutions as the number of chemicals and cabinets grows.

## Part 4: Theoretical Analysis

Compare the strengths and limitations of the implemented algorithms.

**Topics covered:**

* Why local search can become trapped in local minima.
* How temperature schedules, population diversity, heuristics, and conflict selection affect performance.
* Why backtracking differs from iterative conflict minimization.
* Which search approaches can guarantee a minimum cabinet count.
* State-space size, feasibility, completeness, and computational complexity.

## Learning Outcomes

* Model a real-world allocation problem as a constraint satisfaction problem.
* Implement and compare local search, evolutionary optimization, and systematic search.
* Evaluate algorithms using conflict counts, explored states, and empirical success.
* Understand the trade-offs between heuristic efficiency and guaranteed solutions.
