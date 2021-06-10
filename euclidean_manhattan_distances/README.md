# Objective
- Visualize the difference in Euclidean and Manhattan distance calculations


#### Analysis:
The idea of this exploratory work on distance calculation is to understand how different data points appear on the graph in the distance metric.

The Euclidean graphs below tell us the data points are close to (5,5) on the YZ plane.

![1 euclidean55](https://user-images.githubusercontent.com/36130927/121603064-37408a80-ca16-11eb-9e96-8164f57ead08.png)

![2 euclidean33](https://user-images.githubusercontent.com/36130927/121603068-3871b780-ca16-11eb-9f0b-6b6a4ff35c16.png)


The Manhattan graphs below tell us the data points are close to (5,5) on the XZ plane.

![3 manhattan55](https://user-images.githubusercontent.com/36130927/121603074-390a4e00-ca16-11eb-86e5-eccc5597f587.png)

![4 manhattan44](https://user-images.githubusercontent.com/36130927/121603075-39a2e480-ca16-11eb-8bec-e3229770ae5a.png)


But when we compare the same data points calculated into two distances, we see that Manhattan method usually generates a further distance than Euclidean method.
This is expected due to their equations.

![5 scipy dist](https://user-images.githubusercontent.com/36130927/121603076-3a3b7b00-ca16-11eb-8ce0-0a8ef46d5adf.png)


****Euclidean distance:****

![6 CodeCogsEqn - euclidean](https://user-images.githubusercontent.com/36130927/121604860-4ffe6f80-ca19-11eb-8734-69d169d09164.gif)

p,q	=	two points in Euclidean n-space

q<sub>i</sub>, p<sub>i</sub>	=	Euclidean vectors, starting from the origin of the space (initial point)

n	=	n-space



****Manhattan distance:****

![7 CodeCogsEqn - manhattan](https://user-images.githubusercontent.com/36130927/121607386-f2b8ed00-ca1d-11eb-9eec-d87b01d61cf4.gif)






#### Further work:
- Plot a 3D graph to show data points with their distances on all X-, Y-, and Z-axes
- Apply on different use cases to see which distance is more effective


#### Skills used:
Python


#### Libraries:
scipy, numpy, pandas, matplotlib
