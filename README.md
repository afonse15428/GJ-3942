# Time Series Analysis of GJ 3942

Examining the rotation of the planet-hosting M dwarf GJ 3942.

## Description

Based on radial velocities, EXORAP photometry, and activity indicators, the HADES team reported a 16.3-day rotation period for the M dwarf GJ 3942. We re-analyze HADES data, as well as data from TESS (Transiting Exoplanet Survey Satellite), SuperWASP (Wide Angle Search for Planets), and the Hipparcos satellite. The computational notebooks used for this analysis can be found here. 

With these notebooks, we find an estimate of the magnitude-squared coherence between the HADES RV and Hα time series has significant peaks at frequencies 1/16 cycles/day and 1/32 cycles/day. We turn to TESS photometry to test the hypothesis that the true rotation period is 32 days with 16-day harmonic, as well as using SuperWASP and Hipparcos data to consolidate this hypothesis. The TESS observations suggest a 1/16 cycles/day rotation frequency and a 1/32 cycles/day subharmonic, though resolution makes the TESS rotation detection ambiguous, with SuperWASP and Hipparcos detections unable to break the degeneracy between the 16- and 32-day possible rotation periods.

For the computational notebooks, each have corresponding data files. The notebooks GJ3942_coherence_final.ipynb uses GJ3942_HARPSN_Perger17.txt, GJ3942_time_series_analysis_SuperWASP.ipynb uses GJ3942_1SWASP_J160901.59+525637.2.tbl, and GJ3942_time_series_analysis_Hipparcos.ipynb uses GJ3942_Hipparcos_Photometric_Light_Curve.tbl.txt. The source of these data files can be found at the end of their corresponding notebooks.

The relevant data files for GJ3942_time_series_analysis_TESS.ipynb were not included due to a file size limit. These files can be found at the Zenodo repository [here](https://doi.org/10.5281/zenodo.14187051). 

Recommended reading order for computational notebooks:
 - 1. GJ3942_coherence_final.ipynb
 - 2. GJ3942_time_series_analysis_TESS.ipynb
 - 3. GJ3942_time_series_analysis_SuperWASP.ipynb
 - 4. GJ3942_time_series_analysis_Hipparcos.ipynb

Packages required: numpy, matplotlib, scipy, copy, resample, finufft, NWelch

Uploaded file types: .cff, .tbl, .txt, .tbl.txt, .ipynb, .md

## Authors

Andrew Fonseca
[afonse@udel.edu]

Sarah Dodson-Robinson
[sdr@udel.edu]

---

[![DOI](https://zenodo.org/badge/830615706.svg)](https://doi.org/10.5281/zenodo.14187051)

