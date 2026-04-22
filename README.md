# Housing_prediction_model
# 🏠 House Price Prediction (USA Housing Dataset)

## 📌 Project Overview

This project builds a **Linear Regression model** to predict house prices using socio-economic and housing features. It includes **data exploration, visualization, feature engineering, and model evaluation** to understand key drivers of housing prices.

---

## 📊 Dataset

* **Dataset:** USA Housing
* **Records:** 5000 rows
* **Features:**

  * Avg. Area Income
  * Avg. Area House Age
  * Avg. Area Number of Rooms
  * Avg. Area Number of Bedrooms
  * Area Population
  * Price (Target)
  * Address

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Observations:

* **Income → Price:** Strong positive correlation
* **Rooms → Price:** Moderate positive relationship
* **Population → Price:** Moderate impact (demand factor)
* **Bedrooms → Price:** Weak relationship (redundant with rooms)
* Price distribution is **approximately normal**, making it suitable for regression

### Visualizations Used:

* Pairplot
* Correlation Heatmap
* Scatter Plots
* Histogram of Price

---

## ⚙️ Feature Engineering

New features were created to capture deeper relationships:

* `Income_per_Person = Income / Population`
* `Rooms_per_House = Rooms / House Age`

---

## 🤖 Model Building

### Algorithm Used:

* **Linear Regression**

### Features Used:

* Avg. Area Income
* Avg. Area House Age
* Avg. Area Number of Rooms
* Area Population

---

## 📈 Model Evaluation

| Metric | Value    |
| ------ | -------- |
| MAE    | ~82,000  |
| MSE    | ~1.04e10 |
| RMSE   | ~102,000 |

### Interpretation:

* Predictions are on average **within ~6–7% of actual prices**
* Low error indicates **strong model performance**
* Slight difference between MAE and RMSE suggests **minor outliers**

---

## 🧠 Model Insights

* **Income is the strongest driver** of house prices
* **Number of Rooms significantly increases value**
* **House Age reflects area development and affects pricing**
* **Population indicates demand but has moderate impact**
* Bedrooms were excluded due to **redundancy**

---

## 📊 Results Visualization

* **Actual vs Predicted Plot:** Strong linear alignment → high accuracy
* **Residual Distribution:** Errors are centered → model is stable

---

## 🧾 Regression Equation

[
Price = b_0 + b_1(Income) + b_2(HouseAge) + b_3(Rooms) + b_4(Population)
]

* Coefficients represent **impact of each feature on price**
* Intercept adjusts the model baseline

---

## 📦 Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📁 Project Workflow

1. Data Loading & Inspection
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Train-Test Split
5. Model Training (Linear Regression)
6. Evaluation & Visualization

---

## 🚀 Future Improvements

* Implement **Ridge / Lasso Regression**
* Try **Random Forest / XGBoost** for better accuracy
* Perform **hyperparameter tuning**
* Deploy model using **Streamlit or Flask**

---

## 🎯 Conclusion

The linear regression model performs well with **high accuracy (R² ≈ 0.92)** and low error. The dataset structure supports linear modeling, and key insights highlight the importance of income and house size in determining property prices.

---

## 🙌 Author

Anas Khan


---
