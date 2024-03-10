# ElbowClusteringMethod
This is a demostration of how the elbow method works in clustering data which can later be used for training a machine learning model

#K-Means
The k-means function is a method of clustering analysis which aims to partition a dataset into k distinct, non-overlapping subgroups. Each data point belongs to the cluster with the nearest mean value. The "k" in k-means represents the number of clusters. The goal of k-means is to minimize the sum of squared errors (SSE) within each cluster. The SSE is the sum of the squared distances between each data point and the centroid of the cluster it belongs to.
#Elbow Method
The elbow method is a technique used to determine the optimal number of clusters in a dataset. The idea is to run the k-means algorithm for a range of k values, and for each value of k, calculate the SSE. A plot of the SSE as a function of k will typically show a bend or an "elbow" where the SSE starts to level off. This bend or elbow indicates the point at which adding more clusters does not significantly improve the model. The number of clusters at the elbow is considered as the optimal number of clusters for the dataset.

#Multi-Dimensional Clustering

In the code, we are performing K-means clustering on a multi-dimensional dataset (i.e., a dataset with more than one feature). K-means clustering is a popular unsupervised machine learning algorithm used to identify clusters within data. The goal is to partition the data into K distinct, non-overlapping clusters where each data point belongs to the cluster with the nearest mean.

Here's how the code works:

First, we import the necessary libraries, including pandas, KMeans from sklearn.cluster, StandardScaler from sklearn.preprocessing, and matplotlib.pyplot for visualization.
Next, we load a dataset from an Excel file named 'data.xlsx. We then normalize the data using StandardScaler to ensure that all features have equal importance.
We define a list to store the SSE (Sum of Squared Errors) for different number of clusters. SSE is a measure of the distance between each data point and its assigned cluster center. The lower the SSE, the better the clustering.
We define the range of possible number of clusters from 2 to 10.
For each possible number of clusters, we perform K-means clustering on the dataset and calculate the SSE.
Finally, we plot the SSE for different number of clusters to identify the optimal number of clusters. The optimal number of clusters is the one with the lowest SSE.

#Elbow Vs Scatterplot
The elbow method is used to determine the optimal number of clusters in a dataset by plotting the within-cluster sum of squares (WCSS) against the number of clusters and looking for the point where the curve starts to level off. The scatterplot method, on the other hand, involves visualizing the clusters in a two-dimensional scatterplot and looking for distinct groups of points.
