# CS_TASK3
# 📉 Customer Churn Prediction using Machine Learning

This project is part of my **CodSoft ML Internship**. The goal is to develop a machine learning model to predict whether a customer is likely to **churn** (leave a service) based on historical usage and demographic data.

---

## 📌 Objective

To analyze customer data and build a classification model that can **predict churn** so businesses can proactively retain their customers.

---

## 📁 Dataset

- Source: `Churn_Modelling.csv` (from Kaggle) https://www.kaggle.com/datasets/aakash50897/churn-modellingcsv
- Total records: 10,000 bank customers
- Key features:
  - `CreditScore`, `Geography`, `Gender`, `Age`, `Balance`
  - `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`
- Target column: `Exited`
  - `0` → Stayed
  - `1` → Churned

---

## ⚙️ ML Workflow

1. **Data Preprocessing**
   - Removed irrelevant columns: `RowNumber`, `CustomerId`, `Surname`
   - Encoded categorical features: `Gender`, `Geography`
   - Split data into training and testing sets

2. **Model Training**
   - **Logistic Regression**
   - **Random Forest Classifier**
   - **Gradient Boosting Classifier**

3. **Model Evaluation**
   - Accuracy Score
   - Precision, Recall, F1-Score
   - Confusion Matrix (via heatmap)

---

## 📊 Results

| Model                | Accuracy | Recall (Churn) | F1-Score |
|---------------------|----------|----------------|----------|
| Logistic Regression | 80.15%   | Low            | Low      |
| Random Forest       | 86.60%   | Medium         | Medium   |
| Gradient Boosting   | **86.75%** | **High**        | **Best**  |

🎯 **Gradient Boosting Classifier** gave the best balance of accuracy and recall, making it the best choice for detecting churned customers.

---

## 📌 Tools & Libraries

- Python 🐍  
- Jupyter Notebook  
- pandas, numpy  
- scikit-learn  
- matplotlib, seaborn

---

## 📷 Sample Visuals

- Accuracy Comparison Bar Chart  
- Confusion Matrix Heatmap  
- Feature importance (optional)

---

## 💡 Learnings

- Learned the end-to-end flow of a supervised classification problem  
- Understood the importance of **recall** in churn use-cases  
- Got hands-on with **Gradient Boosting** and real-world data encoding

---

## 🚀 Future Enhancements

- Hyperparameter tuning using GridSearchCV  
- Use SMOTE to handle slight imbalance in churn class  
- Build a frontend to input new customer details for live predictions

---

---


