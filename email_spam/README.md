# Email Spam Detection — Logistic Regression

This project implements a simple email spam detection pipeline using logistic regression. The analysis, preprocessing, feature extraction, model training, and evaluation are included in the Jupyter notebook.

## Files

- `email_spam_detection_using_logistic_regression.ipynb` — Jupyter notebook with end-to-end workflow.
- `spam.csv` — Dataset used by the notebook (raw email text and labels).

## Overview

The notebook demonstrates:

- Loading and inspecting the spam dataset
- Text preprocessing and feature extraction (e.g., CountVectorizer or TF-IDF)
- Train/test split
- Train a Logistic Regression classifier and evaluate with accuracy and confusion matrix
- Basic visualizations and analysis of most informative features

Target variable: label indicating `spam` vs `ham` (check the notebook for the exact column name used).

## Dependencies

Recommended packages:

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

If the notebook uses NLTK or other NLP helpers, also install:

```
pip install nltk
```

## How to run

1. Open `email_spam_detection_using_logistic_regression.ipynb` in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure `spam.csv` is available in the same directory or uploaded to Colab.
3. Run cells sequentially. Feature extraction steps may take a short time depending on dataset size.

## Results

Model accuracy and a confusion matrix are printed in the notebook after training. Re-run the notebook to reproduce or tune hyperparameters (e.g., regularization strength, vectorizer parameters).

## Next steps (suggestions)

- Add a `requirements.txt` to lock dependency versions.
- Add text-cleaning steps (stopword removal, lemmatization) and compare results.
- Try additional models (Naive Bayes, Random Forest, SVM) and evaluate precision/recall/F1 for the `spam` class.
- Export a trained model with `joblib` and add a small inference script `predict_spam.py`.

## License & Contact

This repository is provided as-is. If you want, I can add `requirements.txt`, create a headless training script, or export the trained model.
