# SVD + PCA Breakdown – Phase 4 Summary
## Dataset: 20 Newsgroups
### Steps Performed:
- Loaded dataset and extracted raw text and labels.
- Converted the text data into numerical format using TF-IDF Vectorization with stop word removal and max feature limit.
- Applied Truncated SVD (n_components=2) for dimensionality reduction (latent semantic analysis).
- Visualized the reduced components with a 2D scatter plot, colored by their original newsgroup label.
- Applied k-Means Clustering with 20 clusters, calculated silhouette score, and compared predicted clusters with actual groups.

## Key Learnings:
- Learned how TF-IDF helps convert text into a high-dimensional numerical format reflecting word importance.
- Understood how SVD (a form of PCA) compresses sparse TF-IDF data while preserving semantic structure.
- Gained insights into dimensionality reduction benefits, especially for sparse data like text.
- Saw how clustering can reveal latent structure in unlabeled data and evaluated it using silhouette scores and visual comparisons.

## Results
- Dimensionality reduction (SVD) helps with sparse data like TF-IDF by reducing thousands of features into fewer meaningful components.
- SVD captures the most important directions of variance while preserving distances.
- Clustering reveals hidden structure in the data even without knowing true labels — useful for unsupervised exploration.
