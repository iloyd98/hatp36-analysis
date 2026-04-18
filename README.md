# HAT-P-36 Analysis

This repository presents a full analysis of the HAT-P-36 system, including:

- Spectroscopic reduction of the host star (HAT-P-36)
- Transit photometry analysis of HAT-P-36 b
- Estimation of stellar temperature and planetary radius

---

## Repository Structure

- data/ : Observational data (FAST + KeplerCam)
- notebooks/ : Analysis pipelines
- results/ : Generated plots and outputs

---

## Data Access

Due to file size constraints, the full dataset (~5 GB) is hosted externally:

[INSERT GOOGLE DRIVE LINK HERE]

### Setup Instructions

1. Download the dataset from the link above.
2. Place the data into the following directory structure:

Place FAST data inside:
data/FAST/2026-03-18/

Place KeplerCam data inside:
data/KeplerCam/2026-03-18/

The notebook assumes this exact structure.

---

## How to Run

1. Clone this repository:

git clone https://github.com/iloyd98/hatp36-analysis.git
cd hatp36-analysis

2. Install required packages:

pip install astropy photutils plotly batman-package

3. Launch Jupyter:

jupyter lab

4. Open and run:

notebooks/hatp36_analysis.ipynb

5. Run all cells from top to bottom.

---

## Reproducibility

This repository is designed to be fully reproducible:

- All file paths are relative
- The notebook runs end-to-end without modification
- All figures and results are generated directly from the data

---

## Notes

- The FAST pipeline performs spectral reduction and temperature estimation.
- The KeplerCam pipeline extracts a transit light curve and fits a transit model.
- Stellar parameters used in the transit fit are consistent with literature values for HAT-P-36.

---

## Author

Ian Loyd  
Harvard University — ASTRON 100
