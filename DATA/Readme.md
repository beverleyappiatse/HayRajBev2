###Dataset Establishment Details

##Summary
The dataset used for this project is the CHARGED dataset (Guo et al., 2025), a large-scale, harmonized collection of electric vehicle (EV) charging data compiled from multiple cities worldwide. It provides hourly site-level information, including timestamp, site ID, location, total energy delivered (in kWh), and the number of sessions (volume), along with contextual variables such as temperature, precipitation, and electricity prices when available. The dataset is publicly accessible through the Harvard Dataverse repository and will be stored in our group’s shared Google Drive for collaboration. Our initial exploration focuses on the Los Angeles subset due to its rich coverage and clear temporal patterns. Early observations reveal strong daily and weekly trends in volume, with demand peaking during daytime hours and weekdays, suggesting meaningful temporal structure for forecasting. This dataset’s comprehensive scope and hourly granularity make it well-suited for modeling site-level charging demand and evaluating the performance of classical and deep learning approaches.

##Provenance
Researchers at Tsinghua University and collaborators developed the CHARGED dataset to create a standardized, city-scale benchmark for analyzing global EV charging behavior. Data were aggregated from multiple open-access and partner-supplied sources, including regional utility companies, public charging network operators, and smart mobility platforms. To ensure consistency, timestamps, site identifiers, and energy units were harmonized across all cities. The dataset underwent rigorous cleaning and validation to remove duplicates, correct missing timestamps, and align site-level attributes with spatial and temporal references. Each city’s data were verified against local energy statistics and grid load profiles to ensure representativeness. This transparent and well-documented process makes the CHARGED dataset a reliable foundation for cross-city comparisons and reproducible forecasting analyses.

##License
The CHARGED dataset is distributed under the Creative Commons Attribution 4.0 International (CC BY 4.0) license, which permits sharing and adaptation of the data, provided that proper credit is given to the original authors. This open-access license encourages academic and research use while promoting transparency and reproducibility in data-driven studies. Users are free to use, modify, and redistribute the dataset for non-commercial purposes, provided attribution is maintained and any derived works indicate if changes were made. Our project complies fully with the licensing terms, and all references to the dataset appropriately credit Guo et al. (2025) as the data creators.

###Data Dictionary

Field/Column                    Type                   Description                        Units/Values                             Uncertainty
Timestamp                     Datetime       Date and hour of the measurement           YYYY-MM-DD HH: MM                  Low (assuming accurate logging)
Site ID                        Integer     Identifier for the measurement location    Column headers (0, 1, 10, 100…)        Unknown / Not provided
Volume                          Float      Measured quantity at that site and time      Numeric values (0+)                 Measurement error unknown


##Exploratory Data Analysis

Figure 1. Energy Demand (Day by Day datapoints) - Month on X-Axis
Reference EDA file

Figure 2. Average Charging Demand by the Hour of the Day (Hour 0 = 12am, Hour 23 = 11pm)
Reference EDA file
