🍷 LDA with Logistic Regression on Wine Dataset
📌 Overview

This project applies Linear Discriminant Analysis (LDA) to reduce the dimensionality of the Wine dataset and uses Logistic Regression for classification.
LDA reduces features to 2 linear discriminants for visualizing class separation and improving classifier performance.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, sklearn.

Load Dataset → Wine.csv with chemical properties, X = features, y = class labels.

Split Dataset → 80% training, 20% test.

Feature Scaling → Standardize features for LDA.

Apply LDA → Reduce to 2 linear discriminants (LD1, LD2).

Train Logistic Regression → Fit on LDA-transformed training set.

Predict & Evaluate → Test set predictions, confusion matrix, accuracy score.

Visualization → Plot decision regions for training and test sets using LD1 and LD2.

🎯 Importance

Reduces dimensionality while preserving class separability.

Logistic Regression works effectively on LDA-transformed features.

2D visualization helps understand class distributions intuitively.
