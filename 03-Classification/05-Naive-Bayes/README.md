Naive Bayes Classification (Social Network Ads)
📌 Overview

This project demonstrates Naive Bayes, a simple yet powerful classification algorithm based on Bayes' theorem.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product based on their age and salary.

🚀 Why It’s Important

Classification tasks → Works well with both categorical and numerical data.

Simple & fast → Easy to implement and computationally efficient.

Probabilistic approach → Uses probability to classify points, making it interpretable.

Prediction & evaluation → Can quickly predict new users and check accuracy.

Visualization → Decision boundary plots help understand how the model separates classes.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for better performance.

Train a Gaussian Naive Bayes classifier → Fit the model on training data.

Make predictions → On the test set and compare with actual values.

Evaluate performance → Using Confusion Matrix and Accuracy Score.

Visualize decision boundaries → Show how Naive Bayes separates classes on the test set.
