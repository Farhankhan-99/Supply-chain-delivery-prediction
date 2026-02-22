# Supply Chain Delivery Delay Prediction

## Problem Statement

Late deliveries in supply chain operations increase operational costs and reduce customer satisfaction.  
The objective of this project is to build a machine learning model that predicts whether an order will be delivered late or on time using historical shipment data.

---

## Project Overview

This project implements an end-to-end machine learning workflow including data preprocessing, exploratory analysis, model development, hyperparameter tuning, and performance evaluation.  
The goal is to identify high-risk shipments in advance and support better logistics planning decisions.

---

## Exploratory Data Analysis (EDA) – Key Insights

Approximately 60% of the orders in the dataset are delayed, indicating moderate class imbalance.  
Delay rates are consistent across shipping modes (~59–60%), suggesting transportation type alone does not significantly impact delivery performance.  
Warehouse-level delay percentages are also similar (~59–60%), indicating systemic operational inefficiencies rather than location-specific issues.  
High-importance products show the highest delay rate (65%), which highlights potential prioritization or process gaps.  
Overall, delays appear to be influenced by multiple combined factors rather than a single dominant variable.

---

## Model Development and Evaluation

Three classification models were implemented:

- Logistic Regression (baseline)
- Decision Tree
- Random Forest

Data preprocessing was handled using ColumnTransformer with encoding and scaling, integrated into Scikit-learn pipelines to prevent data leakage.  
Model performance was evaluated using Accuracy, Precision, Recall, F1-score, and ROC-AUC.

Random Forest achieved the best overall performance and was selected as the final model due to stronger generalization and balanced classification metrics.

---

## Hyperparameter Tuning

Random Forest hyperparameters were optimized using GridSearchCV with cross-validation to improve robustness and reduce overfitting.  
The tuned model showed improved stability and predictive performance compared to default settings.

---

## Conclusion

The final model successfully predicts delivery delays with strong classification performance.  
This solution can be used to flag high-risk shipments before dispatch, enabling proactive logistics adjustments and improved service reliability.

---

## Future Improvements

- Implement XGBoost or LightGBM for performance comparison  
- Apply advanced imbalance handling techniques such as SMOTE  
- Deploy the model using Flask or FastAPI  
- Build a monitoring dashboard using Streamlit or Power BI  

---

## Technologies Used

Python  
Pandas  
NumPy  
Scikit-learn  
Matplotlib  
Seaborn  
