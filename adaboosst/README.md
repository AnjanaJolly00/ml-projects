# AdaBoost Employee Attrition Prediction

This small project demonstrates using AdaBoost (with a decision tree base estimator) to predict employee attrition (whether an employee leaves). The analysis and modeling are contained in the Jupyter notebook and use the included HR dataset.

## Files

- `adaboost.ipynb` — Jupyter notebook with data exploration, preprocessing, model selection (GridSearchCV), model training, and evaluation.
- `HR_comma_sep.csv` — HR dataset used in the notebook.

## Overview

The notebook performs the following steps:

- Load and inspect the dataset
- Basic exploratory data analysis and visualization
- One-hot encoding for categorical features
- Split data into training and test sets
- Use `GridSearchCV` to tune `n_estimators` for `AdaBoostClassifier` (base estimator: `DecisionTreeClassifier`)
- Train final AdaBoost model and evaluate accuracy on train/test splits

Key modeled target: `left` (0 = stayed, 1 = left)

## Dataset notes

Columns include (as used in the notebook):

- `satisfaction_level` — value between 0 and 1
- `last_evaluation` — value between 0 and 1
- `number_project` — number of projects
- `average_monthly_hours` — avg hours per month
- `time_spend_company` — years in company
- `Work_accident` — 0/1
- `promotion_last_5years` — 0/1
- `left` — 0/1 (target)

## Dependencies

Recommended Python packages (install with pip):

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn plotly
```

Or create a `requirements.txt` with the above packages.

## How to run

1. Open `adaboost.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `HR_comma_sep.csv` is available in the same directory (or upload it in Colab where the notebook expects it).
3. Run cells sequentially. The notebook includes a `GridSearchCV` step which may take a few minutes depending on your machine.

If using Google Colab, the notebook includes a cell that uploads local files; use that to upload `HR_comma_sep.csv`.

## Results

Model performance (accuracy) is printed in the notebook after training. Re-run the notebook to reproduce results or modify hyperparameters in the GridSearch section.

## Next steps (suggestions)

- Add a `requirements.txt` to pin dependency versions.
- Add a small unit test or a script to run training/evaluation headlessly (e.g., `train.py`).
- Explore additional metrics (precision, recall, F1) and class imbalance handling.

## License & Contact

This project is provided as-is. If you'd like any improvements or want me to add a `requirements.txt` or run the notebook and report exact metrics, tell me and I will proceed.
