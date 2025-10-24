# HayRajBev2

## Electric Vehicle Charging Demand

**Course:** DS 4002 Section 001  
**Date:** 10/20/2025  
**Team Members:** Hayden Cook (leader), Beverley Appiatse, Raj Bhowmic  
**Instructor:** Professor Alonzi

---

## Contents of the Repository

This repository follows the TIER Protocol 4.0 to ensure transparency and reproducibility. Top-level items:

- LICENSE.md  
- README.md (this file)  
- SCRIPTS/ — source code and execution scripts  
- DATA/ — raw and processed datasets and metadata_README.md  
- OUTPUT/ — figures, tables, and model outputs  
- docs/ — proposal and final report

---

## Section 1: Software and Platform

### Software used
- Python 3.10 (Anaconda or standard distribution)  
- Jupyter Notebook

### Add-on packages (install before running)
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn

(Install with: `pip install -r requirements.txt` — `requirements.txt` is included in the repo.)

### Platform
- Developed and tested on macOS Monterey (12.6)  
- Compatible with Windows 10/11 and Linux

---

## Section 2: Map of Documentation

**Repository structure (top-level):**

- README.md  
- LICENSE.md  
- SCRIPTS/  
  - 01_data_cleaning.py  
  - 02_feature_engineering.py  
  - 03_model_training.py  
  - 04_visualization.ipynb  
- DATA/  
  - raw/ (original files)  
  - processed/ (cleaned files)  
  - metadata_README.md (data summary, provenance, license, data dictionary, ethical statements, 2+ plots)  
- OUTPUT/  
  - figures/  
  - tables/  
  - model_artifacts/  
- docs/  
  - project_proposal.pdf  
  - final_report.pdf

Each folder contains a local README.md (where relevant) describing contents and usage.

---

## Section 3: Instructions for Reproducing Results

Follow these steps in order to reproduce the project results.

1. **Clone the repository and change directory**  
   - `git clone https://github.com/your-username/HayRajBev2.git`  
   - `cd HayRajBev2`

2. **Set up environment**  
   - Create and activate a virtual environment (recommended).  
     - macOS / Linux: `python -m venv env && source env/bin/activate`  
     - Windows (PowerShell): `python -m venv env; .\env\Scripts\Activate.ps1`  
   - Install dependencies: `pip install -r requirements.txt`

3. **Obtain data**  
   - If `DATA/raw/` is present in the repo, skip.  
   - If not (large files), follow `DATA/metadata_README.md` to download and place files into `DATA/raw/`.  
   - Confirm expected filenames listed in `DATA/metadata_README.md`.

4. **Preprocess data**  
   - Run: `python SCRIPTS/01_data_cleaning.py`  
   - Output: cleaned files saved to `DATA/processed/`. Check logs printed to console.

5. **Feature engineering**  
   - Run: `python SCRIPTS/02_feature_engineering.py`  
   - Output: feature datasets saved to `DATA/processed/`.

6. **Train baseline and models**  
   - ARIMA baseline (example): `python SCRIPTS/03_model_training.py --model arima --site-id 100`  
   - Deep learning example (if included): `python SCRIPTS/03_model_training.py --model lstm --epochs 50`  
   - Model artifacts and logs are written to `OUTPUT/model_artifacts/`.

7. **Generate visualizations and results**  
   - Open and run notebook: `jupyter notebook SCRIPTS/04_visualization.ipynb`  
   - Final figures and CSV summaries saved to `OUTPUT/figures/` and `OUTPUT/tables/`.

8. **Verify outputs**  
   - Compare generated files in `OUTPUT/` with those in `OUTPUT/reference/` (if provided).  
   - Key metrics are recorded in `OUTPUT/tables/metrics_summary.csv`.

**Notes:**  
- Use the `--help` option on scripts for additional flags and options (e.g., `--site-id`, `--start-date`, `--end-date`).  
- For reproducible runs, seed randomness where applicable; seeds used in experiments are recorded in `OUTPUT/model_artifacts/training_config.json`.

---

## References

Guo, X., Zhang, Y., & Li, T. (2025). *CHARGED: A Harmonized Global Dataset for Electric Vehicle Charging Demand Forecasting.* Harvard Dataverse. https://doi.org/10.7910/DVN/CHARGED

CHARGED Dataset GitHub Repository. (2025). Global EV Charging Data Collection and Benchmarking. Retrieved from: https://github.com/Tsinghua-IDEA-lab/CHARGED

OpenAI ChatGPT. (2025). Assistance with data exploration, visualization, and report composition.

---

## License

This repository is licensed under the MIT License. See LICENSE.md for details.
