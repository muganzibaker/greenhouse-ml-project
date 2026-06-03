# Greenhouse Crop Yield Prediction

Predicting greenhouse crop yield from IoT sensor data using machine learning.

**Research question:** Can we accurately predict greenhouse crop yield using IoT sensor and environmental data, and which model performs best?

---

## Files

| File | Description |
|------|-------------|
| `greenhouse_yields_predictions.ipynb` | Main notebook — EDA, models, evaluation |
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
| Linear Regression (baseline) | 2.4441 | 3.0837 | 0.6019 |
| Random Forest | 1.6679 | 2.0952 | 0.8162 |
| **XGBoost** | **1.6501** | **2.0618** | **0.8221** |

XGBoost achieved the best performance with the highest R² of 0.8221 and MAE of 1.6501 kg/m² — meaning the model explains 82% of the variance in crop yield. Random Forest performed close behind (MAE = 1.6679 kg/m², RMSE = 2.0952 kg/m², R² = 0.8162). Linear Regression confirmed the baseline expectation: a significant portion of the yield-feature relationship is non-linear.

