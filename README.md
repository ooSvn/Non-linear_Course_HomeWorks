
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

---

### `gradient_newton_methods.py`

This script implements and compares two optimization algorithms for minimizing quadratic functions.

#### **1. Gradient Descent with Backtracking Line Search**

* **Functions**:

  * `grad_calculator(coeff, x)` → computes gradient of $f(x, y) = a x^2 + b y^2$.
  * `f(coeff, x)` → evaluates the quadratic function.
  * `grad_BT(coeffs, x_0, s, beta, alpha, tolerance)` → gradient descent with backtracking.

* **Algorithm**:

  * Starts from an initial guess.
  * Adjusts step size using the Armijo condition.
  * Iterates until gradient norm is below tolerance.

* **Experiment**:

  * Analyzes effect of the **y-coefficient** on the number of iterations.
  * Visualization shows that balanced curvatures improve convergence speed.

#### **2. Pure Newton’s Method**

* **Functions**:

  * `hessian_calculator(coeffs)` → computes Hessian matrix.
  * `pure_newton(coeffs, x_0, tolerance)` → Newton’s method for quadratic optimization.

* **Algorithm**:

  * Uses exact curvature information (Hessian inverse).
  * Updates solution in a single step for quadratic functions.
  * Number of iterations remains stable regardless of coefficient scaling.

* **Experiment**:

  * Varies the coefficient of $y$ and plots number of iterations.
  * Demonstrates the robustness of Newton’s method for quadratic problems.

---

---

**File: `Data_Fitting_&_Denoising.py`**

**Description:**
This file contains implementations for **image denoising** and **data fitting** tasks using **Regularized Least Squares (RLS)** and **polynomial regression**.

* **Q1 – Image Denoising:**

  * Implements RLS-based denoising on grayscale images.
  * Applies different regularization parameters (λ) and multi-run strategies.
  * Includes analysis of method suitability, performance, and weaknesses.

* **Q2 – Data Fitting:**

  * Polynomial fitting on several datasets.
  * Integrates RLS-based denoising to improve fitting accuracy.
  * Evaluates error and demonstrates effect of noise and outliers.

**Dependencies:** `numpy`, `matplotlib`, `opencv-python`

**Usage:**
Run the file to visualize denoised images, fitted curves, and error analysis for different datasets.

---
