# EE2703 Applied Programming Lab

A structured collection of programming and computational assignments completed for **EE2703 – Applied Programming Lab at IIT Madras**.

The repository covers Python programming, SPICE circuit analysis, numerical methods, Fourier analysis, Laplace-domain LTI systems, filter analysis, digital signal processing, and FIR filtering.

## Skills Demonstrated

- Python programming and modular function design
- NumPy, SciPy, SymPy and Matplotlib
- File parsing and command-line interfaces
- Object-oriented modelling of circuit components
- Modified nodal analysis and linear-system solution
- Least-squares parameter estimation
- Numerical integration and Fourier-series approximation
- Finite-difference solution of Laplace's equation
- Laplace transforms and continuous-time LTI systems
- Symbolic circuit analysis
- DFT/FFT and spectral analysis
- Windowing, spectral leakage and STFT
- FIR filtering, convolution and correlation
- Technical plotting and numerical interpretation

## Repository Structure

```text
ee2703-applied-programming/
├── assignments/
│   ├── assignment-01/   # SPICE netlist parser
│   ├── assignment-02/   # SPICE circuit solver / MNA
│   ├── assignment-03/   # Least-squares fitting
│   ├── assignment-04/   # Fourier-series approximation
│   ├── assignment-05/   # Numerical Laplace-equation solver
│   ├── assignment-06/   # Laplace-transform and LTI analysis
│   ├── assignment-07/   # Active filter analysis
│   ├── assignment-08/   # DFT / FFT
│   ├── assignment-09/   # Spectral analysis and STFT
│   └── assignment-10/   # FIR filters and discrete-time DSP
├── REPORT.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

## Running the Assignments

Create a virtual environment and install the dependencies:

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux/macOS
source .venv/bin/activate

pip install -r requirements.txt
```

Each assignment is self-contained. Run the relevant Python file from its assignment directory so that relative input/data and `plots/` paths work correctly.

Example:

```bash
cd assignments/assignment-01
python code.py ckt1.netlist
```

For Assignment 5:

```bash
cd assignments/assignment-05
python code.py --Nx 50 --Ny 50 --radius 0.35 --Niter 4000
```

## Notes

- Generated plots are retained because they demonstrate the numerical results and signal-analysis work.
- Course question sheets are intentionally not included in this public-facing repository; the repository focuses on the implementation and results.
- The code reflects coursework implementations and is organized for portfolio/review purposes rather than as a production software package.

## Author

**Vikas Raj**  
IIT Madras  
EE2703 – Applied Programming Lab
