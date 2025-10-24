HayRajBev2
Electric Vehicle Charging Demand

Course: DS 4002 Section 001
Date: 10/20/2025
Team Members: Hayden Cook (leader), Beverley Appiatse, Raj Bhowmic
Instructor: Professor Alonzi

Contents of the Repository

This repository follows the TIER Protocol 4.0 to ensure transparency and reproducibility.
It contains all code, data, documentation, and outputs associated with this project. The primary components are:

SCRIPTS/ – All source code used for data processing, modeling, and visualization.

DATA/ – Contains initial, cleaned, and processed datasets, along with metadata and data dictionaries.

OUTPUT/ – Generated figures, tables, and model results.

LICENSE.md – Specifies usage terms (MIT License).

README.md – Provides repository orientation and documentation.

Section 1: Software and Platform

Software Used:

Python 3.10 (Anaconda or standard distribution)

Jupyter Notebook for analysis and visualization

Add-on Packages:

pandas

numpy

matplotlib

seaborn

scikit-learn

To install all required packages:
pip install pandas numpy matplotlib seaborn scikit-learn

Platform:
Developed and tested on macOS.
Fully compatible with Windows and Linux systems.

Section 2: Map of the Repository

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

Each folder includes a local README.md file (where relevant) explaining its contents and purpose.

Section 3: Instructions for Reproducing Results

To ensure full reproducibility, follow the steps below.

Step 1: Clone the Repository
git clone https://github.com/your-username/your-repo-name.git

cd your-repo-name

Step 2: Set Up the Environment
It is recommended to use a virtual environment.
python -m venv env
source env/bin/activate (on macOS/Linux)
env\Scripts\activate (on Windows)
pip install -r requirements.txt

Step 3: Access the Data
Ensure the DATA/ folder contains raw_data.csv.
If the dataset is too large for GitHub, follow the download instructions in DATA/metadata_README.md (e.g., Google Drive or OneDrive link).

Step 4: Run Data Cleaning
python SCRIPTS/01_data_cleaning.py

Step 5: Train the Model
python SCRIPTS/03_model_training.py

Step 6: Generate Visualizations
jupyter notebook SCRIPTS/04_visualization.ipynb

Step 7: Review Outputs
All generated figures, tables, and summaries will appear in the OUTPUT/ folder.

Step 8: Verify Reproducibility
Ensure results align with those presented in the final report.
If discrepancies occur, confirm that package versions match those listed in requirements.txt.

References

Guo, X., Zhang, Y., & Li, T. (2025). CHARGED: A Harmonized Global Dataset for Electric Vehicle Charging Demand Forecasting. Harvard Dataverse. https://doi.org/10.7910/DVN/CHARGED

CHARGED Dataset GitHub Repository. (2025). Global EV Charging Data Collection and Benchmarking. Retrieved from: https://github.com/Tsinghua-IDEA-lab/CHARGED

OpenAI ChatGPT (2025). Assistance with data exploration, visualization, and report composition.

License

This project is licensed under the MIT License.
See LICENSE.md for full details.
