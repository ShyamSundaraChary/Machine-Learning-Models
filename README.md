# Machine Learning Models

This repository contains a small collection of machine learning example projects and notebooks that I completed. Each top-level folder contains a dataset and an interactive Jupyter notebook showing the full analysis, modeling, and evaluation steps.

## Project structure

- `IsolationForest/`

  - `ecommerce_purchase_data.csv` — dataset used for anomaly detection.
  - `Isolation_Forest.ipynb` — notebook that demonstrates isolation forest for outlier detection on ecommerce purchases.

- `LinearRegreesion/` (note: folder name contains a minor spelling variation)

  - `insurance.csv` — insurance dataset (charges, age, BMI, etc.).
  - `LInear_Regression_GPP_44.ipynb` — notebook with exploratory data analysis, feature prep and linear regression models.
  - `insurance_readme.md` — dataset-specific notes.

- `Logistic Regression/`

  - `Titanic-Dataset.csv` — Titanic passenger data for classification.
  - `Logistic_Regression.ipynb` — notebook implementing logistic regression to predict survival.
  - `README.md` — any additional notes in that folder.

- `Regresion-1/`
  - `customer_satisfaction_data.csv` and `cleaned_customer_satisfaction_data.csv` — customer satisfaction datasets and cleaning output.
  - `Regression_1_ML.ipynb` — notebook exploring regression models on satisfaction scores.

## Highlights

- Demonstrated supervised learning (linear and logistic regression) and unsupervised anomaly detection (isolation forest).
- Each notebook contains: data loading, exploratory data analysis (visuals & statistics), preprocessing, model training, evaluation (metrics and plots), and short conclusions.

## How to run these notebooks (Windows — cmd.exe)

1. Open a Command Prompt and change to the repository root:

```bat
cd /d "C:\Users\shyam\Desktop\Machine Learning Models"
```

2. (Optional but recommended) Create and activate a Python virtual environment:

```bat
python -m venv .venv
.venv\Scripts\activate
```

3. Install dependencies:

```bat
pip install -r requirements.txt
```

4. Start a Jupyter server and open the notebooks in your browser:

```bat
jupyter notebook
```

Open any of the `.ipynb` files listed above and run the cells sequentially.

## Dependencies

Common libraries used across the notebooks are listed in `requirements.txt`. They include:

- Python 3.8+ (recommended)
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- jupyter

If you prefer manual install:

```bat
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```
