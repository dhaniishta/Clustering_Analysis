# Clustering_Analysis

This project demonstrates the comparative performance analysis of different clustering algorithms with various preprocessing techniques applied to the **Iris dataset** from the UCI Machine Learning Repository. The study evaluates clustering quality based on multiple metrics and presents results in tables and graphs.

---

## Project Workflow

1. **Dataset Used**: 
   - **Iris Dataset**: A multivariate dataset with 150 samples of three classes (Setosa, Versicolor, Virginica), each with four features.

2. **Preprocessing Techniques**:
   - **No Data Processing**: Raw data as is.
   - **Normalization**: Scaling features to zero mean and unit variance.
   - **Principal Component Analysis (PCA)**: Reducing dimensions to 2.
   - **Combination (T+N+PCA)**: Applying normalization followed by PCA.

3. **Clustering Algorithms**:
   - **K-Means Clustering**
   - **Hierarchical Clustering**
   - **Mean-Shift Clustering**

4. **Evaluation Metrics**:
   - **Silhouette Score**: Measures cluster compactness and separation.
   - **Calinski-Harabasz Index**: Evaluates the dispersion ratio of clusters.
   - **Davies-Bouldin Index**: Measures cluster compactness and similarity.

---

## Results Overview

The results of the clustering analysis are stored in the file **`clustering_results.csv`**. Each algorithm's performance is evaluated for 3, 4, and 5 clusters across different preprocessing techniques.

### Example of Results Table:
| Algorithm       | Preprocessing      | Clusters | Silhouette | Calinski | Davies-Bouldin |
|------------------|--------------------|----------|------------|----------|----------------|
| K-Means         | Normalized         | 3        | 0.68       | 6633     | 0.59           |
| Hierarchical    | PCA                | 4        | 0.49       | 1983     | 0.71           |
| Mean-Shift      | No Data Processing | 3        | 0.99       | 5586     | 0.13           |

---

## Visualizations

1. **Dendrogram**: Represents hierarchical clustering results.
2. **PCA Scatter Plots**: Visualize clusters in reduced dimensions.

---
