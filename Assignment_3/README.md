# Assignment 3 – Fitting Data to Models

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment studies least-squares fitting of noisy data and
investigates how noise affects the accuracy of the estimated model
parameters.

The given data is generated from the model

f(t) = 1.05 J₂(t) - 0.105t

with different levels of normally distributed noise. The noisy data is
then fitted using a model of the form

g(t, A, B) = A J₂(t) + Bt

to estimate the unknown parameters A and B.

## Learning Outcomes

After completing this assignment, I learned to:

- Read and parse numerical data from a file
- Work with NumPy arrays
- Generate and analyse noisy data
- Use Bessel functions with SciPy
- Construct matrices for linear parameter estimation
- Perform least-squares fitting using `scipy.linalg.lstsq`
- Calculate mean squared error
- Generate contour plots
- Analyse the effect of noise on parameter estimation
- Use logarithmic plots to study relationships between variables

## Files

| File | Description |
|------|-------------|
| `code.py` | Main Python program implementing the data fitting and analysis. |
| `generateData.py` | Generates the noisy data and stores it in `fitting.dat`. |
| `fitting.dat` | Input data containing the time values and noisy measurements. |
| `Assignment_3_Question.pdf` | Original assignment specification. |
| `Expected_Plots.pdf` | Reference plots provided with the assignment. |
| `Vikas_Raj_EE19B108_Assignment_3_Report.pdf` | Assignment report. |
| `Vikas_Raj_EE19B108_Assignment_3_Report.tex` | LaTeX source used to generate the report. |
| `plots/` | Generated plots used in the report. |

## Method

The assignment follows these main steps:

1. Generate data using the known function

   ```text
   f(t) = 1.05 J₂(t) - 0.105t