# Mean, Variance, Standard Deviation Calculator

This project implements a Python function `calculate()` that computes statistical measures from a list of 9 numbers arranged as a 3x3 matrix. The function returns a dictionary containing the mean, variance, standard deviation, max, min, and sum calculated along the rows, columns, and the entire matrix.

---

## How It Works

- The input to the function is a list containing exactly **9 numbers**.
- This list is converted into a **3x3 NumPy array**.
- A helper function named `stats()` takes a NumPy statistical function (like `np.mean` or `np.var`) and computes:
  - The result **along columns** (`axis=0`) as a list.
  - The result **along rows** (`axis=1`) as a list.
  - The result on the **entire matrix (flattened)** as a single value.
- The function returns a dictionary where each key corresponds to a statistic, and its value is a list of three results: for columns, rows, and the full matrix.

---

## How to Run
Make sure you have NumPy installed:
`pip install numpy`

Use the `calculate()` function from `mean_var_std.py`.

Run tests with:
`python3 main.py`

## Why This Design?
The use of a single helper function stats() reduces code repetition by accepting different NumPy functions as parameters and performing calculations along specified axes. This design makes the code clean, maintainable, and scalable.

## Files in This Project

mean_var_std.py: Contains the calculate() function.

main.py: Script to run and test the function.

test_module.py: Unit tests for the project.

README.md: This file explaining the project.


Feel free to explore and modify the project as you like!


This is the boilerplate for the Mean-Variance-Standard Deviation Calculator project. Instructions for building your project can be found at https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-projects/mean-variance-standard-deviation-calculator
