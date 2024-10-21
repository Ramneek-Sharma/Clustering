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

- **K-Means Clustering Results:**
<img width="1317" alt="Screenshot 2024-10-21 at 6 19 48 AM" src="https://github.com/user-attachments/assets/5e53a148-490a-4b61-a14f-5543e273c2b0">
<img width="71" alt="Screenshot 2024-10-21 at 6 20 03 AM" src="https://github.com/user-attachments/assets/92a5ffa3-1771-46a6-871a-54c53e740d2d">
<img width="372" alt="Screenshot 2024-10-21 at 6 20 14 AM" src="https://github.com/user-attachments/assets/82bc24c6-c8d2-4ce7-a23a-6cb530a364a6">





- **Hierarchical Clustering Results:**
<img width="1331" alt="Screenshot 2024-10-21 at 6 22 07 AM" src="https://github.com/user-attachments/assets/014ac91a-ee58-48a3-b96b-e36c95b990fa">

<img width="69" alt="Screenshot 2024-10-21 at 6 16 26 AM" src="https://github.com/user-attachments/assets/cc2d1df2-e1e1-4b02-92dc-5e6f796a9b5c">
<img width="375" alt="Screenshot 2024-10-21 at 6 20 48 AM" src="https://github.com/user-attachments/assets/f5cc8cdc-be27-4b06-8aff-e07960988080">


- **Mean Shift Clustering Results:**
<img width="1321" alt="Screenshot 2024-10-21 at 6 16 14 AM" src="https://github.com/user-attachments/assets/774bcef8-ccc3-473c-8337-a0c416b99bfe">
<img width="69" alt="Screenshot 2024-10-21 at 6 16 26 AM" src="https://github.com/user-attachments/assets/cc2d1df2-e1e1-4b02-92dc-5e6f796a9b5c">
<img width="368" alt="Screenshot 2024-10-21 at 6 16 41 AM" src="https://github.com/user-attachments/assets/b92b3028-0dea-4ae9-a9ba-c95645564fdb">

### Visualizations

Below are the visual representations of clustering results:

- **K-Means Clustering Results:**
[graph of kmean(click here)](https://github.com/Ramneek-Sharma/Clustering/blob/main/kmean_graph.pdf)
- **Hierarchical Clustering Results:**
[graph of Hierarchical(click here)](https://github.com/Ramneek-Sharma/Clustering/blob/main/heirarchy.pdf)

- **Mean Shift Clustering Results:**
[graph of MeanShift(click here)](https://github.com/Ramneek-Sharma/Clustering/blob/main/meanshift.pdf)



## Conclusions

- **PyCaret**: Simplifies the implementation of clustering algorithms, automatically calculates metrics, and requires less code compared to Scikit-learn. It also handles the heavy lifting of pre-processing and results in more concise code.
  
  However, PyCaret doesn't generate some specific visualizations out-of-the-box, requiring users to manually plot them or use Scikit-learn or other libraries for advanced visualizations.

- **Scikit-learn**: Offers more control over the clustering process and customization options for each algorithm. However, it requires more code for calculating metrics and generating visualizations.

### Key Observations:

1. **K-Means**: Achieved higher performance across both libraries, though PyCaret slightly outperformed Scikit-learn in terms of clustering metrics.
2. **Mean Shift**: Performed best overall in terms of Silhouette Score, particularly in PyCaret.
3. **Hierarchical Clustering**: Performed similarly in both libraries but lagged behind K-Means and Mean Shift.


