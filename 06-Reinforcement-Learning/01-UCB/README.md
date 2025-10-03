🎯 Upper Confidence Bound (UCB) for Ad Selection
📌 Overview

This project shows the UCB algorithm for selecting ads to maximize clicks over multiple users.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, math.

Load Data → Ads_CTR_Optimisation.csv with clicks (1) or no clicks (0).

Initialize Variables → Track selected ads, number of selections, total rewards.

UCB Algorithm → For each round, choose the ad with the highest upper confidence bound.

Visualize Results → Histogram of how many times each ad was selected.

🎯 Importance

Helps select ads optimally to increase click-through rate.

Balances exploration (trying new ads) and exploitation (choosing best ads).
