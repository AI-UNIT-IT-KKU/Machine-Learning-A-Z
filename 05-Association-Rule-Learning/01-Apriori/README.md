🛒 Market Basket Analysis using Apriori
📌 Overview

This project demonstrates Market Basket Analysis using the Apriori algorithm with the Market_Basket_Optimisation.csv dataset.
The dataset contains transactional data of items purchased together, and Apriori helps to discover association rules between products.

⚙️ Steps in the Code

Import libraries

numpy, pandas, matplotlib → For data handling and visualization.

apyori → For running the Apriori algorithm.

Load dataset

Read the CSV file and convert each row into a list of purchased items.

Prepare transactions

Transform rows into lists of strings (handling empty cells).

Run Apriori

Apply the Apriori algorithm with chosen thresholds:

min_support = 0.003 → At least ~22 transactions.

min_confidence = 0.2 → Rules must have ≥20% confidence.

min_lift = 3 → Only strong associations are kept.

min_length = 2, max_length = 2 → Consider rules between pairs of items.

Parse results

Extract left-hand side (LHS), right-hand side (RHS), support, confidence, and lift values.

Visualization / Display

Print or return the top rules sorted by lift in a pandas DataFrame.

🎯 Importance

Market Basket Analysis helps businesses gain insights such as:

Frequent item combinations → Discover which products are often bought together.

Product placement & cross-selling → Improve in-store or online recommendations.

Targeted promotions → Design discounts, bundles, and marketing campaigns.

This analysis supports retail strategies, sales growth, and customer satisfaction.
