# Hotspots detection with unsupervised ML
The task at hand is to detect hotspots for Uber pickup in NY to better help drivers be where they are needed.

## The data

The dataset is obtained from the [Uber Pickups in New York City dataset](https://www.kaggle.com/datasets/fivethirtyeight/uber-pickups-in-new-york-city) on Kaggle, and focuses on the month of May 2014.

## Clustering
Ouliers are initially removed using DBScan. Hotspots are then determined using KMeans on 9 centroids.
The ideal number of centroids is based on the evaluation of the silhoutte score and inertia score of KMeans models train on different number of clusters.
The clusters are determined on an hour-by-hour and day-by-day basis.

## Data display
Clusters are displayed on an interactive Plotly graph


<img width="564" alt="Untitled" src="https://user-images.githubusercontent.com/49685784/169396712-505ae7cd-652d-43ba-88a4-720277e7185d.png">
