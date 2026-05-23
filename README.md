# Greenhouse Crop Yield Prediction

Predicting greenhouse crop yield from IoT sensor data using machine learning.

**Research question:** Can we accurately predict greenhouse crop yield using IoT sensor and environmental data, and which model performs best?

---

## Files

| File | Description |
|------|-------------|
| `greenhouse_yield_prediction.ipynb` | Main notebook — EDA, models, evaluation |
| `greenhouse_crop_yields.csv` | Dataset (10,400 records) |
| `project_report.docx` | Final written report |

---

## Dataset

**Source:** [Kaggle — moezalikhan/greenhouse-crop-yields-dataset](https://www.kaggle.com/datasets/moezalikhan/greenhouse-crop-yields-dataset)  
**Size:** 10,400 rows, 20 features  
**Target:** `yield_kg_per_m2`  
**Crops:** Tomato, Cucumber, Lettuce, Pepper

---

## Models & Results

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression (baseline) | 2.44 | 3.08 | 0.60 |
| **Random Forest** | **1.66** | **2.09** | **0.82** |
| XGBoost | 1.72 | 2.18 | 0.80 |

Random Forest performed best. Results validated with 5-fold cross-validation.

---

## How to Run

Open `greenhouse_yield_prediction.ipynb` in Google Colab and run all cells. The dataset loads automatically from this repository — no uploads needed.

**Local:**
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn scipy
jupyter notebook greenhouse_yield_prediction.ipynb
```

---

## Submission — May 2026
