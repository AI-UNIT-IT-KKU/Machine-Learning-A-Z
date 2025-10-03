Support Vector Regression (SVR) Example
📌 Overview

This project demonstrates how to use Support Vector Regression (SVR) to predict salaries based on position levels.

SVR is a powerful regression technique that works well for non-linear relationships by using kernels such as the RBF (Radial Basis Function).

🚀 Why It’s Important

Traditional Linear Regression may fail when data has curved or complex patterns.

SVR, with kernels, can map input data into higher dimensions, allowing it to capture these non-linear relationships.

It is widely used in finance, business forecasting, and scientific research where accurate predictions on complex data are needed.

⚙️ What the Code Does

Importing libraries → Load essential Python libraries for data handling, visualization, and machine learning.

Loading the dataset (Position_Salaries.csv) → Contains position levels and their corresponding salaries.

Feature selection → Separate independent variable (position level) and dependent variable (salary).

Data preprocessing → Apply feature scaling to standardize values (very important for SVR).

Training the SVR model → Fit the SVR with the RBF kernel on scaled data.

Making predictions → Predict salaries for new position levels.

Visualizing results → Plot actual data points and the SVR regression curve.

Improving plot resolution → Use smaller steps in X to get a smoother regression curve.
