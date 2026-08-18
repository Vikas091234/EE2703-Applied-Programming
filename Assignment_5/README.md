# Assignment 5 – Laplace Equation

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment solves the two-dimensional Laplace equation to
determine the electric potential distribution in a conducting plate.

A conducting plate contains a circular electrode maintained at 1 V,
while the bottom boundary is grounded and the remaining boundaries
are electrically insulated.

The potential distribution is obtained numerically using an iterative
finite-difference method.

## Learning Outcomes

After completing this assignment, I learned to:

- Formulate the two-dimensional Laplace equation
- Convert a differential equation into a finite-difference equation
- Solve a numerical partial differential equation iteratively
- Apply Dirichlet and Neumann boundary conditions
- Use NumPy array slicing for vectorized computation
- Analyse numerical convergence
- Plot potential distributions using contour and surface plots
- Calculate current density from the potential gradient
- Visualize vector fields using quiver plots
- Use command-line arguments in Python

## Files

| File | Description |
|------|-------------|
| `code.py` | Main Python program for solving the Laplace equation. |
| `Assignment_5_Question.pdf` | Original assignment specification. |
| `plots/` | Generated plots showing potential and convergence results. |

## Mathematical Background

For a conducting material with constant conductivity under DC
conditions, the potential satisfies Laplace's equation:

```text
∇²φ = 0