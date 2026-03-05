# K-Means Customer Clustering

This project contains examples of K-Means clustering applied to customer datasets. The notebooks demonstrate data exploration, feature preparation, cluster analysis, and visualization to discover customer segments.

## Files

- `kmeans_clustering.ipynb` — General K-Means notebook demonstrating clustering techniques.
- `kmeans_customer_clustering.ipynb` — Customer segmentation workflow using `Mall_Customers.csv` or `Live.csv`.
- `Mall_Customers.csv` — Customer dataset commonly used for clustering examples.
- `Live.csv` — Additional dataset included for experiments.

## Overview

Typical workflow in the notebooks:

- Load dataset and inspect basic statistics
- Preprocess features (scaling, selecting numeric features)
- Use the elbow method or silhouette score to choose `k`
- Fit `KMeans` and analyze cluster centroids
- Visualize clusters using 2D plots (PCA or feature pairs)

## Dependencies

Install recommended packages with pip:

```
pip install jupyterlab pandas numpy scikit-learn matplotlib seaborn
```

## How to run

1. Open either notebook in JupyterLab/Jupyter Notebook or Google Colab.
2. Ensure the chosen CSV (`Mall_Customers.csv` or `Live.csv`) is in the same directory or upload it to Colab.
3. Run cells sequentially. The elbow and silhouette computations are fast for these small datasets.

## Next steps (suggestions)

- Add a `requirements.txt` to pin dependency versions.
- Add a `notebooks/` README section explaining which notebook to run for which dataset.
- Export cluster assignments to CSV and add a small `cluster_analysis.py` script for headless processing.
- Compare K-Means with other clustering algorithms (DBSCAN, Agglomerative) and include silhouette/Rand index comparisons.

## License & Contact

This project is provided as-is. Tell me if you want a `requirements.txt`, exported cluster CSVs, or a headless script created next.
