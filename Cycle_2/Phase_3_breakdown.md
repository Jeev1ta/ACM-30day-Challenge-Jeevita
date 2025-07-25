# Data Preparation
- Loaded the dataset and removed the Id column.
- Scaled the features using StandardScaler.

# Clustering
- Applied k-Means Clustering.
  - Used the Elbow Method to determine optimal number of clusters (k=3).
- Applied Hierarchical Clustering.
  - Plotted the Dendrogram using scipy's linkage and dendrogram.
  - Extracted flat clusters using fcluster.
- Dimensionality Reduction
  - Applied PCA to reduce dimensions to 2D for visualization.
  - Visualized clusters from both methods using PCA plots.
# Outputs
- Plots:
  - Elbow Curve
  - Dendrogram
  - PCA Cluster Visualization for both k-Means and Hierarchical Clustering.
