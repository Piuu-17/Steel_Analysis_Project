# Steel Industry Energy Consumption Analysis & Prediction

This repository contains a comprehensive data science project predicting electricity consumption for a South Korean steel manufacturing plant using historical operational data from the UCI Machine Learning Repository.

##  Overview
Understanding and forecasting power consumption is essential for smart grid management and operational efficiency. This project implements data cleaning, feature engineering, and multiple regression algorithms to accurately predict power usage.

## 📊 Dataset Information
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Steel+Industry+Energy+Consumption+Dataset) / Korea Electric Power Corporation
- **Records:** 35,040 instances
- **Features:** 11 features including reactive power (`Lagging` & `Leading`), power factor, $CO_2$ emissions, time-based features (`NSM` - Number of Seconds from Midnight), `WeekStatus`, `Day_of_week`, and `Load_Type`.
- **Target Variable:** `Usage_kWh` (Energy consumption in kWh)

##  Tech Stack & Libraries
- **Language:** Python
- **Data Handling:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Sweetviz
- **Machine Learning:** Scikit-Learn

##  Model Performance & Results

| Model | R^2 Score | Mean Absolute Error (MAE) |
| :--- | :--- | :--- |
| **Random Forest** | **0.9988** | **0.4256** |
| Decision Tree | 0.9978 | 0.6266 |
| KNN Regressor | 0.9947 | 1.1483 |
| Support Vector Machine (SVR) | 0.9930 | 1.2400 |
| Linear Regression | 0.9824 | 2.5020 |

**Key Finding:** The **Random Forest Regressor** demonstrated superior performance, achieving the highest accuracy with an $R^2$ score of **99.88%** and the lowest Mean Absolute Error.
