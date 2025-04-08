# 🛍️ Rossmann Store Sales Forecasting

## 📌 Overview

Forecasts daily sales for 1,115 Rossmann stores using XGBoost. Helps optimize:
- Inventory management 
- Staff scheduling  
- Promotional planning 

---

## 🏆 Key Results
✅ **17% MAPE** (42% better than naive baseline)  
✅ Processes 1M+ records in <5 minutes  
✅ Identified 3 underperforming promo strategies 

---

## 📂 Dataset

- Source: [Rossmann Sales Forecasting on Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales)
- `train.csv`: Historical sales data for 1,115 Rossmann stores
- `store.csv`: Additional information about each store (type, competition, promos)

---

## 🧠 Features Engineered

| Feature                | Description                                            |
|------------------------|--------------------------------------------------------|
| `WeekOfYear`           | Seasonality indicator                                  |
| `MonthsSinceCompetition` | Time since a competitor opened near the store        |
| `IsPromoMonth`         | Detects effective promo timing       |
| `PrevWeekSales`        | Lag feature to capture recent sales trend              |

---

## ⚙️ Tools & Libraries

- Python 🐍
- Pandas & NumPy
- XGBoost (regression)
- Matplotlib
- Scikit-learn

---

## 🚀 Model Summary

- **Model**: XGBoost Regressor  
- **Evaluation Metric**: MAPE (Mean Absolute Percentage Error) 
