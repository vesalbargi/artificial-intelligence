# Linear Programming and Optimization

This assignment explores **linear programming** through two practical optimization problems. It focuses on finding optimal solutions under constraints and formulating real-world resource allocation problems as mathematical optimization models.

## Part 1: Corner Point Method

Implement the Corner Point Method to solve a linear programming problem with two decision variables and multiple linear constraints.

**Key tasks:**

* Generate possible vertices by finding intersections between pairs of constraint boundaries.
* Use NumPy to solve systems of linear equations and identify unique intersections.
* Check each candidate point against all constraints to determine feasibility.
* Evaluate feasible vertices and identify the one that maximizes the objective function.

**Result:** Find the optimal solution and examine why certain constraint combinations produce infeasible points or fail to form unique vertices.

## Part 2: Online Advertising Optimization

Formulate an online advertising allocation problem inspired by how search platforms allocate ads across queries and advertisers.

The objective is to **maximize expected advertising revenue** while respecting available resources and advertiser budgets.

**Key concepts:**

* **Decision variables:** Represent the number of ad impressions allocated to each advertiser for each search query.
* **Objective function:** Maximize expected revenue based on click-through rates and advertiser bids.
* **Budget constraints:** Ensure that the expected advertising cost for each advertiser stays within its budget.
* **Impression constraints:** Prevent the allocation from exceeding the available search volume for each query.
* **Non-negativity:** Ensure that all allocation values are non-negative.

**Result:** Develop a linear programming formulation for an advertising allocation problem involving three advertisers and three search queries. Solving the model for an optimal allocation is an optional extension.

## References

## References

1. Carnegie Mellon University — [Optimization Assignment](https://www.cs.cmu.edu/~15381-s19/assignments/programming/optimization/index.html)
2. MIT OpenCourseWare — [The Analytics Edge: Linear Optimization](https://ocw.mit.edu/courses/15-071-the-analytics-edge-spring-2017/pages/linear-optimization/)
