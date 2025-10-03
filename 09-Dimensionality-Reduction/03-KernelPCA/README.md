🍷 Kernel PCA with Logistic Regression on Wine Dataset
📌 Overview

This project applies Kernel PCA to perform non-linear dimensionality reduction on the Wine dataset and uses Logistic Regression for classification.
Kernel PCA maps features into a higher-dimensional space for better class separability.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, sklearn.

Load Dataset → Wine.csv with chemical properties, X = features, y = class labels.

Split Dataset → 80% training, 20% test.

Feature Scaling → Standardize features for Kernel PCA.

Apply Kernel PCA → Reduce to 2 principal components (PC1, PC2) using RBF kernel.

Train Logistic Regression → Fit on Kernel PCA-transformed training set.

Predict & Evaluate → Test set predictions, confusion matrix, accuracy score.

Visualization → Plot decision regions for training and test sets using PC1 and PC2.

🎯 Importance

Enables non-linear dimensionality reduction for complex data.

Useful when linear PCA cannot separate classes well.

2D visualization gives intuitive understanding of class separation.

Logistic Regression performs effectively after Kernel PCA transformation.
