# Student Academic Prediction — Decision Tree & Random Forest

This project demonstrates predicting student academic performance using decision trees and random forests. The analysis is contained in `student_academic_prediction_using_dt_and_rf.ipynb` and uses the provided `xAPI-Edu-Data.csv` dataset.

## Files

- `student_academic_prediction_using_dt_and_rf.ipynb` — Jupyter notebook with data exploration, preprocessing, model training (Decision Tree and Random Forest), and evaluation.
- `xAPI-Edu-Data.csv` — Dataset used in the notebook.

## Overview

Notebook workflow:

- Load and inspect the dataset
- Exploratory data analysis and visualizations
- Preprocessing and encoding categorical features
- Train/test split
- Train and compare `DecisionTreeClassifier` and `RandomForestClassifier`
- Evaluate using accuracy, confusion matrix, and feature importance

## Typical target

The notebook predicts a student performance/academic outcome column — check the notebook for the precise target column name.

## Dependencies

Install recommended packages with pip:

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

## How to run

1. Open `student_academic_prediction_using_dt_and_rf.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `xAPI-Edu-Data.csv` is in the same directory or upload it to Colab.
3. Run cells sequentially to reproduce preprocessing, training, and evaluation steps.

## Results

Model metrics (accuracy, confusion matrices) and feature importances are printed and visualized in the notebook. Re-run the notebook to reproduce results or adjust hyperparameters.

## Next steps (suggestions)

- Add a `requirements.txt` to pin dependency versions.
- Add cross-validation and GridSearchCV for hyperparameter tuning.
- Save trained models with `joblib` and add an inference script (`predict.py`).
- Compare models (e.g., XGBoost, LightGBM) and evaluate broader metrics (precision, recall, F1).

## License & Contact

This project is provided as-is. Tell me if you want a `requirements.txt`, a headless training script, or model export next.
