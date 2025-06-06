# hierarchical-clustering-using-agglomerative
Hierarchical Clustering is an unsupervised machine learning algorithm used to group similar data points into clusters. Unlike flat clustering methods like K-Means, hierarchical clustering creates a nested hierarchy of clusters, represented as a tree-like structure called a dendrogram.

🧠 How it works
There are two main approaches:

Agglomerative (Bottom-Up) –

Starts with each data point as its own cluster

Iteratively merges the closest pairs of clusters

Continues until all points are merged into a single cluster

Most commonly used

Divisive (Top-Down) –

Starts with one large cluster containing all data

Recursively splits it into smaller clusters

Less common and more computationally intensive

📏 How similarity is measured
The distance between clusters is defined using a linkage method:

Single linkage: shortest distance between points in two clusters

Complete linkage: farthest distance between points

Average linkage: average distance between all pairs

Ward’s method: minimizes variance within clusters (most popular)

🌳 Dendrogram
A dendrogram is a tree diagram that shows the order and distances of cluster merges. You can "cut" the tree at a certain height to form clusters — this determines the number of final groups.

✅ Advantages
No need to pre-specify the number of clusters (you can choose later)

Works well with small to medium-sized datasets

Produces interpretable results through dendrograms

⚠️ Disadvantages
Computationally expensive for large datasets (especially divisive)

Sensitive to noise and outliers

Once clusters are merged/split, you can't undo them (no backtracking)

📌 Use Cases
Customer segmentation

Gene sequence analysis

Document or text clustering

Social network analysis


