# Customer Satisfaction Index (CSI) Prediction - Conclusion

## 📌 Project Overview

The objective of this project was to predict the **Customer Satisfaction
Index (CSI)** using survey data that included features such as product
category, purchase amount, customer demographics, delivery speed, and
customer service interactions.

## 📊 Model Results

We applied multiple regression models (Linear Regression, Random Forest,
XGBoost) and evaluated them using **MAE, RMSE, and R²** metrics.\

- The results showed **poor performance with negative R² values**,
  indicating that the models performed worse than simply predicting the
  average CSI.

## 🔎 Feature Analysis

- To understand this behavior, we analyzed feature-target relationships
  using **correlation analysis** and **feature importance (Random
  Forest)**.

- The results revealed that: - **Customer Age (0.24)**,
  **Purchase Amount (0.19)**, and **Log Purchase (0.19)** had the highest
  influence on CSI. - Features such as **Gender, Product Category, and
  Service Flags (Good/Poor Service)** contributed almost nothing to
  predicting CSI.
- This indicates that the dataset does not capture the
  true drivers of customer satisfaction.

## ✅ Key Findings

1.  CSI values in this dataset show **weak or no correlation** with most
    available features.\
2.  Customer satisfaction is likely influenced by **other hidden
    factors** (e.g., product quality, promotions, real service
    experience) that are not present in the dataset.\
3.  As a result, machine learning models cannot make accurate
    predictions with the current data.

## 🏁 Final Remark

While this dataset was useful for demonstrating the **end-to-end machine
learning process** (EDA, preprocessing, feature engineering, and model
training), it is **not sufficient for building a reliable CSI prediction
model**.\
For better performance, future work should include more relevant
features such as textual feedback, detailed service ratings, and support
interaction quality.
