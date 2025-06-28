# 📊 Telco Customer Churn Prediction

Predict whether a customer is likely to churn using their service, billing, and demographic data.  
Built with 💡 Logistic Regression, 🌲 Random Forest, and ⚡ XGBoost.

---

## 🎯 Problem Statement

Churn directly impacts revenue in telecom companies. This project helps predict which customers are at risk of leaving, enabling proactive retention strategies.

---

## 📁 Dataset

- **Source**: Kaggle – [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Rows**: 7032
- **Target Variable**: `Churn` (`Yes` / `No`)

---

## 🧰 Tech Stack

- **Languages**: Python  
- **Libraries**:  
  `pandas`, `scikit-learn`, `matplotlib`, `seaborn`, `xgboost`, `joblib`

---

## 🚀 Workflow

1. **Data Cleaning**  
   ✅ Drop `customerID`  
   ✅ Convert `TotalCharges` to numeric  
   ✅ Drop missing values  

2. **Preprocessing**  
   ✅ Binary encode `Yes/No` columns  
   ✅ One-hot encode remaining categorical features  
   ✅ Feature scaling using `StandardScaler`

3. **Model Training**  
   ✔ Logistic Regression  
   ✔ Random Forest  
   ✔ XGBoost

4. **Evaluation**  
   🔍 Accuracy, Confusion Matrix, Classification Report

5. **Model Export**  
   ✅ `xgboost_telco_model.pkl`  
   ✅ `scaler_telco.pkl`

---

## 📈 Results

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression| **78.75%** |
| Random Forest      | **78.18%** |
| ⚡ XGBoost          | **76.33%** |

> 🎉 Final model: **Logistic Regression** chosen based on precision and balance

---

## 🧪 Sample Output

```python
Predicted Churn: No
