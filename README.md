
### `Optimization_problem.py`

This script contains three optimization problems formulated and solved using **CVXPY**:

* **Q1 – Appropriate Diet (Diet Problem)**

  * Goal: Minimize the cost of food while satisfying minimum nutritional requirements.
  * Approach: Linear programming with non-negativity constraints.
  * Output: Optimal food quantities, nutrition levels received, and minimum cost.

* **Q2 – Project Management (Resource Allocation Problem)**

  * Goal: Minimize the total cost of allocating resources to tasks, considering deadlines, resource limits, and minimum benefit requirements.
  * Approach: Linear programming with inequality constraints on time, resources, and productivity.
  * Output: Optimal resource allocation, minimum cost, and spent time.

* **Q3 – Portfolio Selection (Mean-Variance Optimization)**

  * Goal: Maximize return on investment while balancing risk (variance).
  * Approach: Quadratic programming with portfolio weights summing to 1 and non-negativity constraints.
  * Output: Optimal investment distribution, total return, maximized utility value, and portfolio variance.

---
