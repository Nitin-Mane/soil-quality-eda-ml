# 🌱 Soil Quality EDA & Machine Learning for Rice

This repository provides **data cleaning, exploratory data analysis (EDA), and machine learning pipelines** for soil nutrient datasets, with a focus on **rice cultivation**.

---

## 📂 Repository Structure
```

soil-quality-eda-ml/
│
├── notebooks/
│   ├── Data\_Cleaning\_Soil.ipynb        # full data cleaning workflow
│   ├── Soil\_EDA\_ML\_Rice.ipynb          # rice-focused EDA + ML analysis
│
├── outputs/                            # generated plots & cleaned files
│   ├── crop\_yield\_dataset.cleaned.csv
│   ├── cleaning\_report.json
│   ├── missing\_before.png
│   ├── missing\_after.png
│   └── dist\_clean\_\*.png
│
├── data/
│   └── crop\_yield\_dataset.csv          # raw dataset (optional, or .gitignore)
│
├── requirements.txt                    # Python dependencies
├── README.md                           # project overview
└── LICENSE (optional)

```

---

## ⚙️ Installation
Clone the repo and install dependencies:

```bash
git clone https://github.com/Nitin-Mane/soil-quality-eda-ml.git
cd soil-quality-eda-ml
pip install -r requirements.txt
````

Dependencies include:

* `numpy`, `pandas`, `matplotlib`, `scikit-learn`
* `xgboost` & `lightgbm` (optional for advanced models)
* `jupyterlab` for running notebooks

---

## ▶️ Usage

1. Place your raw dataset in `data/crop_yield_dataset.csv`.
2. Run the cleaning notebook:

   * `notebooks/Data_Cleaning_Soil.ipynb`
3. Use the cleaned file (`outputs/crop_yield_dataset.cleaned.csv`) for analysis:

   * `notebooks/Soil_EDA_ML_Rice.ipynb`

---

## 📊 Features

* Handles **missing values** with median/mode imputation
* Removes **duplicates** and fixes **out-of-range values** (e.g., pH, humidity)
* Detects & optionally clips **outliers** (IQR winsorization)
* Generates **summary statistics, correlation heatmaps, distributions**
* Trains and compares **ML models**:

  * Linear Regression
  * Random Forest (default & tuned via CV)
  * XGBoost / LightGBM (if installed)
* Stratified comparisons by **Soil\_Type** and **pH\_bin**

---

## 📈 Example Outputs

* Nutrient % vs rice target bar chart
* Missingness plots (before/after cleaning)
* Distribution plots (pH, N, P, K, Yield)
* Correlation heatmap
* Per-soil-type and per-pH\_bin model performance

---

## 📜 License

MIT License (or add your preferred license)

---

✨ Maintained by [Your Name](https://github.com/Nitin-Mane)

```
