Support Vector Machine (SVM) Classification with Kernel (Social Network Ads)
📌 Overview

This project demonstrates Support Vector Machine (SVM) for classification using a kernel.

The dataset (Social_Network_Ads.csv) contains:

Age

Estimated Salary

Purchased → whether a user bought the product (0 = No, 1 = Yes).

The goal is to train a model that predicts if a user will purchase a product based on age and salary.
By using the RBF kernel, SVM can handle non-linear data where a straight line cannot separate the classes properly.

🚀 Why It’s Important

Classification tasks → SVM is powerful for both linear and non-linear data.

Kernels → Transform data into higher dimensions, making classes separable.

Feature scaling → Required since SVM relies on distance calculations.

Prediction → Can classify new data points even when data is not linearly separable.

⚙️ What the Code Does

Import libraries → numpy, pandas, matplotlib.

Load the dataset (Social_Network_Ads.csv) → Extract features (X) and target (y).

Split the dataset → Training (75%) and Testing (25%).

Apply Feature Scaling → Normalize values for correct distance measurement.

Train an SVM classifier with RBF kernel → Captures non-linear boundaries to separate classes.

Make predictions → Classify new/unseen users and test set samples.

Visualize decision boundaries → Show how SVM with kernel separates non-linear data.
