Support Vector Machine (SVM) Classification (Social Network Ads)
📌 Overview

This project demonstrates Support Vector Machine (SVM), a popular algorithm for classification tasks.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will buy a product based on their age and salary by finding the optimal separating hyperplane between the two classes.

🚀 Why It’s Important

Classification tasks → SVM is powerful for separating categories.

Non-linear data → With kernels (e.g., RBF), SVM can handle data that is not linearly separable.

Decision boundaries → Maximizes the margin between classes, making predictions more robust.

Preprocessing → Feature scaling ensures distances are meaningful for the algorithm.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for better performance.

Train an SVM classifier → Using a linear kernel.

Make predictions → For new/unseen users and on the test set.

Evaluate performance → Compare predicted values with actual ones.
