# User Product Purchase Prediction — Logistic Regression
# Problem statement

This project demonstrates a logistic regression approach to predict whether a user will purchase a product based on demographic and usage features. The analysis is contained in the Jupyter notebook and uses the included `User_Data.csv` dataset.

## Files

- `user_product_purchase_prediction_using_logistic_regression.ipynb` — Jupyter notebook with data exploration, preprocessing, model training, and evaluation.
- `User_Data.csv` — Dataset used in the notebook.

## Overview

Notebook workflow:

- Load and inspect the dataset
- Exploratory data analysis and visualizations
- Preprocessing (encoding categorical features, scaling if needed)
- Train/test split
- Train a Logistic Regression classifier and evaluate using accuracy and a confusion matrix
- Analyze feature importance / coefficients to interpret model

Typical target: a binary column indicating purchase (0 = no purchase, 1 = purchase). Check the notebook for the exact column name used.

## Dependencies

Recommended packages (install via pip):

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

## How to run

1. Open `user_product_purchase_prediction_using_logistic_regression.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `User_Data.csv` is in the same directory or upload it to Colab.
3. Run cells sequentially to reproduce preprocessing, training, and evaluation steps.

## Results

Model accuracy and the confusion matrix are printed in the notebook after training. Re-run the notebook to reproduce results or tune preprocessing and hyperparameters.

