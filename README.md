# 🛍️ Rossmann Store Sales Forecasting

## 📌 Overview

This project forecasts daily sales for Rossmann stores across multiple locations using historical sales data, promotions, competition, and store metadata.  
The model uses **XGBoost**, a powerful gradient boosting algorithm, and performs feature engineering to incorporate **seasonality**, **lag features**, and **promotion cycles**.

📊 **Goal**: Help retail managers make informed decisions around inventory, staffing, and promotions by providing accurate sales predictions.

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
| `IsPromoMonth`         | Whether the current month is part of the promo cycle       |
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
