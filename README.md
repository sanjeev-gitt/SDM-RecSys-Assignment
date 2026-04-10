# Recommender Systems Assignment
## System Development for Marketing 
### Amsterdam University of Applied Sciences 2025/2026

Author: Sanjeev Dubey
Student ID: 500975381

## Notebooks

| Notebook | Dataset | Techniques |
|----------|---------|------------|
| MovieLens_RecSys.ipynb | MovieLens 1M | Technique A: SVD + SVD++ (bonus), Technique D: ItemKNN |
| Yelp_RecSys.ipynb | Yelp Academic Dataset | Technique B: Content UserKNN + ItemKNN, Technique C: Collab UserKNN |

## Results Summary

| Model | Dataset | RMSE |
|-------|---------|------|
| SVD | MovieLens | 1.0171 |
| SVD++ (bonus) | MovieLens | 0.8749 |
| ItemKNN | MovieLens | 0.9411 |
| Content ItemKNN | Yelp | 1.2088 |
| Content UserKNN | Yelp | 1.3403 |
| Collab UserKNN | Yelp | 1.3398 |

## Key Finding

Matrix sparsity determines which technique works.
At 94.93% sparsity (MovieLens), collaborative filtering via SVD++ excels.
At 99.99% sparsity (Yelp), content-based filtering is the only viable approach.

## Requirements

- Python 3.8+
- pandas, numpy, matplotlib, seaborn
- scikit-learn, scipy
- No Surprise library used
- All models implemented from scratch
