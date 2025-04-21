# Cardiovascular Disease Prediction

This repository contains a machine learning pipeline to predict the presence of cardiovascular disease using clinical and biometric data. The project walks through data cleaning, exploration, model training, evaluation, and visualization to build a deployable disease prediction system.

## Problem Statement

Cardiovascular diseases (CVDs) are the leading cause of death globally, often due to delayed diagnosis. Early risk detection can significantly improve outcomes and reduce strain on healthcare systems.

This project uses patient data (age, blood pressure, cholesterol, etc.) to predict CVD presence using supervised learning models. The goal is to develop models that are both accurate and interpretable to assist healthcare professionals in early risk assessment.

## Dataset

- **Source**: [Kaggle – Cardiovascular Disease Dataset](https://www.kaggle.com/datasets/somyang2711/cardiovascular-disease-dataset)
- **Records**: ~70,000 patients
- **Features**: Age, Gender, Blood Pressure, Cholesterol, Glucose, Lifestyle habits
- **Target**: Presence of cardiovascular disease (`0` = No, `1` = Yes)

## Project Workflow

### 1. Data Cleaning & Preprocessing
- Removed incorrect values (e.g. height/weight outliers)
- Encoded categorical variables
- Scaled features where necessary

### 2. Exploratory Data Analysis (EDA)
- Class distributions by gender, age, cholesterol, and activity
- Correlation heatmap and boxplots for feature relationships
- Distribution plots of key risk factors

### 3. Machine Learning Models
- **Logistic Regression**
- **Random Forest**
- **XGBoost**

All models were trained on a balanced and cleaned dataset.

### 4. Evaluation
- **Metrics Used**:
  - Accuracy, Precision, Recall, F1-Score
  - ROC-AUC and PR-AUC
- **Visualizations**:
  - Confusion Matrices
  - ROC Curves
  - Precision-Recall Curves
  - Feature Importance (for RF & XGBoost)

## Final Conclusion

This project demonstrates that machine learning can effectively predict cardiovascular disease risk using readily available patient data. 

- **XGBoost** achieved the best overall performance in ROC-AUC and PR-AUC.
- **Random Forest** balanced performance and interpretability well.
- **Logistic Regression** provided a solid, interpretable baseline.

With further tuning and validation on external datasets, this model could serve as a decision-support tool in preventive healthcare.

## Technologies Used

- Python
- Jupyter Notebook
- pandas, numpy, seaborn, matplotlib
- scikit-learn
- XGBoost

## Getting Started

To run the project locally:

```bash
git clone https://github.com/your-username/cardiovascular-disease-prediction.git
