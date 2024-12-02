# Dimensionality Reduction Techniques

## Youtube Link:

## Colab links: 
### Dimensionality Reduction Techniques: https://colab.research.google.com/drive/1r4-h-uGxbJ_f54OCxXDzpijJdjD5BW8M?usp=sharing
### Dimensionality Reduction using Data Bricks: https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/3771171209066087/4327013100957085/1964591634214885/latest.html

## Insights from different Dimensionality Reduction Techniques:

### 1. Randomized PCA
#### Results: Successfully captured the variance in high-dimensional data (e.g., Fashion-MNIST) while being computationally efficient for large datasets.
#### Key Insights: Randomized PCA is ideal for reducing dimensionality in large datasets without significant loss of information. It provides results comparable to standard PCA but at a fraction of the computational cost.
### 2. Kernel PCA
#### Results: Effectively captured non-linear patterns in data, such as separating clusters in the Olivetti Faces dataset using an RBF kernel.
#### Key Insights: Kernel PCA excels in handling non-linear relationships, making it suitable for datasets where linear methods like standard PCA fail. However, it is computationally intensive and requires careful kernel selection for optimal results.
### 3. Incremental PCA
#### Results: Reduced the dimensionality of large datasets (e.g., Breast Cancer) in memory-efficient chunks, preserving most of the original variance.
#### Key Insights: Incremental PCA is a practical choice for very large datasets that cannot fit in memory. It balances efficiency with accuracy, making it a scalable alternative to standard PCA for real-world applications.
### 4. t-SNE
#### Results: t-SNE effectively groups similar data points into tight clusters, particularly visible in datasets like MNIST.
#### Insights: It is excellent for identifying and visualizing distinct clusters in high-dimensional data. However, the results often distort the global relationships between clusters, making it unsuitable for tasks requiring a holistic view of the data.
### 5. UMAP
#### Results: UMAP balances cluster formation with a better representation of global relationships compared to t-SNE.
#### Insights: The embeddings offer both local and global perspectives, making it versatile for large datasets. UMAP produces smoother and faster results than t-SNE, especially for datasets like single-cell RNA-seq.
### 6. Locally Linear Embedding (LLE)
#### Results: LLE successfully unraveled the Swiss Roll dataset, projecting it into a flat, two-dimensional plane.
#### Insights: LLE preserves local structures well but can struggle with noisy data or more complex manifolds. It is particularly effective when neighborhood relationships are critical.
### 7. ISOMAP
#### Results: ISOMAP unfolds non-linear manifolds, such as the Swiss Roll and faces datasets, preserving both local and global geodesic relationships.
#### Insights: ISOMAP excels in capturing global structures, making it suitable for data with intrinsic manifold properties. However, its performance deteriorates with high noise levels or sparse data.
### 8. MDS
#### Results: MDS retained pairwise dissimilarities effectively for the Iris dataset, showing clear separation among classes.
#### Insights: It provides a well-balanced representation of similarities or dissimilarities but may struggle with very large datasets due to computational constraints.
### 9. Factor Analysis
#### Results: Factor Analysis identified latent factors in the 20 Newsgroups dataset, grouping data points based on underlying shared patterns.
#### Insights: It highlights hidden relationships in tabular datasets, but its performance is limited to linearly separable factors.
### 10. Autoencoders
#### Results: Autoencoders compressed MNIST images into a reduced feature space while preserving essential information for reconstruction.
#### Insights: The embeddings captured both global and local relationships, demonstrating the power of neural networks for non-linear dimensionality reduction. Reconstruction errors indicate the quality of dimensionality reduction.
