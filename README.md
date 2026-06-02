# Greenhouse Crop Yield Prediction

Predicting greenhouse crop yield from IoT sensor data using machine learning.

**Research question:** Can we accurately predict greenhouse crop yield using IoT sensor and environmental data, and which model performs best?

---

## Files

| File | Description |
|------|-------------|
| `greenhouse_yield_prediction(5).ipynb` | Main notebook — EDA, models, evaluation |
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
| Linear Regression (baseline) | 2.4429 | 3.0830 | 0.6021 |
| **Random Forest** | **1.6584** | **2.0886** | **0.8174** |
| XGBoost | 1.7221 | 2.1750 | 0.8020 |

Random Forest performed best. Results validated with 5-fold cross-validation.

---

```

---
