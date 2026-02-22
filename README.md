# Supply Chain Delivery Delay Prediction

## 🎯 Problem Statement

Late deliveries increase operational costs and reduce customer dissatisfaction.  
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
- High-priority products show the highest delay rate (65%).  

---

## 🤖 Model & Evaluation

Models implemented:
- Logistic Regression  
- Decision Tree  
- Random Forest  

Random Forest delivered the best overall performance.

**Final Model Performance (Random Forest):**

- Test Accuracy: **68.0%**
- Train Accuracy: **72.7%**
- Best Cross-Validation Score: **68.19%**
- Class 0 Recall: **0.94**
- Class 1 Recall: **0.50**
- Weighted F1-Score: **0.67**

The model shows reasonable generalization with limited overfitting. While it performs strongly in identifying on-time deliveries, recall for delayed shipments can be further improved.

---

## ⚙️ Hyperparameter Tuning

GridSearchCV with cross-validation was used to optimize Random Forest parameters, improving stability and generalization compared to default settings.

---

## 🚀 Future Improvements

- Improve recall for delayed shipments using SMOTE or class weighting  
- Experiment with XGBoost / LightGBM  
- Threshold tuning for better precision-recall balance  
- Deploy using Flask or FastAPI  
- Build monitoring dashboard using Streamlit or Power BI  

---

## 🛠️ Tech Stack

Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn
