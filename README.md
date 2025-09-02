# 🌱 Soil Quality EDA & Machine Learning for Rice

This repository provides **data cleaning, exploratory data analysis (EDA), and machine learning pipelines** for soil nutrient datasets, with a focus on **rice cultivation**.

## 📂 Contents
- `notebooks/Data_Cleaning_Soil.ipynb`  
  → Cleans the raw dataset (`crop_yield_dataset.csv`): handles missing values, outliers, plausibility checks, imputations, and saves a cleaned CSV + cleaning report.
- `notebooks/Soil_EDA_ML_Rice.ipynb`  
  → Performs EDA (correlation heatmaps, distributions) and trains ML models (Linear Regression, Random Forest, XGBoost/LightGBM if available) to predict `Crop_Yield`.
- `outputs/`  
  → Stores all cleaned files, plots, and metrics (auto-generated).

## ⚙️ Installation
Clone the repo and install dependencies:
```bash
git clone https://github.com/Nitin-Mane/soil-quality-eda-ml.git
cd soil-quality-eda-ml
pip install -r requirements.txt
