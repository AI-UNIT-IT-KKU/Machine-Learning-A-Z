Random Forest Classification (Social Network Ads)
📌 Overview

This project demonstrates Random Forest, an ensemble method for classification tasks.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product by combining multiple Decision Trees to improve accuracy and reduce overfitting.

🚀 Why It’s Important

Classification tasks → Random Forest is powerful and robust for predicting categories.

Ensemble method → Combines multiple trees for more stable and accurate predictions.

Reduces overfitting → Averages predictions from multiple trees to generalize better than a single tree.

Feature importance → Can indicate which features contribute most to predictions.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for better model performance.

Train a Random Forest classifier → Using multiple Decision Trees with entropy as the splitting criterion.

Make predictions → For new users and the test set.

Evaluate performance → Compare predicted values with actual ones.
