Polynomial Regression with Python
📌 Overview

This project demonstrates Polynomial Regression, a machine learning technique that extends Linear Regression by adding polynomial terms (squared, cubic, etc.) to capture non-linear relationships between variables.

🚀 Why It’s Important

Linear Regression assumes a straight-line relationship between the independent variable (X) and the dependent variable (Y).

However, real-world data often follows more complex, curved patterns.

Polynomial Regression allows the model to fit these curves, leading to more accurate predictions when the relationship is non-linear.

This makes it especially useful in fields like economics, engineering, and science, where trends are rarely perfectly linear.

⚙️ What the Code Does

Loads the dataset (Position_Salaries.csv) → contains job positions, their levels, and salaries.

Builds a Linear Regression model → used as a baseline for comparison.

Transforms the features into polynomial form → adds squared, cubic, and higher-order terms.

Builds a Polynomial Regression model → fits the transformed data.

Visualizes the results → compares Linear vs Polynomial regression curves.

Makes predictions → estimates the salary for a specific position level (e.g., 6.5).
