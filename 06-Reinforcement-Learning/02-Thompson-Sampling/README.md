📊 Thompson Sampling for Ad Selection
📌 Overview

This project demonstrates Thompson Sampling, a multi-armed bandit algorithm, applied to online ad selection.
The dataset Ads_CTR_Optimisation.csv contains simulated user interactions:

Rows → users (rounds)

Columns → ads

Values → 1 if the user clicked the ad, 0 otherwise

The goal is to maximize total clicks by selecting the best-performing ads over multiple rounds.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, random.

Load Dataset → Load the CSV file with user interactions.

Initialize Variables → Track selected ads, rewards per ad, and total clicks.

Thompson Sampling Algorithm →

For each round, draw a random value from the Beta distribution for each ad.

Select the ad with the highest sample.

Update reward counters based on clicks.

Visualize Results → Histogram of how many times each ad was selected.

🎯 Importance

Balances exploration vs. exploitation in decision-making.

Helps advertisers optimize ad selection to maximize click-through rate (CTR).

Automatically adapts to changing reward probabilities.
