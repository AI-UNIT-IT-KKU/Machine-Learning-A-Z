K-Nearest Neighbors (K-NN) Classification (Social Network Ads)
📌 Overview

This project demonstrates K-Nearest Neighbors (K-NN), a simple and intuitive classification algorithm.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product based on their age and salary by checking the closest data points (neighbors).

🚀 Why It’s Important

Classification tasks → K-NN is widely used for category prediction.

Easy to understand → It classifies based on the majority vote of the nearest neighbors.

Preprocessing → Feature scaling ensures distances are measured correctly.

Visualization → Decision boundary plots help us see how the algorithm separates the two classes.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib for data handling and visualization.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for correct distance measurement.

Train the K-NN classifier → Using n_neighbors=5.

Make predictions → For a new user and on the test set.

Evaluate the model → Using Confusion Matrix and Accuracy Score.

Visualize decision boundaries → For both training and test sets.
