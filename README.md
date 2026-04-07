# Bulldozer Price Prediction

This repository contains an end‑to‑end **machine learning project** that predicts the **auction sale price of bulldozers** based on historical sales data and equipment features. The notebook applies data preprocessing, feature engineering, model training, and evaluation to build a regression model.  

The project is based on the **Bluebook for Bulldozers** dataset.

---

## 🚜 Project Overview

The goal of this project is to build a model that can predict the sale price of a bulldozer using historical auction data and equipment specifications. This is a **regression problem** — predicting a continuous numeric value. :contentReference[oaicite:2]{index=2}

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `bulldozer-price-regression.ipynb` | Main Jupyter Notebook with full model workflow |
| `data/TrainAndValid.csv` | Training & validation dataset |
| `data/Test.csv` | Test dataset for predictions |
| `README.md` | This file |

---

## 📊 Data Description

- The dataset is sourced from the **Kaggle Bluebook for Bulldozers competition**.  
- It includes features like make year, model, equipment attributes, and sale metadata.  
- The target variable is **SalePrice** (only in training data). :contentReference[oaicite:3]{index=3}

---

## 🛠 Project Pipeline

The notebook follows these high‑level steps:

1. **Data Loading & Exploration**  
2. **Feature Engineering** (e.g. extract year/month from sale date)  
3. **Handling Missing Values** (median imputation & missing flags)  
4. **Categorical Encoding** (integer codes)  
5. **Model Training** (e.g. RandomForestRegressor)  
6. **Evaluation**  
7. **Prediction on Test Set**  
8. **Exporting Results**

---

## 🧠 Preprocessing Details

- `saledate` is parsed into numerical components like year, month, day, and day of the week.  
- Numeric features are imputed with medians and missing indicators are created.  
- Categorical columns are encoded as numeric codes.  
- The test set is aligned with the training features before prediction.

---

## 📦 Requirements

To run the notebook, you need:

```bash
pip install pandas numpy scikit-learn matplotlib jupyter
