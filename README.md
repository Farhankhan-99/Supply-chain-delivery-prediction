# Supply Chain Delivery Delay Prediction

## 🎯 Problem Statement

Late deliveries increase operational costs and reduce customer satisfaction.  
This project builds a machine learning model to predict whether a shipment will be delivered late or on time using historical logistics data.

---

## 📌 Project Overview

An end-to-end ML pipeline was developed including preprocessing, EDA, model building, hyperparameter tuning, and evaluation.  
The objective is to proactively identify high-risk shipments and support better logistics decision-making.

---

## 📊 Key EDA Insights

- ~60% of orders are delayed, indicating moderate class imbalance.  
- Delay rates are consistent across shipping modes (~59–60%).  
- Warehouses show similar delay patterns, suggesting systemic inefficiencies.  
- High-priority products have the highest delay rate (65%).  

---

## 🤖 Model & Evaluation

Models implemented:
- Logistic Regression  
- Decision Tree  
- Random Forest  

Pipelines were used to prevent data leakage.  
Models were evaluated using Accuracy, Precision, Recall, F1-score, and ROC-AUC.

Random Forest performed best and was selected as the final model.

---

## ⚙️ Hyperparameter Tuning

GridSearchCV with cross-validation was used to optimize Random Forest parameters, improving model stability and generalization.

---

## 🚀 Future Improvements

- Implement XGBoost / LightGBM  
- Apply SMOTE for imbalance handling  
- Deploy via Flask or FastAPI  
- Build dashboard using Streamlit / Power BI  

---

## 🛠️ Tech Stack

Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn
