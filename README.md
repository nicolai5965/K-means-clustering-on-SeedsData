# Seed Dataset Clustering
This repository contains a Python implementation of the K-means clustering algorithm to classify seeds based on their features using the seed dataset. The code also includes Principal Component Analysis (PCA) for visualization purposes.

## Data Preparation
The dataset is loaded from a text file using NumPy, and the feature data and labels are separated. The features are then normalized using z-score normalization.

## K-means Clustering Algorithm
The K-means clustering algorithm is implemented using the following functions:

* init_centroids(): Initializes the centroids randomly from the data.
* assign_clusters(): Assigns each data point to the nearest centroid.
* update_centroids(): Updates the centroids based on the mean of the data points in the cluster.
* k_means_clustering(): Performs the K-means clustering algorithm for a given number of iterations.

## Optimal Number of Clusters (K)
The Elbow Method is used to find the optimal number of clusters (K) by calculating the inertia for different values of K and plotting the resulting graph. The optimal K is determined based on the point where the rate of change in inertia starts to decrease.

## PCA for Visualization
PCA is performed on the dataset using the perform_pca() function to reduce the dimensionality of the data for visualization purposes. The data is then transformed to a 2D representation using the transform_data() function.

## Results Visualization
The clustered data points are plotted in 2D using the first two principal components as the axes. Different colors are used to represent the different clusters.

## Evaluation
The Adjusted Rand Index (ARI) is calculated to evaluate the clustering performance against the true labels of the dataset. A higher ARI indicates better clustering performance.

## Usage
To use this code, run the provided Python script in Google Colab. Ensure that you have the required libraries installed, including NumPy, matplotlib, and scikit-learn. Also, make sure to upload the seed dataset to your Google Drive and provide the correct file path.

## Conclusion
This implementation demonstrates the use of K-means clustering for classifying seeds based on their features. The optimal number of clusters is determined using the Elbow Method, and PCA is employed to visualize the clustered data points in 2D. The ARI is calculated to evaluate the clustering performance.
