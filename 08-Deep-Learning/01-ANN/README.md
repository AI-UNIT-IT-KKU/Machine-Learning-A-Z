🔮 Customer Churn Prediction using ANN
📌 Overview

This project predicts customer churn using an Artificial Neural Network (ANN).
The dataset Churn_Modelling.csv contains customer details such as:

Geography

Gender

Age

Balance

Other features
The target column indicates if the customer exited (churned).

⚙️ Steps in the Code

Import Libraries → numpy, pandas, tensorflow (Keras), sklearn.

Load Dataset → Features (X) and target (y = Exited).

Encode Categorical Data → Label encode Gender, one-hot encode Geography.

Split Dataset → 80% training, 20% testing.

Feature Scaling → Standardize features for better ANN performance.

Build ANN → Input layer + 2 hidden layers (6 units each, ReLU), output layer (1 unit, Sigmoid).

Compile ANN → Optimizer: Adam, Loss: Binary Crossentropy, Metric: Accuracy.

Train ANN → Batch size: 32, Epochs: 100.

Predict & Evaluate → Predict on test set, convert probabilities to 0/1, compute confusion matrix and accuracy.

🎯 Importance

Helps businesses retain customers proactively.

ANN captures complex patterns better than traditional models.

Supports targeted marketing to reduce churn.
