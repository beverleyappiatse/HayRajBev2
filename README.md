HayRajBev2
Electric Vehicle Charging Demand

Course: DS 4002 Section 001
Date: 10/20/2025
Team Members: Hayden Cook (leader), Beverley Appiatse, Raj Bhowmic
Instructor: Professor Alonzi

Contents of the Repository

This repository follows the TIER Protocol 4.0 to ensure transparency and reproducibility.
It contains all code, data, documentation, and outputs associated with this project. The primary components are:

Section 1: Software and Platform

Software Used:
The primary software used for this project is Python 3.11.

Packages:
The following Python packages are required:

pandas

numpy

matplotlib

seaborn

scikit-learn

Platform:
The project was developed and tested on macOS Monterey (version 12.6), but it should also be compatible with Windows 10/11 and Linux operating systems.

Section 2: Map of Documentation

Repository Structure:

Top-level directory:

README.md – Overview and documentation of the repository.

LICENSE.md – Project license (MIT).

SCRIPTS/ – Contains all Python scripts used in data processing and analysis.

DATA/ – Contains all datasets used in the project.

raw/ – Original, unaltered datasets.

processed/ – Cleaned and transformed datasets ready for analysis.

OUTPUT/ – Contains results and generated figures.

figures/ – Visualizations produced from the analysis.

tables/ – Exported summary statistics and data tables.

Section 3: Instructions for Reproducing Results

To reproduce the results of this project, follow the steps below:

1. Clone the repository
Download a local copy by running:
git clone [repository-link]

2. Install dependencies
Install all required packages using:
pip install -r requirements.txt

3. Access the data
Make sure all raw datasets are located in the DATA/raw folder.

4. Run preprocessing scripts
Execute the scripts in the SCRIPTS folder in numerical order (e.g., 01_clean_data.py, 02_analyze_data.py).

5. Generate outputs
After running the scripts, results will automatically be saved in the OUTPUT folder under figures and tables.

6. Verify results
Compare your generated results with the reference files in OUTPUT to confirm successful replication.

References

Guo, X., Zhang, Y., & Li, T. (2025). CHARGED: A Harmonized Global Dataset for Electric Vehicle Charging Demand Forecasting. Harvard Dataverse. https://doi.org/10.7910/DVN/CHARGED

CHARGED Dataset GitHub Repository. (2025). Global EV Charging Data Collection and Benchmarking. Retrieved from https://github.com/Tsinghua-IDEA-lab/CHARGED

OpenAI ChatGPT. (2025). Assistance with data exploration, visualization, and report composition.
