# Objective
- Apply unsupervised machine learning (k-means clustering in this project) to group customers based on their purchasing behaviors
- Explore Elbow and Silhouette methods to choose k
- Visualize with PCA to help reduce the dimensionality

### Analysis:
In this project, we will find out which customer would act on the offers sent out to make purchases.
The problem is, we don't know how many groups to divide them into.
This type of situation is best applied with unsupervised learning. In this case, we used k-means clustering.
We choose k, the number of groups, using different methods list below.

#### The elbow method:

We plot the sum-of-squares error vs. k and choose the elbow point in the plot as the best value for k.
E.g., at which point the inertia seems to slow down.

![1 elbow inertia vs k](https://user-images.githubusercontent.com/36130927/126213026-15efc771-130c-4266-9343-60a8edc821f9.png)


Then we plot the amount of points in each of the k clusters.

![2 k clusters](https://user-images.githubusercontent.com/36130927/126212524-dd70d73f-4a58-4129-9911-4d045f5b196e.png)



#### The silhouette method

We choose k based on the highest silhouette score, ranging from -1 (poor clustering) to +1 (very dense clustering).
Score of 0 means clusters overlap.

![3 silhouette score interpretation](https://user-images.githubusercontent.com/36130927/126212539-88ba4973-6fa0-4da6-af5a-7f04ca90d80e.png)


![4 silhouette analysis](https://user-images.githubusercontent.com/36130927/126212606-38c14efd-320f-42eb-a28f-3ec7d8399c22.png)

We see k at 4 has the highest silhouette score.
However, cluster 3 is of poorer clustering compared to cluster 5 when k at 6, which has the second highest silhouette score.
I would choose 6 as the k using this method.

![5 silhouette score](https://user-images.githubusercontent.com/36130927/126213135-8e6b87f2-3c1a-4769-9d7b-1355b0b4e9dd.png)


So it seems that there is no absolute answer for using these methods as it can be subjective.

#### PCA

We can try to visualize the clusters with Principal Component Analysis (PCA).


![6 clustering](https://user-images.githubusercontent.com/36130927/126212663-2953cfcd-f50f-4438-b8d6-69a4c1b916fe.png)



In the plots above, 4 clusters seems to have more defined groups than 5 or 6 clusters.
Using the elbow method again on explained variance vs. k, we see that the curve slows down sharply at k = 4.
It means that that rate of descent starts to slow with the marginal increase in k, or k is not as effective as before starting that point.


![7 explained variance vs k](https://user-images.githubusercontent.com/36130927/126212686-00be0a7e-8e04-45a7-9950-47d24dbb6de5.png)



We further tested the silhouette score with other clustering algorithms,
including Affinity Propagation, Spectral Clustering, Agglomerative Clustering, and DBSCAN.
The scikit-learn documentation provides a general guidelines for different clustering algorithms.

![8 clustering algorithms](https://user-images.githubusercontent.com/36130927/126212846-0fc3d415-6f9a-4a49-92c8-d25f47963185.png)


### Conclusion:
- K-means clustering is one way to group clusters, with complements of methods such as elbow and silhouette.
- PCA can be used in various ways in dimension reduction.
For examples, it can be used to address regression performance with highly correlated variables,
in which it will untangles the correlations into a smaller number of features.
It can also reduce a large set of variables into a smaller one.

### Further work:
- Explore other methods of choosing k
- Visualize clusters with other clustering algorithms


### Skills used:
Python, data cleaning, data visualization, predictive modeling


### Libraries:
scikit-learn, numpy, pandas, matplotlib, seaborn
