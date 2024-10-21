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
| Index               | No data processing (c=3) | No data processing (c=4) | No data processing (c=5) | Normalized (c=3) | Normalized (c=4) | Normalized (c=5) | Transform (c=3) | Transform (c=4) | Transform (c=5) | PCA (c=3) | PCA (c=4) | PCA (c=5) | T+N (c=3) | T+N (c=4) | T+N (c=5) | T+N+P (c=3) | T+N+P (c=4) | T+N+P (c=5) |
|---------------------|--------------------------|--------------------------|--------------------------|------------------|------------------|------------------|-----------------|-----------------|-----------------|-----------|-----------|-----------|-----------|-----------|-----------|--------------|--------------|--------------|
| **Silhouette**       | 0.5528                   | 0.4954                   | 0.3663                   | 0.4565           | 0.4310           | 0.3450           | 0.6540          | 0.6131          | 0.5820          | 0.5520    | 0.4975    | 0.4922    | 0.4781    | 0.4272    | 0.3569    | 0.4781       | 0.4272       | 0.3569       |
| **Calinski-Harabasz**| 561.6277                 | 529.1967                 | 456.0335                 | 239.4845         | 206.0730         | 202.6359         | 1164.8165       | 1346.6146       | 1378.3527       | 561.5936  | 530.4871  | 492.7029  | 225.3     | 213.7555  | 202.2256  | 225.3        | 213.7555      | 202.2256     |
| **Davies-Bouldin**   | 0.662                    | 0.764                    | 0.916                    | 0.8275           | 0.9223           | 0.9439           | 0.4883          | 0.5369          | 0.5987          | 0.666     | 0.7757    | 0.8088    | 0.7434    | 0.9024    | 0.9181    | 0.7434       | 0.9024       | 0.9181       |


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


