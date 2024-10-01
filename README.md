# CryptoClustering

Challenge Overview:

In this challenge, Python and unsupervised learning techniques were used to explore how 24-hour and 7-day price changes affect cryptocurrencies.


Steps to Prepare the Data:

Normalization: The StandardScaler() from scikit-learn was applied to ensure that all data features were on the same scale, giving them equal importance.


Creating a DataFrame: 

A new DataFrame was created with the scaled data, using "coin_id" from the original dataset as the index.

Finding the Best K: 

The elbow method was used to determine that the optimal number of clusters, 
𝑘
k, was 4 when analyzing the original scaled data.

K-Means Clustering: 

K-Means clustering was performed on the original scaled data, and the clusters were visualized using hvPlot, with 'price_change_percentage_24h' on the x-axis and 'price_change_percentage_7d' on the y-axis.

Using PCA: 

Principal Component Analysis (PCA) was used to reduce the features to three main components, which explained 88% of the variation in the data.

Clustering with PCA Data: 

The best 
𝑘
k value was also found to be 4 when using the PCA data, consistent with the results from the original scaled data.

Visualizing PCA Clusters: 

A second cluster graph was created with hvPlot, using 'PC1' for the x-axis and 'PC2' for the y-axis.

Analyzing Results:

 Finally, the clustering results were compared with and without PCA. Some clusters showed changes in color, indicating shifts in group membership.