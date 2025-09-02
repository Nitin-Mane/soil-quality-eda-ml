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
git clone https://github.com/YOUR_USERNAME/soil-quality-eda-ml.git
cd soil-quality-eda-ml
pip install -r requirements.txt
Dependencies:

Python 3.9+

pandas, numpy, matplotlib

scikit-learn

xgboost (optional)

lightgbm (optional)

▶️ Usage
Place your raw dataset in data/crop_yield_dataset.csv.

Run the cleaning notebook:

notebooks/Data_Cleaning_Soil.ipynb

Use the cleaned data (outputs/crop_yield_dataset.cleaned.csv) for modeling:

notebooks/Soil_EDA_ML_Rice.ipynb

📊 Features
Handles missing values (median/mode imputation).

Removes duplicates and corrects out-of-range values (e.g., pH, humidity).

Detects and optionally clips outliers via IQR winsorization.

Generates summary statistics, correlation heatmaps, and distributions.

Trains baseline and tuned models (Random Forest, Linear Regression, optional XGBoost/LightGBM).

Provides per-Soil_Type and per-pH_bin model comparisons.

📈 Example Plots
Correlation heatmap

Nutrient % vs rice target

Distribution of soil pH, N, P, K

Per-soil-type model performance

📜 License
MIT License (or add your preferred license)

✨ Maintained by Nitin Mane
