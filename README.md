# 🌾 Drought Forecasting in the Canadian Prairies 💧  
### Machine Learning Analysis of Drought Conditions (1982–2022)

This repository contains the complete pipeline for forecasting droughts in the Canadian Prairies using historical climate data from **1982 to 2022**.  
The project focuses on building and comparing four machine learning models for binary drought classification using two key features: **precipitation** and **evapotranspiration**.

---

## 📂 Project Files

- `CHIRPS_Monthly_Prairies_1982_2022.csv` – Monthly precipitation (mm) from CHIRPS  
- `ERA5_Evapotranspiration_Prairies_1982_2022.csv` – Monthly evapotranspiration (mm) from ERA5-Land  
- `PDSI_TerraClimate_Prairies_1982_2022.csv` – Palmer Drought Severity Index from TerraClimate  
- `EDA_Climate.py` – Optional script for exploratory data analysis  
- `data_preparation_modelling.py` – Merges and processes the raw datasets, generates the drought label, and outputs the final modeling dataset  
- `final_ml_model.py` – Trains and evaluates Logistic Regression, Random Forest, XGBoost, and SVM models  
- `README.md` – Project documentation  

---

## 🔍 Objectives

- Merge satellite climate datasets from **CHIRPS**, **ERA5-Land**, and **TerraClimate**  
- Create binary drought labels based on normalized PDSI:  
  - `1 = Drought` if PDSI < -0.5  
  - `0 = No Drought` otherwise  
- Build, tune, and evaluate four machine learning models:  
  - Logistic Regression  
  - Random Forest  
  - XGBoost  
  - Support Vector Machine (SVM)  

---

## 📊 Features Used

- `mean_precip_mm` – Monthly mean precipitation  
- `evap_mm` – Monthly evapotranspiration  

---

## 🧪 Modeling Process

Each model follows the same workflow:

- Stratified 80/20 train-test split  
- Feature standardization using `StandardScaler`  
- Hyperparameter tuning using 5-fold `GridSearchCV`  
- Evaluation using:
  - Accuracy  
  - F1-score  
  - ROC-AUC  
  - Confusion matrix  
  - Classification report  
- ROC Curve plotting  

---

## 🛠️ Tools & Libraries

- **Python 3**  
- `pandas`, `NumPy`  
- `scikit-learn`  
- `xgboost`  
- `matplotlib`, `seaborn`  

---

## 👤 Author

**Sanan Thushanthan**  
Toronto Metropolitan University – Master of Data Science and Analytics (MDSA)  
**Supervisor:** Dr. Farid Shirazi
