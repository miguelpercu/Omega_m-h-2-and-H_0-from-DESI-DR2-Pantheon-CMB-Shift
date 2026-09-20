# Phenomenological Measurement of Omega_m h^2 and H_0

**Authors:** Miguel Ángel Percudani, Jorge Iván Díaz
**Date:** September 2026
**License:** CC BY 4.0

---

## Overview

This repository contains a reproducible MCMC analysis of the cosmological parameters (H_0, Omega_m h^2) using three independent datasets:

- **DESI DR2** baryon acoustic oscillation (BAO) measurements (13 data points, full covariance)
- **Pantheon+** Type Ia supernovae (1590 SNe with z > 0.01, full statistical + systematic covariance)
- **CMB shift parameters** (l_A and R from Planck 2018)

The analysis assumes a spatially flat LambdaCDM universe. No extended framework is assumed or tested. The goal is a phenomenological measurement of standard cosmological parameters, comparing with Planck 2018.

## Results

| Parameter | This work | Planck 2018 | Deviation |
|-----------|-----------|-------------|-----------|
| H_0 [km/s/Mpc] | 69.91 +/- 0.71 | 67.4 +/- 0.5 | +2.51 |
| Omega_m h^2 | 0.14763 +/- 0.00126 | 0.1422 +/- 0.0008 | +3.6 sigma |

Best-fit chi^2 = 1420.53 for N = 1605 data points (13 BAO + 1590 SNe + 2 CMB).
Reduced chi^2 ≈ 0.885.

**Interpretation:** The measured Omega_m h^2 is 3.8% higher than Planck at approximately 3.6 sigma. This deviation connects to the well-documented tension between early-universe probes (CMB) and late-universe probes (BAO + SNe). It is not interpreted here as evidence for any extension beyond LambdaCDM.

## Repository Contents








## Requirements

- Python 3.8+
- NumPy, SciPy
- emcee (MCMC sampler)
- corner (corner plots)
- matplotlib

Install with:

```bash
pip install numpy scipy emcee corner matplotlib













python cosmo_measurement.py





Percudani, M. A., & Díaz, J. I. (2026).
Phenomenological Measurement of Omega_m h^2 and H_0
from DESI DR2, Pantheon+, and CMB Shift Data.
Zenodo. DOI: https://doi.org/10.5281/zenodo.22853862