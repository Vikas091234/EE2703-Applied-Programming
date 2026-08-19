# EE2703 — Applied Programming Lab

A collection of ten computational assignments completed for **EE2703 – Applied Programming Lab at IIT Madras**.

The repository progresses from basic Python and SPICE netlist processing to circuit simulation, numerical methods, Fourier analysis, continuous-time LTI systems, active filters, and digital signal processing.

## Repository structure

```text
.
├── README.md
├── REPORT.md
│
├── Assignment_1/
│   ├── Assignment 1 - Question.pdf
│   ├── ckt1.netlist
│   ├── ckt2.netlist
│   ├── ckt3.netlist
│   ├── code.py
│   └── README.md
│
├── Assignment_2/
│   ├── 3.0.1.py
│   ├── 4.2.1.py
│   ├── Assignment 2 - Question.pdf
│   ├── ckt1.netlist
│   ├── ckt2.netlist
│   ├── ckt3.netlist
│   ├── ckt4.netlist
│   ├── ckt5.netlist
│   ├── ckt6.netlist
│   ├── ckt7.netlist
│   ├── ckt8.netlist
│   ├── code.py
│   └── README.md
│
├── Assignment_3/
│   ├── plots/
│   │   ├── Fig 0.png
│   │   ├── Fig 1.png
│   │   ├── Fig 2.png
│   │   ├── Fig 3.png
│   │   └── Fig 4.png
│   ├── Assignment 3 - Question.pdf
│   ├── code.py
│   ├── fitting.dat
│   ├── generateData.py
│   ├── README.md
│   └── Report.pdf
│
├── Assignment_4/
│   ├── plots/
│   │   ├── Figure 1.png
│   │   ├── Figure 2.png
│   │   ├── Figure 3.1.png
│   │   ├── Figure 3.png
│   │   ├── Figure 4.1.png
│   │   ├── Figure 4.png
│   │   ├── Figure 5.1.png
│   │   ├── Figure 5.png
│   │   ├── Figure 6.1.png
│   │   ├── Figure 6.png
│   │   ├── Figure 7.png
│   │   └── Figure 8.png
│   ├── Assignment 4 - Question.pdf
│   ├── code.py
│   ├── README.md
│   └── report.pdf
│
├── Assignment_5/
│   ├── plots/
│   │   ├── Fig1.png
│   │   ├── Fig2.png
│   │   ├── Fig3.png
│   │   ├── Fig4.png
│   │   ├── Fig5.png
│   │   ├── Fig6.png
│   │   └── Fig7.png
│   ├── Assignment 5 - Question.pdf
│   ├── code.py
│   ├── README.md
│   └── report.pdf
│
├── Assignment_6/
│   ├── plots/
│   │   ├── Fig 1.png
│   │   ├── Fig 2.png
│   │   ├── Fig 3.png
│   │   ├── Fig 4.png
│   │   ├── Fig 5(a).png
│   │   ├── Fig 5(b).png
│   │   ├── Fig 6(a).png
│   │   ├── Fig 6(b).png
│   │   └── Fig 6(c).png
│   ├── Assignment 6 - Question.pdf
│   ├── code.py
│   ├── README.md
│   └── report.pdf
│
├── Assignment_7/
│   ├── plots/
│   │   ├── Fig 1.png
│   │   ├── Fig 2.png
│   │   ├── Fig 3.png
│   │   ├── Fig 4.png
│   │   ├── Fig 5.png
│   │   ├── Fig 6.png
│   │   ├── Fig 7.png
│   │   ├── Fig 8.png
│   │   ├── Fig 9.png
│   │   └── Fig 10.png
│   ├── Assignment 7 - Question.pdf
│   ├── code_.py
│   ├── README.md
│   └── report.pdf
│
├── Assignment_8/
│   ├── plots/
│   │   ├── Fig0.png
│   │   ├── Fig1.png
│   │   ├── Fig2.png
│   │   ├── Fig3.png
│   │   ├── Fig4.png
│   │   ├── Fig5.png
│   │   └── Fig6.png
│   ├── Assignment 8 - Question.pdf
│   ├── code.py
│   ├── README.md
│   └── report.pdf
│
├── Assignment_9/
│   ├── plots/
│   │   ├── Fig0.png
│   │   ├── Fig1.png
│   │   ├── Fig2.png
│   │   ├── Fig3.png
│   │   ├── Fig6.png
│   │   ├── Fig7.png
│   │   ├── Fig8.png
│   │   ├── Fig9.png
│   │   ├── Fig10.png
│   │   ├── Fig11.png
│   │   ├── Figure_10.png
│   │   └── Figure_11.png
│   ├── Assignment 9 - Question.pdf
│   ├── code.py
│   ├── README.md
│   └── report.pdf
│
└── Assignment_10/
    ├── plots/
    │   ├── Fig0.png
    │   ├── Fig1.png
    │   ├── Fig2.png
    │   ├── Fig3.png
    │   ├── Fig4.png
    │   ├── Fig5.png
    │   ├── Fig6.png
    │   ├── Fig7.png
    │   └── Fig8.png
    ├── Assignment 10 - Question.pdf
    ├── code.py
    ├── h.csv
    ├── report.aux
    ├── report.pdf
    └── x1.csv
```

> `.git/` is intentionally omitted from the documentation tree because it is repository metadata rather than coursework content.

---

# Assignment overview

| Assignment | Topic | Main work |
|---|---|---|
| 1 | Introduction to Python / SPICE parsing | Netlist parsing, file handling, CLI arguments |
| 2 | SPICE Part 2 | Circuit modelling, MNA, linear-system solution |
| 3 | Fitting Data to Models | Least-squares fitting, Bessel functions, noise analysis |
| 4 | Fourier Approximations | Fourier coefficients, integration, least squares |
| 5 | Laplace Equation | Finite differences, boundary conditions, iterative solution |
| 6 | Laplace Transform | LTI transfer functions, impulse/forced response, frequency response |
| 7 | Active Filter Analysis | Symbolic circuit equations, low/high-pass filter analysis |
| 8 | Digital Fourier Transform | FFT/IFFT, spectra, phase, modulation, Gaussian spectrum |
| 9 | DFT and Spectral Analysis | Leakage, windowing, estimation, chirps, STFT |
| 10 | FIR and Discrete-Time DSP | FIR response, convolution, FFT convolution, correlation |

---

## Assignment 1 — Introduction to Python

Assignment 1 introduces Python programming through processing of SPICE netlist files.

The program:

1. accepts a netlist filename from the command line;
2. locates the `.circuit` and `.end` markers;
3. extracts the circuit section;
4. processes the circuit-element lines;
5. prints the elements in reverse order.

### Files

- `code.py` — implementation
- `ckt1.netlist`, `ckt2.netlist`, `ckt3.netlist` — sample inputs
- `Assignment 1 - Question.pdf` — assignment statement
- `README.md` — assignment documentation

---

## Assignment 2 — SPICE Part 2

Assignment 2 extends the SPICE work into an object-oriented circuit solver.

The implementation models circuit components, parses SPICE values, identifies circuit nodes, constructs the matrix equations, and solves them numerically.

The documented implementation supports:

- resistors
- capacitors
- inductors
- independent voltage sources
- independent current sources
- VCVS
- VCCS
- CCVS
- CCCS

The main numerical method is **Modified Nodal Analysis (MNA)** followed by a linear-system solve.

### Files

- `code.py` and `code(1).py`-style supporting material represented by the supplied files
- `3.0.1.py`
- `4.2.1.py`
- eight SPICE netlists
- assignment statement
- README

The actual repository currently contains `code.py`, not a file named `code(1).py`; the tree above therefore uses the actual filename.

---

## Assignment 3 — Fitting Data to Models

Assignment 3 studies least-squares fitting of noisy data.

The supplied model is:

```text
f(t) = 1.05 J₂(t) - 0.105t
```

and the fitting model is:

```text
g(t, A, B) = A J₂(t) + Bt
```

The assignment investigates parameter estimation under different noise levels.

### Main techniques

- NumPy arrays
- SciPy Bessel functions
- least-squares fitting
- mean-squared error
- contour plots
- logarithmic plots
- noisy-data analysis

`generateData.py` creates the fitting data stored in `fitting.dat`.

---

## Assignment 4 — Fourier Approximations

Assignment 4 computes Fourier-series approximations of:

```text
e^x
```

and

```text
cos(cos(x))
```

Fourier coefficients are obtained using:

- direct numerical integration;
- least-squares estimation.

The resulting coefficients are compared and used to reconstruct the functions.

The generated plots document coefficient convergence, reconstruction, and the Gibbs phenomenon.

---

## Assignment 5 — Laplace Equation

Assignment 5 numerically solves the two-dimensional Laplace equation for the electric potential in a conducting plate.

The problem contains:

- a circular electrode maintained at 1 V;
- a grounded bottom boundary;
- insulated remaining boundaries.

The implementation uses an iterative finite-difference method.

The analysis includes:

- convergence behaviour;
- potential contour/surface plots;
- electric field/current-density calculations;
- vector-field visualization.

The program accepts numerical parameters through command-line arguments, including grid dimensions, electrode radius, and iteration count.

---

## Assignment 6 — Laplace Transform

Assignment 6 studies continuous-time LTI systems using Laplace-domain representations.

The supplied work includes mechanical-system analysis and an RLC-network analysis.

Techniques include:

- transfer functions;
- impulse responses;
- forced responses;
- system simulation;
- frequency-response analysis;
- Bode plots;
- transient and long-term behaviour.

---

## Assignment 7 — Active Filter Analysis

Assignment 7 analyses second-order active low-pass and high-pass filters.

The circuit equations are formulated and solved symbolically using **SymPy**, then converted into numerical LTI representations for simulation using SciPy.

The implementation produces:

- Bode plots;
- input/output responses;
- step responses;
- responses to sinusoidal inputs;
- responses to damped sinusoidal inputs.

### Important filename detail

The actual implementation file in this repository is:

```text
Assignment_7/code_.py
```

not `code.py`.

The documentation tree intentionally preserves this exact filename.

---

## Assignment 8 — Digital Fourier Transform

Assignment 8 uses FFT-based computation to study discrete Fourier transforms and spectra.

The implementation includes:

- FFT followed by IFFT reconstruction;
- spectrum of `sin(5t)`;
- amplitude modulation;
- spectra of `sin³(t)` and `cos³(t)`;
- spectrum of `cos(20t + 5cos(t))`;
- numerical versus analytical Gaussian spectrum.

The program also calculates numerical errors for the random-sequence reconstruction and Gaussian-spectrum comparison.

---

## Assignment 9 — DFT and Spectral Analysis

Assignment 9 investigates practical spectral-analysis problems.

The implementation covers:

- spectral leakage;
- Hamming-windowing;
- frequency estimation;
- phase estimation;
- noisy sinusoidal signals;
- chirp signals;
- Short-Time Fourier Transform (STFT).

The code includes reusable functions for:

```text
hammingWindow()
plotSignal()
plotSpectrum()
estimateWandD()
STFT()
plot3DSTFT()
```

The chirp analysis is extended from a full-signal DFT to a time-evolving STFT representation.

---

## Assignment 10 — FIR and Discrete-Time Signal Processing

Assignment 10 analyses a supplied FIR filter and performs several discrete-time signal-processing operations.

The implementation:

1. reads the FIR impulse response from `h.csv`;
2. plots the impulse response;
3. computes its frequency response;
4. constructs
   ```text
   x[n] = cos(0.2πn) + cos(0.85πn)
   ```
5. computes linear convolution;
6. computes circular convolution using FFT;
7. computes FFT-based convolution with zero padding;
8. reads a Zadoff–Chu sequence from `x1.csv`;
9. studies correlation after a shift.

The assignment therefore covers both direct and FFT-based convolution as well as sequence correlation.

---

# Tools and libraries

The coursework primarily uses:

- Python
- NumPy
- SciPy
- SymPy
- Matplotlib

Specific tasks also use:

- `numpy.fft`
- `scipy.fftpack`
- `scipy.signal`
- `scipy.linalg`
- `mpl_toolkits.mplot3d`

---

# What this repository demonstrates

## Scientific computing

- numerical linear algebra
- least-squares estimation
- numerical integration
- finite-difference methods
- iterative numerical solutions

## Circuit analysis

- SPICE netlist parsing
- circuit component modelling
- Modified Nodal Analysis
- DC/AC circuit analysis
- symbolic filter analysis

## Signals and systems

- Fourier series
- DFT/FFT
- frequency and phase spectra
- sampling effects
- modulation
- spectral leakage
- windowing
- frequency/phase estimation
- chirp analysis
- STFT

## Digital signal processing

- FIR filtering
- frequency response
- linear convolution
- circular convolution
- FFT-based convolution
- correlation
- Zadoff–Chu sequence analysis

---

## Author

**Vikas Raj**  
IIT Madras  
EE2703 – Applied Programming Lab
