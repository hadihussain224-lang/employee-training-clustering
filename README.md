# Employee Training Outcomes — PCA & K-Means Clustering

Segments employees into motivation-based clusters using survey data,
then links those clusters to real training outcomes like completion
rate and skill proficiency gain.

## Overview

This project merges five related datasets — survey responses, employee
records, enrollment outcomes, and question metadata — into a single
analysis table. It then:

1. Extracts 12 motivation-related survey items
2. Standardizes them and runs **PCA** to reduce dimensionality
3. Applies **K-Means clustering** (k=3) on the top 3 principal components
4. Computes a `LearningGain` metric (outcome proficiency − intake proficiency) per employee
5. Summarizes each cluster's average motivation scores, completion rate, and learning gain

The result identifies distinct employee motivation profiles and how
they relate to training success.

## Tech stack

Python · pandas · scikit-learn (PCA, KMeans, StandardScaler)

## Files

| File | Description |
|---|---|
| `TerraNova_PCA_KMeans.ipynb` | Full analysis: merging, PCA, clustering, cluster summary |
| `Team_M4_*.csv` | Source survey, enrollment, and employee datasets |
| `Team M4 Executive Report.pdf` | Written findings and business recommendations |

## Running it

```bash
pip install pandas numpy scikit-learn
jupyter notebook TerraNova_PCA_KMeans.ipynb
```

## Author

Muhammad Hadi Hussain
