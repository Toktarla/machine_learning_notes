Clustering is a type of **unsupervised learning** used to group similar data points together. 
Finds patterns and groupings
Doesnt need labels (outputs) in dataset

 **Centroid**: The center of a cluster. In k-means, the centroid is the mean of all points in that cluster.
 
 **Distance Metric**: A function that defines the distance between two data points (e.g., Euclidean distance).
 
 **Euclidean Distance**: The straight-line distance between two points in a multi-dimensional space.

#### **Common Clustering Algorithms:**

- **k-Means**: A popular method that partitions the data into **k** clusters by minimizing the sum of squared distances between points and their cluster centroids.
- **Hierarchical Clustering**: Builds a tree-like structure (dendrogram) and does not require specifying the number of clusters beforehand.
- **Spectral Clustering**: Uses the eigenvalues of the similarity matrix of the data to reduce the dimensionality of the problem.
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**: Groups points based on their density, useful for data with clusters of arbitrary shape.

- **Expectation-Maximization (EM)**: A statistical method for finding maximum likelihood estimates of parameters in models with latent variables, like Gaussian Mixture Models (GMM).
- **Gaussian Mixture Model (GMM)**: A probabilistic model that assumes the data is a mixture of several Gaussian distributions, each representing a cluster.
- **Choosing k**: Determining the optimal number of clusters in a dataset. Methods include the **Elbow Method**, **Silhouette Score**, and **Gap Statistic**.


