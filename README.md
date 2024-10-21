# Clustering 

Three clustering algorithms are used : **K-Means**, **Hierarchical Clustering**, and **Mean Shift Clustering**. Algorithms are implemented using two different approaches: one using **PyCaret** and the other using **Scikit-learn**. We evaluate their performance using key clustering metrics: **Silhouette Score**, **Calinski-Harabasz Index**, and **Davies-Bouldin Score**.

**reason for using pycaret** Simplifies the implementation of clustering algorithms, automatically calculates metrics, and requires less code compared to Scikit-learn. It also handles the heavy lifting of pre-processing and results in more concise code.
  
  However, PyCaret doesn't generate some specific visualizations out-of-the-box, requiring users to manually plot them or use Scikit-learn or other libraries for advanced visualizations. Thats why the clustering also perform by **sckikit-learn**


## Overview

Clustering is an unsupervised learning technique used to group similar data points. In this project, we compare three popular clustering algorithms:

1. **K-Means**
2. **Hierarchical Clustering**
3. **Mean Shift Clustering**

Each algorithm was implemented using two approaches:
- **PyCaret**, an automated machine learning library.
- **Scikit-learn**, a popular machine learning library in Python.

The goal is to compare the performance of these algorithms based on **Silhouette Score**, **Calinski-Harabasz Index**, and **Davies-Bouldin Score**.

## Datasets

Iris Dataset is used  for this clustering analysis. The dataset contains multiple features that allow us to explore the performance of different clustering methods.

## Clustering Algorithms

1. **K-Means Clustering**: A centroid-based clustering algorithm that partitions data into k clusters.
2. **Hierarchical Clustering**: A tree-like clustering structure that can be agglomerative or divisive.
3. **Mean Shift Clustering**: A centroid-based algorithm that iteratively shifts centroids towards regions of higher data density.



## Metrics

We evaluate clustering performance using the following metrics:

- **Silhouette Score**: Measures how similar a point is to its own cluster compared to other clusters. Higher scores indicate better-defined clusters.
- **Calinski-Harabasz Index**: Measures the ratio of within-cluster dispersion to between-cluster dispersion. Higher values indicate better-defined clusters.
- **Davies-Bouldin Index**: Measures the average similarity ratio of each cluster with its most similar cluster. Lower values indicate better clustering.

## Results


### Visualizations

Below are the visual representations of clustering results:

- **K-Means Clustering Results:**
<img width="1307" alt="Screenshot 2024-10-21 at 5 54 53 AM" src="https://github.com/user-attachments/assets/3d778593-6745-4e4f-89f5-a6866a383c5b">
<img width="1255" alt="Screenshot 2024-10-21 at 5 55 29 AM" src="https://github.com/user-attachments/assets/d9cef17b-17c6-4d0e-b162-6d64405e17dd">

- **Hierarchical Clustering Results:**


- **Mean Shift Clustering Results:**




## Conclusions

- **PyCaret**: Simplifies the implementation of clustering algorithms, automatically calculates metrics, and requires less code compared to Scikit-learn. It also handles the heavy lifting of pre-processing and results in more concise code.
  
  However, PyCaret doesn't generate some specific visualizations out-of-the-box, requiring users to manually plot them or use Scikit-learn or other libraries for advanced visualizations.

- **Scikit-learn**: Offers more control over the clustering process and customization options for each algorithm. However, it requires more code for calculating metrics and generating visualizations.

### Key Observations:

1. **K-Means**: Achieved higher performance across both libraries, though PyCaret slightly outperformed Scikit-learn in terms of clustering metrics.
2. **Mean Shift**: Performed best overall in terms of Silhouette Score, particularly in PyCaret.
3. **Hierarchical Clustering**: Performed similarly in both libraries but lagged behind K-Means and Mean Shift.


