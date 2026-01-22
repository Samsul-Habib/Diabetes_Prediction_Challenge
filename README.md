# Diabetes Prediction – Kaggle Playground Series S5E12

## Overview
This project solves the Kaggle Playground Series Season 5 Episode 12 competition, which focuses on predicting the probability of a patient being diabetic using structured health-related data. The solution follows a clear machine learning workflow from data preparation to model training and evaluation.

Final Kaggle Score: 0.69636

---

## Dataset
The competition provides:
- train.csv – training data with labels
- test.csv – test data without labels
- sample_submission.csv – submission format

Target column:
- diabetes (0 or 1)

---

## Methodology

### Data Analysis
- Checked data shape and feature types
- Verified class distribution
- Confirmed absence of critical missing values

### Preprocessing
- Separated features and target
- Split data into training and validation sets
- Prepared data for tree-based models

### Models Tested
- Random Forest
- XGBoost
- LightGBM

LightGBM showed the best validation performance.

---

## Hyperparameter Tuning
- Used Optuna for parameter search
- Optimized LightGBM parameters including depth, learning rate, and number of trees
- Selected model based on validation ROC-AUC

---

## Evaluation
Metrics used:
- ROC-AUC

The final model generalizes well to unseen data.

---

## Final Model
- Algorithm: LightGBM Classifier
- Tuning: Optuna
- Kaggle Public Score: 0.69636

---

## Repository Structure

---

## How to Run
1. Clone the repository
```bash
git clone https://github.com/Samsul-Habib/Diabetes_Prediction_Challenge.git
```

2. Create virtual environment
```bash
python -m venv my_env
```

3. Activate the environment
```bash
my_env\Scripts\activate
```

4. Install dependencies
```bash
pip install numpy pandas scikit-learn lightgbm xgboost catboost optuna matplotlib seaborn
```

5. Open VS code
```bash
code .
```

6. Select the kernel and run the notebook cells.
