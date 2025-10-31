# Insurance Expenses Prediction - README

## 1. Import Libraries
We use Python libraries like pandas, numpy, matplotlib, seaborn, and scikit-learn.  
These provide tools for handling data, visualization, preprocessing, and building models.

## 2. Load Data
The dataset (`insurance.csv`) is loaded and inspected for shape, types, and summary statistics.  
This step helps us understand the data before analysis.

## 3. Exploratory Data Analysis (EDA)
- Check for missing values  
- Visualize correlations  
- Compare smoker vs non-smoker expenses  
- Plot the distribution of expenses  

These steps help identify trends and risk factors.

## 4. Preprocessing
- Split features (X) and target (`y = expenses`)  
- Standardize numerical features  
- Encode categorical features  
- Split dataset into train/test sets  

This prepares the data for machine learning models.

## 5. Linear Regression (Baseline Model)
A linear regression model is trained and evaluated.  
It provides a quick, interpretable baseline for comparison.

## 6. Random Forest Regressor (Advanced Model)
A Random Forest model is trained to capture non-linear relationships.  
It usually performs better than linear regression.

## 7. Model Comparison
Both models are compared using metrics like **MSE, RMSE, MAE, and R²** to determine performance.

## 8. Feature Importance (Risk Factors)
Feature importance from Random Forest highlights that **smoker status, BMI, and age** are the biggest drivers of expenses.

## 9. Visualization: Actual vs Predicted
Scatter plots of actual vs predicted values show how close the model predictions are to reality.

## Conclusion
- Linear Regression is simple and interpretable  
- Random Forest provides better accuracy  
- Smoker status is the most important factor, followed by BMI and age  
- This workflow mirrors real ML projects, from problem definition to insights  
