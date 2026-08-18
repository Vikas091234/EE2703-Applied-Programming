# Assignment 8 – Digital Fourier Transform

## Course

EE2703 – Applied Programming Lab

## Objective

This assignment studies the Discrete Fourier Transform (DFT) and its
implementation using the Fast Fourier Transform (FFT).

Different signals are sampled and their frequency spectra are computed
using the FFT. The assignment also investigates frequency resolution,
phase, modulation sidebands, and the effect of the sampling window on
the spectrum of a Gaussian function.

## Learning Outcomes

After completing this assignment, I learned to:

- Understand the relationship between the Fourier Transform, DTFT and DFT
- Compute the DFT using FFT
- Recover a signal using the inverse FFT
- Interpret magnitude and phase spectra
- Use `fftshift()` to display positive and negative frequencies
- Understand the effect of sampling on frequency resolution
- Analyse sinusoidal signals in the frequency domain
- Identify modulation sidebands
- Analyse non-bandlimited signals
- Compare a numerically computed Gaussian spectrum with its theoretical
  Fourier transform

## Files

| File | Description |
|------|-------------|
| `code.py` | Python implementation of the DFT and spectrum analysis tasks. |
| `Assignment_8_Question.pdf` | Original assignment specification. |
| `plots/` | Generated magnitude and phase spectrum plots. |

## Background

For a periodic sequence with period `N`, the DFT is defined as:

```text
F[k] = Σ f[n] exp(-j2πnk/N)