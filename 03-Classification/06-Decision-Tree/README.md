Decision Tree Classification (Social Network Ads)
📌 Overview

This project demonstrates Decision Tree, a popular algorithm for classification tasks.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product based on age and salary by building a tree structure that splits data based on feature values.

🚀 Why It’s Important

Classification tasks → Decision Trees are intuitive and easy to interpret.

Non-linear separation → Can handle complex decision boundaries.

Feature importance → Identifies which features contribute most to classification.

Prediction → Can classify new users and check performance quickly.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for better performance.

Train a Decision Tree classifier → Using entropy as the splitting criterion.

Make predictions → For new users and the test set.

Evaluate performance → Compare predicted values with actual ones.
