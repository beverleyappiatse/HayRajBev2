# HayRajBev2
# Electric Vehicle Charging Demand

## Course: DS 4002 Section 001
## Date: 10/20/2025
## Team Members: Hayden Cook (leader), Beverley Appiatse, Raj Bhowmic
## Instructor: Professor Alonzi

### Contents of the Repository

This repository is structured following the TIER Protocol 4.0 to ensure transparency and reproducibility. It includes all code, data, documentation, and outputs used to complete this project. The major folders are:

SCRIPTS/ – Contains all source code and scripts used for data processing, analysis, and visualization

DATA/ – Contains initial, cleaned, and processed datasets, along with metadata and data dictionaries

OUTPUT/ – Contains all generated figures, tables, and results from the analysis

LICENSE.md – Specifies the terms of use (MIT License by default)

README.md – Orientation and documentation for this repository

#### Section 1: Software and Platform

Software Used:

Python 3.10 (Anaconda or standard distribution)

Jupyter Notebook for running analysis and visualizations

Add-on Packages:

pandas

numpy

matplotlib

seaborn

scikit-learn

Platform:

Developed and tested on macOS Monterey (version 12.6)

Fully compatible with Windows 10/11 and Linux systems

#### Section 2: Map of Documentation

Repository Structure:

project-repository/
│
├── README.md
├── LICENSE.md
│
├── SCRIPTS/
│ ├── 01_data_cleaning.py
│ ├── 02_feature_engineering.py
│ ├── 03_model_training.py
│ ├── 04_visualization.ipynb
│
├── DATA/
│ ├── raw_data.csv
│ ├── cleaned_data.csv
│ ├── metadata_README.md
│
├── OUTPUT/
│ ├── model_summary.txt
│ ├── results_table.csv
│ ├── figure_1_accuracy_plot.png
│ ├── figure_2_feature_importance.png
│
└── docs/
├── project_proposal.pdf
├── final_report.pdf

Each folder contains a local README.md where relevant, explaining the files and their purposes.

#### Section 3: Instructions for Reproducing Results

Step 1: Clone the Repository
Download a local copy by running:
git clone [repository-link]
cd your-repo-name

Step 2: Set Up the Environment
It is recommended to use a virtual environment. Install dependencies listed in requirements.txt:
python -m venv env
source env/bin/activate (macOS/Linux)
env\Scripts\activate (Windows)
pip install -r requirements.txt

Step 3: Access the Data
Ensure the DATA/ folder contains raw_data.csv. If the dataset is too large for GitHub, refer to DATA/metadata_README.md for a download link.

Step 4: Run Data Cleaning
Execute the first script to clean and prepare the dataset:
python SCRIPTS/01_data_cleaning.py

Step 5: Train the Model
Run the model training script:
python SCRIPTS/03_model_training.py

Step 6: Generate Visualizations
Open the Jupyter Notebook and execute all cells to create visualizations:
jupyter notebook SCRIPTS/04_visualization.ipynb

Step 7: Review the Outputs
All generated tables and figures will appear in the OUTPUT/ folder.

Step 8: Verify Results
The outputs should reproduce the same results as shown in the presentation and final report. Ensure all dependencies and package versions match those listed.

### References

Guo, X., Zhang, Y., & Li, T. (2025). CHARGED: A Harmonized Global Dataset for Electric Vehicle Charging Demand Forecasting. Harvard Dataverse. https://doi.org/10.7910/DVN/CHARGED

CHARGED Dataset GitHub Repository. (2025). Global EV Charging Data Collection and Benchmarking. Retrieved from: https://github.com/Tsinghua-IDEA-lab/CHARGED

OpenAI ChatGPT. (2025). Assistance with data exploration, visualization, and report composition.

License

This repository uses the MIT License (see LICENSE.md for full details).
