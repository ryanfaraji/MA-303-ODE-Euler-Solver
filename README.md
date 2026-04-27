# MA-303-ODE-Euler-Solver

Python program for approximating first-order differential equations using Euler's method, with exact solution and error comparison.

## Objective

The purpose of this project is to create a Python program that approximates the solution of a first-order differential equation with an initial condition using Euler's method. When an exact solution is known, the program also compares the numerical approximation to the exact solution and shows the error and cumulative error.

## Mathematics Behind the Project
<img width="239" height="192" alt="image" src="https://github.com/user-attachments/assets/3aa1c03f-d176-419d-a492-021611e19db6" />

This project is based on an initial value problem:

dy/dx = f(x, y), with initial condition y(x0) = y0

Euler's method estimates the next value by using the slope at the current point:

y(n+1) = y(n) + h f(x(n), y(n))

where h is the step size.

This means the program starts at the initial point and moves forward one step at a time, using the derivative to estimate the next y-value.

## What the Program Does

The program allows the user to:
- enter a differential equation of the form dy/dx = f(x, y)
- enter an initial condition
- enter a step size and interval
- compute approximate values using Euler's method
- compare the approximation to an exact solution when one is known
- compute absolute error and cumulative error
- display a graph of the approximation and exact solution

## Example Used in the Project

One example used in the project is:

dy/dx = y
y(0) = 1

The exact solution is:

y = e^x

This example is useful because the exact solution is known, so the approximation can be compared directly to the true solution.

## Results

The results show that Euler's method follows the general shape of the exact solution, but it is not exact. As the program moves farther from the initial condition, the error grows. This helps show that Euler's method is an approximation and that step size affects accuracy.

## Files Included

- main.py — the Python program
- README.md — the project report and overview
- requirements.txt — required Python packages

## How to Run the Program

1. Install the required packages:

pip install -r requirements.txt

2. Run the program:

python main.py

3. Choose either the built-in demo or enter your own problem.

## Conclusion

This project demonstrates how Euler's method can be used to approximate solutions of differential equations when an exact solution may be difficult to find. It also shows how numerical error builds over time and why step size matters.
