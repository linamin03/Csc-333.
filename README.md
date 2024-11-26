# Csc-333.   README for Linear Programming Solutions

This README provides a detailed guide to understand and run the code provided for solving various optimization problems using linear programming. The code makes use of Python’s NumPy, Matplotlib, and SciPy libraries to solve and visualize these problems.

Overview of the Code

The code consists of:
	1.	Imports:
	•	numpy for numerical operations.
	•	matplotlib.pyplot for graph plotting.
	•	scipy.optimize.linprog for solving linear programming problems.
	2.	Core Functions:
	•	plot_graph(A, b, c, result, problem_title): Visualizes the constraints, feasible region, and optimal solution for a given linear programming problem.
	•	solve_problem(c, A, b, bounds, title): Solves the linear programming problem using scipy.optimize.linprog and plots the result.
	3.	Optimization Problems:
	•	The code solves 10 optimization problems, such as maximizing profit, minimizing cost, and resource allocation, each defined by:
	•	c: Coefficients of the objective function.
	•	A and b: Constraints in the form ￼.
	•	bounds: Variable bounds.

Steps to Run the Code

1. Prerequisites

Make sure you have Python installed along with the required libraries. Install the dependencies with the following commands:

pip install numpy matplotlib scipy

2. File Setup

Save the code in a Python file, e.g., linear_programming.py, or run it in a Jupyter Notebook.

3. Running the Code

	•	Run the Python script or Jupyter Notebook. Each problem will:
	1.	Solve the linear programming model using linprog.
	2.	Print the result, including:
	•	Success status.
	•	Optimal values of variables.
	•	Optimal value of the objective function.
	3.	Display a graph with:
	•	Constraints as lines.
	•	Feasible region (shaded areas).
	•	Optimal solution (red dot).

Detailed Description of Functions

plot_graph(A, b, c, result, problem_title)

	•	Purpose: Visualizes the constraints and optimal solution for a linear programming problem.
	•	Parameters:
	•	A: Coefficients of constraints.
	•	b: Right-hand side values of constraints.
	•	c: Coefficients of the objective function.
	•	result: Result from linprog.
	•	problem_title: Title for the plot.
	•	Output: A plot showing:
	•	Constraints as lines.
	•	Shaded feasible region.
	•	The optimal solution as a red dot.

solve_problem(c, A, b, bounds, title)

	•	Purpose: Solves the linear programming problem and plots the result.
	•	Parameters:
	•	c: Coefficients of the objective function.
	•	A: Coefficients for constraints.
	•	b: Right-hand side values of constraints.
	•	bounds: Bounds for the variables, e.g., (0, None) for non-negative variables.
	•	title: Title for the problem.
	•	Output:
	•	Prints the result, including success status, optimal variable values, and the optimal value of the objective function.
	•	Calls plot_graph to display the graph.

Optimization Problems Solved

Problem 1: Maximizing Profit for a Factory

	•	Objective Function: Maximize ￼ (profit from two products).
	•	Constraints:
	•	￼
	•	￼
	•	Bounds: ￼.

Problem 2: Minimizing Cost for a Manufacturer

	•	Objective Function: Minimize ￼ (cost of two resources).
	•	Constraints:
	•	￼
	•	￼
	•	Bounds: ￼.

Other Problems:

The remaining problems (3-10) follow a similar structure, with different objective functions and constraints, representing scenarios such as production planning, revenue maximization, and budget allocation.

Expected Output

Console Output:

For each problem, you’ll see something like:

Maximizing Profit for a Factory Solution:
  success: True
  status: 0
  fun: -15.0
  x: [2.00, 3.00]
  message: Optimization terminated successfully.

Graphs:

	•	Constraints are displayed as lines.
	•	The feasible region is shaded.
	•	The optimal solution is marked with a red dot.

Customization

	•	Modify the coefficients c, constraints A and b, or bounds to solve your own optimization problems.
	•	Adjust the x range in plot_graph for larger or smaller feasible regions.

Troubleshooting

	•	Error: “Linprog failed to find a feasible solution”:
	•	Verify that the constraints define a feasible region.
	•	Plots not displaying:
	•	Ensure matplotlib is installed and working.
	•	For Jupyter Notebook, use %matplotlib inline before running the code.

This guide provides all the details needed to understand, run, and modify the linear programming solutions code. Let me know if you need further assistance!
