🧩 Model Selection: Grid Search and k-Fold Cross Validation with SVM
📌 Overview

This project demonstrates model selection techniques for Support Vector Machines (SVM) on the Social Network Ads dataset.
We use Grid Search to find optimal hyperparameters and k-Fold Cross Validation to evaluate model stability.


🔍 Part 1: Grid Search

Feature scaling is applied to standardize features.

SVM classifier with RBF kernel is trained on training set.

Grid Search explores multiple combinations of C, kernel, and gamma to find the best parameters.

Cross-validation (10 folds) evaluates the classifier accuracy.

Decision region plots visualize the classification results for training and test sets.

🔄 Part 2: k-Fold Cross Validation

Same dataset preprocessing and SVM classifier.

k-Fold Cross Validation (10 folds) is applied to training set.

Reports mean accuracy and standard deviation to assess model stability.

Decision region plots show classifier performance on training and test sets.


