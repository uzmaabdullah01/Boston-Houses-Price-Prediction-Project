# Boston-Houses-Price-Prediction-Project
“MIT Elective Project analyzing the Boston Housing dataset using machine learning. Performed full EDA, correlation analysis, log transformation, VIF-based multicollinearity removal, and regression modelling. Achieved R² ~0.76 and identified major socioeconomic, structural, and environmental factors affecting housing prices.”
# 🏡 Boston Housing Price Prediction – MIT Elective Project  
*Machine Learning | Regression | EDA | VIF | Model Diagnostics*  
Based on: “ELECTIVE PROJECT ON MACHINE LEARNING – Boston House Price Prediction”  
Author: ** Dr. Uzma Abdullah**

---

## 📘 Project Overview  
This project analyzes the **Boston Housing dataset** to identify key drivers of property values and build a strong predictive model. It includes full Exploratory Data Analysis (EDA), data preprocessing, regression modelling, multicollinearity checks, residual diagnostics, and cross-validation.  
Findings and analysis are taken from the full project report.  

---

## 🎯 Objectives  
- Identify the socioeconomic, environmental, and structural factors influencing Boston house prices  
- Build a reliable OLS regression model  
- Improve model accuracy using log transformation and multicollinearity removal  
- Validate performance using train/test split and K-fold cross validation  

---

## 🧪 Dataset  
- **506 observations**, **13 variables**  
- No missing or duplicate values  
- Target: `MEDV` (median value of homes, $1000s)  
- Key predictors: CRIM, RM, LSTAT, NOX, PTRATIO, DIS, CHAS  

---

## 🔍 Key Insights (EDA)  
- **RM** (rooms) has strong *positive* correlation with price  
- **LSTAT** (% low-status population) strongly *negative*  
- **NOX**, **PTRATIO**, **CRIM** negatively impact prices  
- **CHAS** (near Charles River) increases prices  
- MEDV is capped at 50 → log transformation applied  

---

## 🧮 Regression Modelling  
### ✔ Full Model  
- **R² = 0.769**, Adjusted R² = 0.761  
- Significant predictors: CRIM, CHAS, NOX, RM, DIS, RAD, PTRATIO, LSTAT  
- Insignificant predictors removed: ZN, INDUS, AGE  

### ✔ Reduced Final Model  
- **R² = 0.767**, Adjusted R² = 0.762  
- Clean, efficient, all predictors statistically significant  
- Stable regression assumptions (linearity, homoscedasticity)

---

## 📊 Model Performance  
| Metric | Train | Test |
|--------|--------|--------|
| RMSE | 0.195 | 0.198 |
| MAE | 0
