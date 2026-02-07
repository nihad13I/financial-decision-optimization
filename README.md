# Stochastic Decision Optimization & Dynamic Programming
## Solving Multi-Stage Resource Allocation and Investment Problems

### Overview
This project implements three distinct optimization models using **Dynamic Programming (DP)** and **Backward Induction**. These models solve for optimal policies in scenarios involving financial liquidity management, capital budgeting, and stochastic investment outcomes.

### Problem Sets & Methodologies
1. **Optimal Borrowing Plan (Interest Minimization):**
   * **Objective:** Minimize total interest paid over a 50-day period with shifting interest rates and borrowing caps.
   * **Method:** Uses backward induction to identify the optimal day and amount to borrow based on future cash requirements.

2. **Knapsack-style Project Selection:**
   * **Objective:** Maximize total profit across five geographical regions subject to a $10M budget constraint.
   * **Method:** A multi-stage resource allocation DP that evaluates the cost-benefit trade-offs for different regional projects.

3. **Stochastic Investment Policy:**
   * **Part 1 (Expectation):** Maximizes the expected final cash amount over a 3-year horizon.
   * **Part 2 (Probability):** Maximizes the probability of achieving a specific financial goal ($20k threshold).
   * **Method:** Markov Chain-based state transitions to model risky assets (Investment A vs. B).

### Technical Stack
* **Language:** Python
* **Concepts:** Recursive optimization, State-Space modeling, Bellman Equations, and Backward Induction.
* **Libraries:** NumPy, SciPy (Norm distribution), Matplotlib.

### Key Results
* **Resource Allocation:** Successfully identified a policy yielding a maximum profit of $73M within a strict $10M budget.
* **Investment Success:** Determined that while Investment A maximizes expected value, Investment B is superior for maximizing the probability of meeting a specific survival threshold (79.75% success rate).
