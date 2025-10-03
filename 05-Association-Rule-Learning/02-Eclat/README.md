🛒 Market Basket Analysis (elcat)
📌 Overview

elcat is a simple Market Basket Analysis project using the Apriori algorithm (apyori library).
It analyzes the dataset Market_Basket_Optimisation.csv, where each row represents a shopping basket, and extracts frequent product associations.
The program displays the top 10 product pairs with the highest support values.

⚙️ How it works

Import Libraries

numpy, pandas, matplotlib → For data handling and visualization.

apyori → To implement the Apriori algorithm.

Load Dataset

The dataset is read without headers (header=None).

Each row (transaction) is converted into a list of purchased items.

Prepare Transactions

Creates a list of 7501 transactions, each with up to 20 items.

Apply Apriori

Algorithm parameters:

Inspect Results

Extracts Product 1 (LHS), Product 2 (RHS), and Support.

Stores results in a pandas DataFrame.

Display Results

Shows the top 10 product pairs ranked by support.

🎯 Why it’s useful

Identifies products that are frequently bought together.

Helps businesses improve product placement and cross-selling strategies.

Can inspire bundle deals and promotions.
