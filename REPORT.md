# EE2703 Applied Programming Lab — Portfolio Report

## Overview

This repository contains ten computational assignments from EE2703 – Applied Programming Lab. The work progresses from basic Python file processing to circuit simulation, numerical methods, Fourier analysis, continuous-time systems, and digital signal processing.

## Assignment Summary

| Assignment | Topic | Main Techniques |
|---|---|---|
| 01 | SPICE Netlist Parser | File parsing, strings, CLI arguments |
| 02 | SPICE Circuit Solver | OOP, complex arithmetic, Modified Nodal Analysis, NumPy linear algebra |
| 03 | Data Fitting | Bessel functions, least squares, noise analysis, SciPy |
| 04 | Fourier Approximations | Numerical integration, Fourier coefficients, least squares, Gibbs phenomenon |
| 05 | Laplace Equation | Finite differences, boundary conditions, iterative numerical solution |
| 06 | Laplace Transform & LTI Systems | Transfer functions, impulse/forced response, frequency response |
| 07 | Active Filters | SymPy symbolic algebra, transfer functions, Bode/step/LSIM analysis |
| 08 | Digital Fourier Transform | FFT/IFFT, spectra, phase, sampling and modulation |
| 09 | Spectral Analysis | Leakage, Hamming window, frequency/phase estimation, chirps, STFT |
| 10 | FIR & Discrete-Time DSP | FIR response, linear/circular convolution, FFT convolution, correlation |

## Technical Highlights

### 1. SPICE Parsing and Circuit Solving

The first two assignments build a small SPICE-oriented analysis workflow. The parser identifies `.circuit` and `.end` sections and converts circuit descriptions into structured data. The second assignment extends this into an object-oriented circuit model and solves the resulting matrix equations using numerical linear algebra.

The important engineering concept demonstrated here is **Modified Nodal Analysis (MNA)**: circuit laws are converted into a linear system of equations and solved numerically.

### 2. Numerical Modelling

Assignments 3–5 apply computational methods to engineering problems:

- noisy-data parameter estimation,
- Fourier-series approximation,
- finite-difference solution of a two-dimensional Laplace equation.

These assignments demonstrate the ability to move from a mathematical model to a numerical algorithm and then validate/interprete the result through plots.

### 3. Continuous-Time Systems and Filters

Assignments 6 and 7 use Laplace-domain representations to analyse LTI systems and active filters. Symbolic equations are converted into numerical transfer functions, after which impulse, step, sinusoidal and frequency-domain responses are studied.

### 4. Digital Signal Processing

Assignments 8–10 focus on the frequency-domain view of signals and practical DSP operations:

- DFT and FFT,
- frequency and phase spectra,
- sampling effects,
- modulation sidebands,
- spectral leakage,
- windowing,
- frequency estimation,
- chirp analysis,
- STFT,
- FIR filtering,
- linear and circular convolution,
- FFT-based convolution,
- sequence correlation.

## Tools and Libraries

The implementations primarily use:

- Python
- NumPy
- SciPy
- SymPy
- Matplotlib

## Portfolio Value

The strongest resume-relevant aspects of this repository are not the fact that these are course assignments, but the technical methods implemented:

1. **Circuit computation:** parsing structured netlists and solving circuit equations numerically.
2. **Numerical methods:** translating differential equations into finite-difference algorithms.
3. **Scientific computing:** least-squares estimation, numerical integration and matrix-based computation.
4. **Signal processing:** FFT-based spectral analysis, windowing, STFT and FIR filtering.
5. **Engineering visualization:** generating plots to inspect convergence, frequency response and numerical results.

## Recommended Resume Framing

Instead of listing all ten assignments individually, present the repository as one technical project:

> **Engineering Computing & Signal Processing — Python**  
> Implemented numerical and signal-processing algorithms in Python covering SPICE netlist parsing and circuit solving, least-squares estimation, Fourier analysis, finite-difference PDE solving, LTI/filter analysis, FFT-based spectral analysis, STFT, FIR filtering, convolution and correlation.

Then link to this repository as supporting evidence.

## Author

Vikas Raj — IIT Madras
