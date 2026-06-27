# 🌾 Irrigation Need Prediction: Agricultural Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-success.svg)]()
[![LightGBM](https://img.shields.io/badge/LightGBM-orange.svg)]()

## 📌 Project Overview
This notebook builds a machine learning pipeline to predict **irrigation need** (Low / Medium / High) for agricultural fields, likely as part of a Kaggle competition.[cite: 2] By analyzing environmental, soil, and crop factors, the models forecast water requirements to aid sustainable agriculture and improve resource management.

## 📊 Dataset
Two CSV files are loaded — `train.csv` (with labels) and `test.csv` (without labels).[cite: 2] Basic exploration is done via `.head()`, `.info()`, and `.isnull().sum()` to understand the structure, data types, and missing values.[cite: 2]

Key features evaluated include:
* **Soil Metrics**: Soil Type, Soil pH, Soil Moisture, Organic Carbon, Electrical Conductivity.
* **Weather Metrics**: Temperature, Humidity, Rainfall, Sunlight Hours, Wind Speed.
* **Crop Data**: Crop Type, Crop Growth Stage, Season.
* **Irrigation Features**: Irrigation Type, Water Source, Field Area, Mulching Used, Previous Irrigation.
* **Target Variable**: `Irrigation_Need` (Low, Medium, High).

## 🧠 Exploratory Data Analysis & Modeling
Two sets of visualizations are created:[cite: 2]
* **Categorical features** (e.g., Soil Type, Crop Type, Season, Region) are plotted as count plots grouped by the target class `Irrigation_Need`, revealing how each category distributes across irrigation levels.[cite: 2]
* **Numerical features** (e.g., Temperature, Humidity, Rainfall) are plotted as histograms with KDE curves, again split by the target, to observe how their distributions differ across irrigation classes.[cite: 2]

The notebook uses a rich set of libraries: **Pandas** for data manipulation, **Seaborn/Matplotlib** for visualization, **Scikit-learn** for modeling utilities, and **XGBoost/LightGBM** as the core gradient boosting models.[cite: 2]

## 🚀 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/atahancelenk/irrigation-need-prediction.git](https://github.com/yourusername/irrigation-need-prediction.git)
   cd irrigation-need-prediction