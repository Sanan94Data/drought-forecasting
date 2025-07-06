# drought-forecasting
"Machine learning analysis of drought conditions in the Canadian Prairies"
# Drought Forecasting in the Canadian Prairies 🌾💧

This repository contains the code, datasets, and methodology for my data science project on forecasting drought events using climate data from 2012 to 2022.

## 📂 Project Structure

- `drought_eda.py`: Exploratory Data Analysis script
- `data/`: Contains cleaned CSV files used in analysis
- `eda/`: Contains generated visualizations (plots, heatmaps, etc.)
- `methodology_diagram.png`: Visual overview of project workflow
- data_preparation.py: Loads and merges raw climate datasets, creates the drought label, splits the data into training and test sets with stratification, and standardizes predictor variables for modeling.



## 📊 Key Datasets

- **CHIRPS** – Precipitation (mm)
- **ERA5-Land** – Evapotranspiration (mm)
- **TerraClimate** – Palmer Drought Severity Index (PDSI)

## 🔍 Goals

- Identify drought patterns across Alberta, Saskatchewan, and Manitoba
- Create binary drought labels using PDSI < -0.5
- Develop a machine learning model to forecast droughts using precipitation and evapotranspiration

## 🧠 Tools Used

- Python (pandas, NumPy, matplotlib, seaborn)
- Google Earth Engine
- Jupyter Notebook

## 👤 Author

Sanan Thushanthan  
Toronto Metropolitan University – MDSA Program  
Supervisor: Dr. Farid Shirazi
