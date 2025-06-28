# Medical Cost Prediction using Machine Learning Models

This project aims to predict individual medical insurance costs based on personal and health-related information using various machine learning models. The dataset used is the popular `insurance.csv`, which contains features like age, BMI, smoker status, and region.

---

## Dataset

- **Source**: [insurance.csv](https://www.kaggle.com/mirichoi0218/insurance)
- **Total Records**: 1338
- **Features**:
  - `age`: Age of the individual
  - `sex`: Gender
  - `bmi`: Body Mass Index
  - `children`: Number of children covered by insurance
  - `smoker`: Smoking status
  - `region`: Residential region
  - `expenses`: Medical insurance charges (Target)

---

## Objective

To build a regression model that accurately predicts `expenses` based on input features, and deploy the solution using **Streamlit** for interactive user predictions.

---

## 🛠Techniques Used

- Exploratory Data Analysis (EDA)
- Outlier Detection & Treatment (IQR Capping)
- Feature Engineering (One-Hot Encoding)
- Log Transformation of Target
- Feature Selection (SelectKBest)
- Model Training & Comparison:
  - Linear Regression
  - Ridge & Lasso Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Hyperparameter Tuning (GridSearchCV)
- Residual Analysis
- Model Evaluation Metrics
- Streamlit Deployment

---

## Model Performance Summary

| Model                | MAE    | RMSE   | R² Score |
|---------------------|--------|--------|----------|
| **Linear Regression**    | 3850.09 | 7150.27 | 0.72     |
| **Lasso Regression**     | 5142.60 | 9222.12 | 0.54     |
| **Ridge Regression**     | 3849.68 | 7147.69 | 0.72     |
| **XGBoost Regressor**    | **2088.97** | **4432.46** | **0.89** |
| **Random Forest Regressor** | 2328.24 | 4685.04 | 0.88     |

---

## Streamlit App

Run the interactive web app with this command:

```bash
streamlit run app.py
