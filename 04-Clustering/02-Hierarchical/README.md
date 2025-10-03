Hierarchical Clustering (Mall Customers Dataset)
📌 Overview

This project demonstrates Hierarchical Clustering using the Mall_Customers.csv dataset.
The dataset includes customer information such as:

Annual Income

Spending Score

Clustering helps segment customers into groups, providing valuable business insights for marketing, sales, and customer relationship management.

⚙️ Steps in the Code

Import libraries

numpy, pandas, matplotlib → For data handling and visualization.

scipy.cluster.hierarchy → For building the dendrogram.

sklearn.cluster.AgglomerativeClustering → For hierarchical clustering.

Load dataset

Extract relevant features: Annual Income and Spending Score.

Dendrogram

Plot a dendrogram to determine the optimal number of clusters.

Shows how data points are merged step by step.

Agglomerative Clustering

Train the model to group customers into 5 clusters using:

Euclidean distance → Measures similarity between points.

Ward linkage → Minimizes variance within each cluster.

Visualization

Scatter plot shows 5 customer clusters.

Different colors represent different groups, making segmentation clear.

🎯 Importance

Hierarchical Clustering helps businesses understand customer behavior by identifying groups such as:

High income & high spending → Loyal, profitable customers.

High income & low spending → Potential targets for upselling.

Low income & high spending → Engaged but budget-conscious customers.

This segmentation supports marketing strategies, customer targeting, and product recommendations.
