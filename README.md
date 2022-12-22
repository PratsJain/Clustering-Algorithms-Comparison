# Clustering-Algorithms-Comparison
We first went through a lot of datasets and visualised them in order to find datasets with separable clusters.
We also looked at the properties of various clustering algorithms in order to find an apt match for each clustering type.
We finally selected three datasets:  
Density Based Clustering: Anuran Calls  
Hierarchichal Clustering: Tech Students Profile Dataset  
Prototypes Clustering: Root Cells Dataset  
For all the datasets, we ran sklearn's dummy classifier to compare the performance of all other
algorithms against random data.
For Intrinsic Metrics, we used:  
Silhouette Score  
Davies Bouldin Score  
For Extrinsic Metrics, we used:  
Adjusted Rand Index Score  
Adjusted Mutual Information Score   

After choosing the datasets, we ran DBSCAN and OPTICS on them for density based
clustering. For DBSCAN, we used Nearest neighbours method to determine
the best value of epsilon and for OPTICS, we used a grid search like method to determine the
best values of minimum cluster size
and minimum samples. We determined the xi using the reachability plot. We then compared the
performances on various metrics
using graph plots.  

For Hierarchichal Clustering, we ran Agglomerative clustering with various linkages (Single,
Complete, Average, Ward) on the datasets.
We used dendrogram plot to compute the number of clusters for the algorithm. We then
compared the performances on various metrics using graph plots.  

For Prototypes Clustering, we ran K-Means clustering along with Spectral and K-Medoids
Clustering on the datasets.
For K-Means and K-Medoids, we used the Elbow Method on inertia along with grid search to
determine the n_cluster
hyperparameter. For Spectral Clustering, we used Silhouette Analysis along with grid search for
hyperparameter tuning.
We then compared the performances on various metrics using graph plots.
For all the datasets and algorithms, we used TSNE plots to compare and visualise the clustering
performance of various algorithms
on the three datasets.  

Overall, we used the following listed clustering algorithms:  
- DBSCAN
- OPTICS
- Hierarchichal Clustering (Linkage: Single)
- Hierarchichal Clustering (Linkage: Average)
- Hierarchichal Clustering (Linkage: Ward)
- Hierarchichal Clustering (Linkage: Complete)
- K Means Clustering
- K Medoids Clustering 
- Spectral Clustering  

We concluded that spectral clsutering performed the best on all thee three datasets. It was consistently the best algorithm and outtperformed the rest of the algorithms.
