# Graph ML for movie recommendations

## Project Description

This project explores the use of Graph Machine Learning to improve movie recommendation systems. We apply two graph neural network models - LightGCN and Neural Graph Collaborative Filtering (NGCF) - to the MovieLens 25M dataset. By treating users and movies as a connected network, these models can uncover deeper patterns in user preferences. We compare the two approaches to see whether a simpler, more efficient model performs better than a more complex one. 

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

## Structure of `main` branch

```
movie-recommendations/
├── models/
│   ├── best_ngcf_e4.pth         # NGCF trained models
│   └── best_ngcf_e5.pth
├── ngcf.ipynb                   # Code with training and testing the NGCF model
├── data-preprocessing.ipynb     # Main preprocessing pipeline
├── eda.ipynb                    # Exploratory data analysis
├── preprocessed_data/           # Generated processed data
│   ├── train_matrix.npz         # Matrix of interactions for training
│   ├── test_matrix.npz          # Quality assessment matrix
│   └── adj_matrix.npz           # Graph adjacency matrix
└── README.md
```