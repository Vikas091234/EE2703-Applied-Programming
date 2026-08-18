# Assignment 7 – Active Filter Analysis

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment analyses active low-pass and high-pass filters using
Laplace transforms, symbolic algebra, and numerical simulation.

The circuit equations are formulated using SymPy and solved
symbolically to obtain the transfer functions. The resulting systems
are then analysed using SciPy's LTI system tools.

## Learning Outcomes

After completing this assignment, I learned to:

- Formulate circuit equations in the Laplace domain
- Use SymPy for symbolic algebra
- Represent circuit equations using matrices
- Solve symbolic matrix equations
- Convert symbolic transfer functions into numerical LTI systems
- Generate Bode plots
- Calculate step responses
- Simulate LTI systems using `scipy.signal.lsim`
- Analyse low-pass and high-pass filter behaviour
- Study the response to sinusoidal and damped sinusoidal inputs

## Files

| File | Description |
|------|-------------|
| `code.py` | Python implementation of the filter analysis. |
| `Assignment_7_Question.pdf` | Original assignment specification. |
| `plots/` | Generated plots for the different questions. |

## Circuits

The assignment analyses two active filters:

### Low-Pass Filter

The first circuit is a second-order active low-pass filter.

The component values used are:

```text
R1 = 10 kΩ
R2 = 10 kΩ
C1 = 1 nF
C2 = 1 nF
G  = 1.586