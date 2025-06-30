# 🔥 Calories Calculator

A machine learning project that predicts the number of calories burned based on physiological and activity-related features using the **XGBoost Regressor**.

## 📌 Project Overview

The **Calories Calculator** uses supervised learning to estimate how many calories an individual burns during physical activity. This can be particularly useful for fitness tracking applications, personalized workout planning, or health monitoring tools.

The project involves:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Training a regression model with XGBoost
- Model evaluation using metrics like MAE, MSE, and R²
- A custom prediction function to estimate calories burned from new data

---

## 📂 Dataset

The dataset includes the following features:
- **Age**
- **Gender**
- **Height**
- **Weight**
- **Duration (minutes)**
- **Heart Rate**
- **Body Temperature**
- **Calories** *(Target variable)*

> 🔍 The dataset must be in CSV format. You can load it using `pandas.read_csv()`.

---

## 🚀 Model Used

We use the **XGBoost Regressor**, a powerful and efficient gradient boosting algorithm.

```python
from xgboost import XGBRegressor

model = XGBRegressor()
model.fit(X_train, y_train)
