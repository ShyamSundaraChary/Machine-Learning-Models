# Titanic Survival Prediction - Logistic Regression

This project builds a **Logistic Regression model** on the Titanic dataset to predict whether a passenger survived or not.

## Steps Followed

### 1. Import Libraries
- Imported necessary libraries like pandas, numpy, matplotlib, seaborn, and scikit-learn for data handling, visualization, and modeling.

### 2. Load Dataset
- Loaded the Titanic dataset into a pandas DataFrame.

### 3. Explore Data
- Checked the shape of the dataset, datatypes, and missing values.

### 4. Handle Missing Values
- Filled missing `Age` values with the median.  
- Filled missing `Embarked` values with the mode (most frequent).  
- Dropped the `Cabin` column since it had too many missing values.  

### 5. Encode Categorical Data
- Converted `Sex` into numeric values (male=0, female=1).  
- Encoded `Embarked` using LabelEncoder.  

### 6. Select Features and Target
- Target variable: `Survived`.  
- Selected useful features: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`.  

### 7. Train-Test Split
- Split the dataset into training (80%) and testing (20%) sets.  

### 8. Build Model
- Trained a Logistic Regression model on the training data.  

### 9. Evaluate Model
- Checked model accuracy.  
- Plotted a confusion matrix.  
- Printed a classification report (precision, recall, f1-score).  

## Conclusion
- Logistic Regression provides a simple baseline model for predicting Titanic survival.  
- Further improvements can be made with feature engineering and advanced models, but this project focuses on the basics.  
