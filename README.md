
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


Nice 👍 you’ve got a **custom Cholesky Factorization** implementation here along with a solver for linear equations.
Here’s how I’d add this file’s explanation to your README:

---

### `cholesky_factorization.py`

This script implements the **Cholesky Factorization** method from scratch and compares it with NumPy’s built-in function.

* **`choleskyFactorization(A)`**

  * Recursively computes the lower triangular matrix $L$ such that $A = L L^T$.
  * Uses matrix partitioning and updates submatrices.

* **`MSE(x, y)`**

  * Calculates the Mean Squared Error (MSE) between two matrices (used to compare custom vs. NumPy implementation).

* **Example Usage**

  * Performs Cholesky factorization on test matrices.
  * Prints the custom factorization vs. NumPy’s result along with the MSE.

* **Equation Solving (`solveEquation`)**

  * Uses the Cholesky factorization to solve linear equations $A x = b$.
  * Back-substitution with $L$ and $L^T$ is applied.
  * Example provided with a $3 \times 3$ system.

---

