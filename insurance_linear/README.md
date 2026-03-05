# Insurance Charges Prediction — Linear Regression

This project demonstrates using linear regression to predict insurance charges based on demographic and health-related features. The analysis and modeling are contained in the `insurance_linear_reg.ipynb` notebook and use the included `insurance.csv` dataset.

## Files

- `insurance_linear_reg.ipynb` — Jupyter notebook with data exploration, preprocessing, model building, and evaluation.
- `insurance.csv` — Dataset used in the notebook.

## Overview

The notebook covers the typical supervised regression workflow:

- Load and inspect the dataset
- Exploratory data analysis and visualizations
- Preprocessing (encoding categorical variables, feature scaling as needed)
- Train/test split
- Train a Linear Regression model and evaluate using metrics like MAE, MSE, and R²

Typical target column: `charges` (insurance cost)

## Dataset columns (typical)

- `age` — Age of primary beneficiary
- `sex` — Gender
- `bmi` — Body mass index
- `children` — Number of children covered by health insurance
- `smoker` — Whether the person smokes (yes/no)
- `region` — Residential area in the US
- `charges` — Individual medical costs billed by health insurance (target)

## Dependencies

Recommended packages (install with pip):

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

## How to run

1. Open `insurance_linear_reg.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `insurance.csv` is in the same directory or upload it to Colab.
3. Run cells sequentially to reproduce preprocessing, training, and evaluation steps.

## Results

Model metrics (MAE, MSE, R²) are printed in the notebook after training. Re-run the notebook to reproduce results or try different feature-engineering steps.

## Next steps (suggestions)

- Add a `requirements.txt` to pin dependency versions.
- Evaluate with cross-validation and try regularized models (Ridge, Lasso).
- Create a headless `train.py` script to train and save the model with `joblib`.
- Add error analysis and plots of residuals to check assumptions of linear regression.

## License & Contact

This repository is provided as-is. If you'd like, I can add `requirements.txt`, implement `train.py`, or run the notebook and report exact metrics.
