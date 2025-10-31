# Detecting Outliers in Customer Purchase Behavior

## Objective

This project aims to identify outliers in customer purchase behavior using the Isolation Forest algorithm on an e-commerce dataset.

The goal is to uncover patterns in anomalous customer data and derive actionable business insights.

## Dataset

The dataset used is `ecommerce_purchase_data.csv`, which contains transactional and demographic information for 3000 customers.

## Methodology

1.  **Data Preprocessing**:

    - Missing numerical values were filled using the **median**.
    - Missing categorical values were filled using the **mode**.
    - The `LastPurchaseDate` was converted into a `DaysSinceLastPurchase` feature to quantify recency.
    - Categorical features (`Gender`, `ProductCategory`) were one-hot encoded for model compatibility.

2.  **Outlier Detection**:

    - An **Isolation Forest** model was applied to the preprocessed dataset to flag anomalous entries. Customers marked as outliers represent approximately 5% of the data.

3.  **Analysis & Visualization**:

    - The characteristics of the outlier group were compared against the inlier group using descriptive statistics.
    - Scatter plots were used to visualize the differences, primarily focusing on `PurchaseAmount` vs. `AnnualIncome` and `PurchaseFrequency`.

## Key Findings

The analysis revealed that customers identified as outliers typically exhibit:

- **Higher Purchase Amounts**: They spend significantly more per transaction.
- **Lower Purchase Frequency**: They make purchases less often than typical customers.
- **Longer Time Since Last Purchase**: They are less recent customers on average.

## Business Insights

- **VIP Customers**: Outliers with high spending are valuable VIPs who should be nurtured with exclusive offers.
- **Churn Risk**: Infrequent purchasers who haven't shopped in a while are potential churn risks and should be targeted with re-engagement campaigns.
- **Data Integrity**: Anomalous patterns (e.g., low income with very high spending) may indicate data errors or fraudulent activity that needs investigation.

## How to Run

1.  **Dependencies**: Ensure the following Python libraries are installed:
    ```bash
    pip install pandas scikit-learn matplotlib seaborn
    ```
2.  **Execution**:
    - Place the Jupyter notebook and the `ecommerce_purchase_data.csv` file in the same directory.
    - Run all cells in the notebook sequentially to reproduce the analysis and visualizations.
