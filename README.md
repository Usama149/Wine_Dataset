## Clustering Results

The Wine dataset was analyzed using two clustering algorithms:

- K-Means Clustering
- Hierarchical Clustering

Before applying the algorithms, the dataset was standardized using `StandardScaler` because the wine features have different value ranges. Since the dataset contains many features, PCA was used to reduce the data to 2 dimensions for visualization.

### K-Means Clustering

The Elbow Method was used to determine the optimal number of clusters. The plot showed a clear elbow at **3 clusters**, suggesting that this was the most suitable number of groups for the dataset.

After applying K-Means with `n_clusters = 3`, the PCA visualization showed three reasonably distinct groups of wine samples. The centroids were positioned near the center of each cluster, indicating that the algorithm captured the overall structure of the data well.

### Hierarchical Clustering

A dendrogram was used to identify the appropriate number of clusters. The large vertical distances between merges suggested that the dataset naturally forms **3 main clusters**.

After applying Agglomerative Hierarchical Clustering with `n_clusters = 3`, the PCA visualization again showed three clearly separated groups. This result supported the findings from K-Means.

### Conclusion

Both K-Means and Hierarchical Clustering produced similar results, showing that the Wine dataset can be naturally divided into **3 clusters** based on its chemical properties.

This suggests that:
- wines within the same cluster are more similar to each other
- wines in different clusters are more distinct
- the dataset contains meaningful natural groupings even without using the original class labels

## Visualizations

### Elbow Method
<img width="580" height="455" alt="the_elbow_method_wine_dataset" src="https://github.com/user-attachments/assets/5a85c43e-b60b-49b4-83ff-73bbf8d9de96" />


### K-Means Clustering
<img width="565" height="455" alt="k_means_clustering_wine_dataset" src="https://github.com/user-attachments/assets/0d1857e5-ff57-4799-aa45-b6be8221b646" />


### Dendrogram
<img width="564" height="454" alt="dendrogram" src="https://github.com/user-attachments/assets/f0b5c489-c307-419f-a3ed-182c8be51cb6" />


### Hierarchical Clustering
<img width="565" height="455" alt="heirarchel_clustering_wine_dataset" src="https://github.com/user-attachments/assets/3ac428e0-07a1-42e6-8548-6007b52015e2" />
