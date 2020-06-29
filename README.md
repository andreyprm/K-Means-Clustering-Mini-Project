# K-Means-Clustering-Mini-Project

This is an unsupervised learning models mini-project using K-Means clustering with World Happiness Score data. 
The goal is to show the workflow of unsupervised learning model specifically the K-Means clustering data.

### Modelling code 
```
from sklearn.cluster import 
inertia = []
for i in range(2,20):
    kmeans = KMeans(n_clusters=i,
               init='k-means++',
               n_init=15,
               max_iter=500,
               random_state=101)
    kmeans.fit(df_pca)
    inertia.append(kmeans.inertia_)KMeans

from sklearn.metrics import silhouette_score
silhouette = {}
for i in range(2,20):
    kmeans = KMeans(n_clusters=i,
               init='k-means++',
               n_init=15,
               max_iter=500,
               random_state=101)
    kmeans.fit(df_pca)
    silhouette[i] = silhouette_score(df_pca, kmeans.labels_, metric='euclidean')
    ```
 
### Clustering Graph
![GitHub Logo](/cluster.png)
