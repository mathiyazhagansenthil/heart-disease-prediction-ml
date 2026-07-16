# Heart Disease Prediction

Predicts whether a patient has heart disease based on health metrics 
(age, cholesterol, blood pressure, chest pain type, etc.) using machine learning.

## Dataset
UCI Heart Disease dataset (from Kaggle)

## What I did
- Explored the data and checked correlations between features
- Trained a model to predict heart disease presence
- Evaluated using accuracy and confusion matrix

## Tech used
Python, pandas, scikit-learn, seaborn/matplotlib

## How to run
Open Main.ipynb in Jupyter and run all cells.

## Results
Compared 6 models: Random Forest, Gradient Boosting, Naive Bayes, KNN, Logistic Regression, SVM

Best model: Random Forest (tuned with GridSearchCV)
- Accuracy: 98.5%
- Recall: 98.6%
- ROC-AUC: 0.999

Also analyzed feature importance to identify which health metrics matter most.

## Methodology
- Split models into scale-sensitive (KNN, Logistic Regression, SVM — used StandardScaler) 
  and scale-insensitive (tree-based models) groups
- Used GridSearchCV for hyperparameter tuning on Random Forest
- Evaluated using accuracy, recall, and ROC-AUC (recall prioritized since 
  missing a true heart disease case is costlier than a false alarm)

  <img width="607" height="453" alt="download" src="https://github.com/user-attachments/assets/e9612568-4016-4c7a-9c4f-665df8daca66" />

