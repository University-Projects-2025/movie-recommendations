# MovieLens Data Processing Pipeline

## Dataset

[MovieLens 25M](https://grouplens.org/datasets/movielens/25m/)

## Dataset Summary

| Metric | Value |
|--------|-------|
| Total Users | 162,541 |
| Total Movies | 59,047 |
| Total Ratings | 25,000,095 |
| Average Rating | 3.53 |
| Data Period | 1995-01-09 to 2019-11-21 |

## Structure of `data-process` branch

```
movie-recommendations/
├── data-preprocessing.ipynb     # Main preprocessing pipeline
├── eda.ipynb                    # Exploratory data analysis
├── preprocessed_data/           # Generated processed data
│   ├── train_matrix.npz         # Matrix of interactions for training
│   ├── test_matrix.npz          # Quality assessment matrix
│   └── adj_matrix.npz           # Graph adjacency matrix
└── README.md
```