# EE2703 Applied Programming Lab — Coursework Report

## 1. Overview

This repository contains ten computational assignments completed for **EE2703 – Applied Programming Lab at IIT Madras**.

The assignments form a progression from basic Python file processing and SPICE netlist parsing to numerical engineering computation, continuous-time systems, Fourier analysis, and digital signal processing.

The work demonstrates the use of Python as an engineering-computation environment rather than only as a programming language.

---

# 2. Assignment Summary

| # | Assignment | Primary topic | Main techniques |
|---:|---|---|---|
| 1 | Introduction to Python | SPICE netlist parsing | File parsing, strings, lists, CLI |
| 2 | SPICE Part 2 | Circuit solver | OOP, MNA, complex arithmetic, NumPy |
| 3 | Fitting Data to Models | Parameter estimation | Bessel functions, least squares, noise |
| 4 | Fourier Approximations | Fourier series | Integration, least squares, reconstruction |
| 5 | Laplace Equation | Numerical PDE | Finite differences, boundary conditions |
| 6 | Laplace Transform | LTI systems | Transfer functions, simulation, frequency response |
| 7 | Active Filter Analysis | Filter modelling | SymPy, symbolic matrices, LTI analysis |
| 8 | Digital Fourier Transform | FFT | DFT/IFFT, spectra, modulation |
| 9 | DFT and Spectral Analysis | Practical spectral analysis | Leakage, windows, estimation, chirps, STFT |
| 10 | FIR & Discrete-Time DSP | Digital filtering | FIR, convolution, FFT convolution, correlation |

---

# 3. Assignment 1 — Introduction to Python

The first assignment introduces Python through SPICE netlist processing.

The program reads a netlist supplied through the command line and identifies the circuit description between:

```text
.circuit
.end
```

It then processes and prints the circuit elements in reverse order.

### Concepts demonstrated

- file handling;
- command-line arguments;
- string processing;
- list manipulation;
- conditional logic;
- basic error handling;
- structured text parsing.

### Repository contents

```text
Assignment_1/
├── Assignment 1 - Question.pdf
├── ckt1.netlist
├── ckt2.netlist
├── ckt3.netlist
├── code.py
└── README.md
```

---

# 4. Assignment 2 — SPICE Part 2

Assignment 2 extends the parser into a circuit-analysis program.

The implementation represents components using Python classes and constructs the equations required for circuit analysis.

The main workflow is:

```text
SPICE netlist
      ↓
Parse components
      ↓
Create circuit objects
      ↓
Identify nodes
      ↓
Construct MNA matrix
      ↓
Solve Mx = b
      ↓
Node voltages / source currents
```

The implementation supports passive elements, independent sources, and dependent sources.

### Main concepts

- object-oriented programming;
- SPICE netlists;
- engineering-unit parsing;
- node indexing;
- complex arithmetic;
- Modified Nodal Analysis;
- numerical linear algebra.

Eight circuit netlists are included for testing.

---

# 5. Assignment 3 — Fitting Data to Models

Assignment 3 studies parameter estimation from noisy data.

The known model is:

```text
f(t) = 1.05 J₂(t) - 0.105t
```

and the fitting model is:

```text
g(t, A, B) = A J₂(t) + Bt
```

The assignment investigates how noise affects the estimated parameters.

### Methods

- Bessel functions from SciPy;
- matrix-based least-squares fitting;
- mean-squared error;
- noisy-data generation;
- contour plots;
- logarithmic analysis.

The generated data is stored in:

```text
fitting.dat
```

and produced using:

```text
generateData.py
```

---

# 6. Assignment 4 — Fourier Approximations

Assignment 4 investigates Fourier-series representations of:

```text
e^x
```

and:

```text
cos(cos(x))
```

Two approaches are compared:

1. direct numerical integration of Fourier coefficients;
2. least-squares estimation of Fourier coefficients.

The calculated coefficients are then used to reconstruct the functions.

### Concepts

- Fourier-series coefficients;
- numerical integration;
- least-squares approximation;
- convergence;
- reconstruction error;
- Gibbs phenomenon;
- semilog/log-log visualization.

---

# 7. Assignment 5 — Laplace Equation

Assignment 5 solves a two-dimensional Laplace equation numerically for an electrically conducting plate.

The problem contains:

- a circular electrode at 1 V;
- a grounded lower boundary;
- insulated remaining boundaries.

The finite-difference discretization converts the continuous PDE into an iterative numerical problem.

### Analysis performed

- convergence with iteration count;
- potential distribution;
- contour plots;
- surface plots;
- electric-field/current-density calculation;
- vector-field visualization.

The program also exposes numerical parameters through command-line arguments.

This assignment demonstrates the transition:

```text
Physical problem
      ↓
Differential equation
      ↓
Finite-difference discretization
      ↓
Iterative numerical solver
      ↓
Engineering visualization
```

---

# 8. Assignment 6 — Laplace Transform and LTI Systems

Assignment 6 studies continuous-time LTI systems through transfer functions.

The supplied implementation covers mechanical systems and an RLC network.

The analysis includes:

- transfer-function construction;
- impulse response;
- system response to input signals;
- frequency response;
- Bode plots;
- transient behaviour;
- long-term response.

The implementation uses SciPy signal-processing tools for numerical system simulation.

---

# 9. Assignment 7 — Active Filters

Assignment 7 analyses second-order active low-pass and high-pass filters.

The circuit equations are constructed using symbolic matrices and solved using SymPy.

The symbolic transfer function is subsequently converted into a numerical LTI representation for simulation.

### Analyses include

- low-pass Bode response;
- high-pass Bode response;
- input/output sinusoidal response;
- damped sinusoidal response;
- step response.

The actual source filename is:

```text
Assignment_7/code_.py
```

This is an important repository-specific detail and is intentionally preserved.

---

# 10. Assignment 8 — Digital Fourier Transform

Assignment 8 introduces FFT-based computation of the DFT.

The implementation first verifies FFT/IFFT reconstruction using a random sequence.

It then analyses:

- `sin(5t)`;
- amplitude modulation;
- `sin³(t)`;
- `cos³(t)`;
- `cos(20t + 5cos(t))`;
- a Gaussian signal.

For the Gaussian, the numerical FFT result is compared against the analytical Fourier transform.

### Concepts

- FFT;
- inverse FFT;
- magnitude spectrum;
- phase spectrum;
- `fftshift`;
- sampling;
- modulation sidebands;
- analytical versus numerical spectrum.

---

# 11. Assignment 9 — DFT and Spectral Analysis

Assignment 9 moves from basic FFT computation to practical spectral analysis.

The assignment studies:

### Spectral leakage

A non-integer number of cycles within the observation interval causes energy to spread across nearby frequency bins.

### Windowing

A Hamming window is implemented to reduce spectral leakage.

### Frequency and phase estimation

The code estimates the frequency and phase of:

```text
cos(ω₀t + δ)
```

using the weighted spectrum and least-squares fitting.

The same estimation is tested with additive noise.

### Chirp analysis

The implementation analyses a chirp whose instantaneous frequency changes with time.

### STFT

The signal is divided into batches and an FFT is computed for each batch, producing a time-frequency representation.

This is one of the more technically substantial assignments because it connects a static DFT with time-varying spectral analysis.

---

# 12. Assignment 10 — FIR and Discrete-Time DSP

Assignment 10 studies FIR filtering and discrete-time operations.

The filter impulse response is loaded from:

```text
h.csv
```

The program computes its frequency response and applies it to:

```text
x[n] = cos(0.2πn) + cos(0.85πn)
```

### Operations performed

#### FIR response

The supplied impulse response is plotted and its frequency response is calculated using `scipy.signal.freqz`.

#### Linear convolution

The output is computed using direct convolution:

```text
y[n] = x[n] * h[n]
```

#### Circular convolution

FFT multiplication is used to compute circular convolution.

#### FFT-based linear convolution

Zero-padding is used so that FFT multiplication reproduces linear convolution.

#### Zadoff–Chu sequence correlation

The sequence stored in:

```text
x1.csv
```

is read as complex samples, shifted, and correlated with the original sequence.

This assignment therefore connects FIR filtering, frequency-domain processing, convolution theory, and sequence correlation.

---

# 13. Technical Progression

The assignments form a useful progression in engineering computation:

```text
Python fundamentals
        ↓
SPICE netlist parsing
        ↓
Circuit modelling + MNA
        ↓
Numerical parameter estimation
        ↓
Fourier-series computation
        ↓
Numerical PDE solution
        ↓
Continuous-time LTI systems
        ↓
Symbolic filter analysis
        ↓
DFT / FFT
        ↓
Spectral analysis + STFT
        ↓
FIR filtering + FFT convolution
```

This progression is more representative of the repository than treating the ten assignments as unrelated exercises.

---

# 14. Tools and Libraries

The coursework primarily uses:

```text
Python
NumPy
SciPy
SymPy
Matplotlib
```

Additional modules used across the assignments include:

- `numpy.fft`
- `scipy.fftpack`
- `scipy.signal`
- `scipy.linalg`
- `mpl_toolkits.mplot3d`

---

# 15. Skills Demonstrated

## Programming

- Python scripting;
- modular function design;
- command-line interfaces;
- file parsing;
- numerical data processing;
- object-oriented programming.

## Circuit and systems

- SPICE netlist processing;
- Modified Nodal Analysis;
- linear-system solution;
- symbolic circuit equations;
- transfer functions;
- active-filter analysis.

## Numerical methods

- least-squares estimation;
- numerical integration;
- finite-difference discretization;
- iterative PDE solution;
- numerical error analysis.

## Signal processing

- Fourier series;
- DFT/FFT;
- FFT/IFFT;
- frequency and phase estimation;
- windowing;
- spectral leakage;
- STFT;
- FIR filtering;
- convolution;
- correlation.

---



## Author

**Vikas Raj**  
IIT Madras  
EE2703 – Applied Programming Lab
