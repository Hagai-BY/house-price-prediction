# 🏠 House Price Prediction Pipeline

This project implements a full machine learning pipeline for predicting house prices using **LightGBM** and **XGBoost**.

---

## 📌 **Project Overview**
This project includes:
1. **Data Cleaning & Processing** – Handling missing values, fixing inconsistencies, and feature engineering.  
2. **Modeling** – Training using LightGBM and XGBoost, including hyperparameter tuning and early stopping.  
3. **Prediction** – Generating predictions and creating a competition-ready submission file.  

---

## 🚀 **Highlights**
✅ **Feature Engineering** – Created 20+ new features (ratio, area size, room count)  
✅ **Full Pipeline** – Data loading → Preprocessing → Feature Engineering → Model Training → Prediction  
✅ **Model Comparison** – LightGBM outperformed XGBoost by ~10% in RMSLE  
✅ **Handling Missing Data** – Combined median/mode and KNN-based imputation  
✅ **Outlier Removal** – Cleaned unrealistic floor values and room counts  

---

## 🏆 **Technical Details**
### 📥 **1. Data Retrieval**
- Loaded from CSV files.  
- Cleaned inconsistencies in `floor`, `room_count`, and `build_year`.  

### 🔎 **2. Data Cleaning & Processing**
- Replaced unrealistic values with NaN.  
- Created new features:  
    - **resident_to_total_ratio** – Ratio of net area to total area.  
    - **year_month** – Monthly trend indicator.  
- Applied imputation using median/mode and KNN.  

### 🌳 **3. Modeling**
- Trained two models:  
    - ✅ LightGBM (final model)  
    - ✅ XGBoost (with and without PCA)  
- Used `early stopping` to prevent overfitting.  

### 🧠 **4. Prediction & Submission**
- Generated submission file in `final_submission.csv`  
- LightGBM achieved the best RMSLE score (0.205)  

---

## 🚀 **How to Run**
### ✅ **Clone the repository:**
```bash
git clone https://github.com/Hagai-BY/house-price-prediction.git

git lfs install

