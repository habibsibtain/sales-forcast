# 🛒 Walmart Sales Forecasting using Machine Learning

This project involves building a robust regression model to forecast sales for Walmart stores using machine learning. Various regression algorithms and an Artificial Neural Network (ANN) were evaluated using GridSearchCV, and the best-performing models were selected based on RMSE and R² score.

---

## 📌 Project Objective

To predict weekly sales across Walmart stores using historical data and promotional information, helping with inventory planning and business decision-making.

---

## 📁 Dataset

The dataset comes from the [Walmart Store Sales Forecasting](https://www.kaggle.com/datasets/aslanahmedov/walmart-sales-forecast), containing:

- **Store**: Unique identifier for each store
- **Dept**: The department number
- **Date**: Weekly date
- **Weekly_Sales**: Target variable
- **IsHoliday**: Whether the week includes a special holiday
- **Temperature**, **Fuel_Price**, **CPI**, **Unemployment**, etc.

---

## ⚙️ Technologies & Libraries Used

- **Python** (Jupyter Notebook, VS Code)
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn** (Regression models, GridSearchCV, Metrics)
- **TensorFlow / Keras** (ANN Model)

---

## 📊 Models & Results

### 🔍 Model Evaluation Summary

| Model                     | Best Parameters                          | CV RMSE     | Test RMSE   | R² Score     |
|--------------------------|------------------------------------------|-------------|-------------|--------------|
| **Linear Regression**     | `{}`                                     | 22327.82    | 22483.14    | 0.031        |
| **Ridge Regression**      | `{'alpha': 10}`                          | 22327.82    | 22483.14    | 0.031        |
| **Lasso Regression**      | `{'alpha': 0.1}`                         | 22327.82    | 22483.14    | 0.031        |
| **Decision Tree**         | `{'max_depth': None}`                    | **5067.40** | **4703.15** | **0.958**    |
| **Random Forest**         | `{'max_depth': None, 'n_estimators': 75}`| **4913.40** | **4782.06** | **0.956**    |
| **K-Nearest Neighbors**   | `{'n_neighbors': 3}`                     | 5945.09     | 5892.25     | 0.933        |
| **Gradient Boosting**     | `{'learning_rate': 0.1, 'n_estimators': 150}` | 12897.97 | 13069.84    | 0.672        |
| **AdaBoost Regressor**    | `{'learning_rate': 0.01, 'n_estimators': 50}` | 19383.61 | 19508.06    | 0.270        |
| **ANN (Neural Network)**  | -                                        | -           | -           | 0.485        |

> ✅ **Random Forest and Decision Tree** showed the best performance in terms of R² score and RMSE.
>
> ⚠️ **ANN** achieved moderate performance and may be improved with more tuning.

---

## 📈 Evaluation Metrics

- **RMSE** (Root Mean Squared Error)
- **R² Score** (Explained Variance)
- **MAE** (Mean Absolute Error, optional)

Residuals and feature importance were also analyzed to ensure model interpretability.

---

## 🧑‍💻 Author

**Md Sibtain Habib**  
📧 sibtainhabib413@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/md-sibtain-habib-38467b2b6/) • [GitHub](https://github.com/habibsibtain)

---

