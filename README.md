# Clustering 

Three clustering algorithms are used : **K-Means**, **Hierarchical Clustering**, and **Mean Shift Clustering**. Algorithms are implemented using two different approaches: one using **PyCaret** and the other using **Scikit-learn**. We evaluate their performance using key clustering metrics: **Silhouette Score**, **Calinski-Harabasz Index**, and **Davies-Bouldin Score**.

**reason for using pycaret** Simplifies the implementation of clustering algorithms, automatically calculates metrics, and requires less code compared to Scikit-learn. It also handles the heavy lifting of pre-processing and results in more concise code.
  
  However, PyCaret doesn't generate some specific visualizations out-of-the-box, requiring users to manually plot them or use Scikit-learn or other libraries for advanced visualizations. Thats why the clustering also perform by **sckikit-learn**


## Overview

Clustering is an unsupervised learning technique used to group similar data points. In this project, we compare three popular clustering algorithms:

1. **K-Means**
<img width="607" alt="Screenshot 2024-10-21 at 6 23 36 AM" src="https://github.com/user-attachments/assets/44fc9b0d-644a-4333-a229-2a176575e6a9">
<img width="552" alt="Screenshot 2024-10-21 at 6 24 36 AM" src="https://github.com/user-attachments/assets/5913a28c-ef40-4aa1-bf5f-d2705e8b1b6e">
<img width="608" alt="Screenshot 2024-10-21 at 6 24 50 AM" src="https://github.com/user-attachments/assets/17f63c5e-1b72-4e30-80d7-c5955304f7d2">
<img width="564" alt="Screenshot 2024-10-21 at 6 25 33 AM" src="https://github.com/user-attachments/assets/2a32fa33-49e2-419b-8940-f73cb8d0b1c9">
<img width="465" alt="Screenshot 2024-10-21 at 6 26 28 AM" src="https://github.com/user-attachments/assets/820fb0f3-b0fd-464c-9671-5d176d6116c6">
<img width="426" alt="Screenshot 2024-10-21 at 6 26 39 AM" src="https://github.com/user-attachments/assets/fb3fe420-b5d3-429a-8310-16e3e90f1ed5">
<img width="468" alt="Screenshot 2024-10-21 at 6 26 52 AM" src="https://github.com/user-attachments/assets/5d34a6f2-2eff-4ed3-87b4-0bd60b08a0cb">
<img width="562" alt="Screenshot 2024-10-21 at 6 27 08 AM" src="https://github.com/user-attachments/assets/4cc9cda6-24fc-4dd9-bf26-869301e77e6e">
<img width="484" alt="Screenshot 2024-10-21 at 6 27 43 AM" src="https://github.com/user-attachments/assets/a9d78bfd-09c8-438e-8286-e4fc25880dca">


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


