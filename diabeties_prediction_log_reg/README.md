# Diabetes Prediction — Logistic Regression

This project demonstrates building a logistic regression model to predict diabetes using the included dataset. The work is contained in a Jupyter notebook with data exploration, preprocessing, model training, and evaluation.

## Files

- `diabeties_log_reg.ipynb` — Jupyter notebook with end-to-end analysis and modeling.
- `diabetes.csv` — Dataset used in the notebook (Pima-type diabetes dataset).

## Overview

The notebook covers:

- Loading and inspecting the dataset
- Exploratory data analysis and basic visualizations
- Preprocessing (e.g., handling missing/zero values, feature scaling)
- Train/test split
- Train a Logistic Regression classifier and evaluate performance
- Print and visualize key metrics (accuracy, confusion matrix)

Target variable: `Outcome` (0 = no diabetes, 1 = diabetes)

## Dataset columns (typical)

- `Pregnancies` — Number of times pregnant
- `Glucose` — Plasma glucose concentration
- `BloodPressure` — Diastolic blood pressure (mm Hg)
- `SkinThickness` — Triceps skin fold thickness (mm)
- `Insulin` — 2-Hour serum insulin (mu U/ml)
- `BMI` — Body mass index (weight in kg/(height in m)^2)
- `DiabetesPedigreeFunction` — Diabetes pedigree function
- `Age` — Age in years
- `Outcome` — Target (0 or 1)

## Dependencies

Recommended packages (install via pip):

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

## How to run

1. Open `diabeties_log_reg.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `diabetes.csv` is in the same directory or upload it in Colab.
3. Run cells sequentially. Some preprocessing steps may assume zeros indicate missing values; review and adjust as needed.

## Results

Model performance (accuracy and confusion matrix) is printed in the notebook after training. Re-run the notebook to reproduce results or tune hyperparameters.

## Next steps (suggestions)

- Add a `requirements.txt` to pin versions.
- Add cross-validation and hyperparameter tuning (e.g., regularization strength).
- Try additional models (Random Forest, SVM) and compare metrics (precision, recall, F1).
- Add a small script `train.py` to run preprocessing and training headlessly.

## License & Contact

This repository is provided as-is. If you'd like I can add `requirements.txt`, add a headless training script, or run the notebook and report exact metrics.
