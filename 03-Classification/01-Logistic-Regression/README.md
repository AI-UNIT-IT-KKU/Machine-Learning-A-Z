Logistic Regression Classification (Social Network Ads)
📌 Overview

This project demonstrates Logistic Regression, a widely used algorithm for classification tasks.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product based on their age and salary.

🚀 Why It’s Important

Classification: Logistic Regression is one of the simplest yet effective algorithms for predicting binary outcomes (e.g., Yes/No, True/False).

Preprocessing: Scaling features improves training speed and ensures fair weight distribution.

Prediction & Evaluation: Demonstrates how to make predictions and measure accuracy with metrics.

Visualization: Shows the decision boundary to better understand how the model separates classes.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib for data handling and visualization.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for better model performance.

Train the Logistic Regression classifier → Fit the model on training data.

Make predictions → On new/unseen data and test set.

Evaluate model performance → Using Confusion Matrix and Accuracy Score.

Visualize decision boundaries → For both training and test sets.
