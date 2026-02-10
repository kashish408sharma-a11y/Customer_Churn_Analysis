# 📊 Customer Churn Analysis & Prediction

## 📌 Project Overview
This project focuses on analyzing and predicting customer churn using Logistic Regression
and presenting insights through an interactive Power BI dashboard.
The goal is to understand why customers churn, identify high-risk customers,
and translate machine learning outputs into business-ready insights.

---

## 🎯 Project Objectives
- Predict customer churn using machine learning
- Identify key churn drivers
- Segment customers by churn risk
- Build an interpretable Power BI dashboard

---

## 🧠 Skills & Concepts Learned
- End-to-end churn analysis workflow
- Data cleaning and preprocessing
- One-Hot Encoding using get_dummies
- Feature scaling
- Logistic Regression for binary classification
- Model evaluation beyond accuracy
- Probability-based prediction and threshold tuning
- Feature importance interpretation
- Power BI dashboarding with DAX
- Business storytelling with data

---

## ⚙️ Data Preparation
- Converted categorical variables using One-Hot Encoding
- Binary mapping for Yes/No fields
- Scaled numerical features:
  - tenure
  - MonthlyCharges
  - TotalCharges

---

## 🤖 Machine Learning Model
- Algorithm: Logistic Regression
- Chosen because:
  - Suitable for binary classification
  - Interpretable coefficients
  - Explains impact of each feature on churn

### Target Variable
- Churn_num
  - 1 → Customer churned
  - 0 → Customer retained

---

## 🧪 Model Evaluation
The model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The prediction threshold was adjusted to 0.35
to improve churner detection.

---

## 📈 Prediction Outputs
- churn_probability → Probability of churn
- churn_risk_score → Risk score (0–100)
- risk_segment → Low / Medium / High
- churn_segment → Model-based churn category

Note:
Even for already churned customers, probabilities represent model confidence.

---

## 🔴 Key Churn Drivers (Feature Importance)
Extracted from Logistic Regression coefficients.

Top factors increasing churn:
- Fiber optic internet
- Senior citizen
- Electronic check payment method
- Higher monthly charges
- Tenure (weak effect)

Positive coefficients indicate higher churn likelihood.

---

## 📊 Power BI Dashboard
Dashboard includes:
1. Churn Overview KPIs
2. Top 5 Churn Drivers (Feature Importance)
3. Customer Risk Segmentation
4. High-Risk Customer Insights

Power BI techniques used:
- DAX SWITCH() measures
- Custom churn driver dimension table
- Top-N filtering
- Business-friendly visual design

---

## 🛠 Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn)
- Logistic Regression
- Power BI
- DAX
- Jupyter Notebook

---

## 🚀 How to Use
1. Run the Python notebook to clean data and train the model
2. Generate churn probabilities and risk scores
3. Load the processed dataset into Power BI
4. Build visuals using provided DAX measures

---

## 📌 Key Insight
Customers using fiber optic internet, senior citizens,
and those paying via electronic checks show the highest churn risk.
Higher monthly charges increase churn probability,
while longer tenure slightly reduces churn risk.



