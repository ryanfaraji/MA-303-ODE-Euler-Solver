# MA-303-ODE-Euler-Solver
Python program for approximating first-order differential equations using Euler’s method, with exact solution and error comparison.

## Mathematics Behind the Project

We start with an initial value problem

\[
\frac{dy}{dx} = f(x,y), \quad y(x_0) = y_0
\]

Euler's Method estimates the next value using the slope at the current point:

\[
y_{n+1} = y_n + h f(x_n, y_n)
\]

where \(h\) is the step size.

## Example Test Problem

\[
y' = y,\quad y(0)=1
\]

Exact solution:

\[
y = e^x
\]

This example is useful because the exact solution is known, so the numerical error can be measured.

## Files

- `main.py` — main program
- `report.md` — short report for the project
- `requirements.txt` — required Python packages

## How to Run

Install packages:

```bash
pip install -r requirements.txt
```

Run the program:

```bash
python main.py
```

## What the Program Does

- lets the user enter a differential equation \(y' = f(x,y)\)
- applies Euler's Method
- prints a table of approximate values
- compares to the exact solution when provided
- computes cumulative error
- plots the approximation and exact solution
