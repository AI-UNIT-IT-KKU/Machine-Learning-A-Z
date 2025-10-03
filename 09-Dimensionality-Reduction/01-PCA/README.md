🍷 PCA with Logistic Regression on Wine Dataset
📌 Overview

This project applies Principal Component Analysis (PCA) to reduce the dimensionality of the Wine dataset and uses Logistic Regression to classify wine types.
PCA reduces features to 2 principal components for easy visualization and effective classification.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, sklearn.

Load Dataset → Wine.csv with chemical properties, X = features, y = class labels.

Split Dataset → 80% training, 20% test.

Feature Scaling → Standardize features for PCA.

Apply PCA → Reduce to 2 principal components (PC1, PC2).

Train Logistic Regression → Fit on PCA-transformed training set.

Predict & Evaluate → Test set predictions, confusion matrix, accuracy score.

Visualization → Plot decision regions for training and test sets using PC1 and PC2.

🎯 Importance

Reduces dimensionality while retaining most of the variance.

Allows easy 2D visualization of high-dimensional data.

Logistic Regression works effectively on PCA-transformed features.
