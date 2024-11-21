# Time Series Analysis of GJ 3942

Examining the rotation of the planet-hosting M dwarf GJ 3942.

## Description

Based on radial velocities, EXORAP photometry, and activity indicators, the HADES team reported a 16.3-day rotation period for the M dwarf GJ 3942. We re-analyze HADES data, as well as data from TESS (Transiting Exoplanet Survey Satellite), SuperWASP (Wide Angle Search for Planets), and the Hipparcos satellite. This analysis was conducted through computational notebooks. These computational notebooks can be found in this repository. The notebooks GJ3942_time_series_analysis_SuperWASP.ipynb and GJ3942_time_series_analysis_Hipparcos.ipynb are used in the extended version published on arXiv [here](https://arxiv.org/abs/2411.05476).

With these notebooks, we find an estimate of the magnitude-squared coherence between the HADES RV and Hα time series has significant peaks at frequencies 1/16 cycles/day and 1/32 cycles/day. We turn to TESS photometry to test the hypothesis that the true rotation period is 32 days with 16-day harmonic, as well as using SuperWASP and Hipparcos data to consolidate this hypothesis. The TESS observations suggest a 1/16 cycles/day rotation frequency and a 1/32 cycles/day subharmonic, though resolution makes the TESS rotation detection ambiguous, with SuperWASP and Hipparcos detections unable to break the degeneracy between the 16- and 32-day possible rotation periods.

For the computational notebooks, each have corresponding data files. The sources for these data files can be found at the end of their corresponding notebooks.
 - The notebook GJ3942_coherence_final.ipynb uses the data file GJ3942_HARPSN_Perger17.txt
 - The notebook GJ3942_time_series_analysis_SuperWASP.ipynb uses the data file GJ3942_1SWASP_J160901.59+525637.2.tbl
 - The notebook GJ3942_time_series_analysis_Hipparcos.ipynb uses the data file GJ3942_Hipparcos_Photometric_Light_Curve.tbl.txt
 - The notebook GJ3942_time_series_analysis_TESS.ipynb uses the data files within the MAST_files folder

List of files within MAST_files:
 - tess2020078014623-s0023-0000000162494287-0177-s_lc.fits
 - tess2022085151738-s0050-0000000162494287-0222-a_fast-lc.fits
 - tess2022085151738-s0050-0000000162494287-0222-s_lc.fits
 - tess2022112184951-s0051-0000000162494287-0223-a_fast-lc.fits
 - tess2022112184951-s0051-0000000162494287-0223-s_lc.fits
 - tess2022138205153-s0052-0000000162494287-0224-a_fast-lc.fits
 - tess2022138205153-s0052-0000000162494287-0224-s_lc.fits

Recommended reading order for computational notebooks:
 - 1. GJ3942_coherence_final.ipynb
 - 2. GJ3942_time_series_analysis_TESS.ipynb
 - 3. GJ3942_time_series_analysis_SuperWASP.ipynb
 - 4. GJ3942_time_series_analysis_Hipparcos.ipynb

Packages required: numpy, matplotlib, scipy, copy, resample, finufft, NWelch

Uploaded file types: .cff, .tbl, .txt, .tbl.txt, .ipynb, .md, .fits

## Authors

Andrew Fonseca
[afonse@udel.edu]

Sarah Dodson-Robinson
[sdr@udel.edu]

---

[![DOI](https://zenodo.org/badge/830615706.svg)](https://doi.org/10.5281/zenodo.14187051)

