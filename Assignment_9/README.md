# Assignment 9 – DFT and Spectral Analysis

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment studies practical aspects of the Discrete Fourier
Transform (DFT), including spectral leakage, windowing, frequency
estimation, phase estimation, noise, chirp signals, and the
Short-Time Fourier Transform (STFT).

The assignment uses FFT-based computation to analyse signals in both
the frequency and time-frequency domains.

## Learning Outcomes

After completing this assignment, I learned to:

- Analyse signals using the DFT
- Understand spectral leakage
- Apply a Hamming window before computing the DFT
- Estimate signal frequency from its spectrum
- Estimate phase using least-squares fitting
- Perform frequency and phase estimation in the presence of noise
- Analyse chirp signals
- Understand how frequency changes with time
- Implement a Short-Time Fourier Transform
- Visualize time-frequency information using 3D plots

## Files

| File | Description |
|------|-------------|
| `code.py` | Python implementation of all assignment problems. |
| `Assignment_9_Question.pdf` | Original assignment specification. |
| `plots/` | Generated DFT, spectrum, and STFT plots. |

## Problems Covered

### 1. Spectrum of sin(√2 t)

The spectrum of:

```text
sin(√2 t)