🍽 Sentiment Analysis of Restaurant Reviews
📌 Overview

This project performs sentiment analysis on restaurant reviews using Naive Bayes.
The dataset Restaurant_Reviews.tsv contains reviews labeled as liked (1) or not liked (0).
The goal is to predict whether a review is positive or negative based on its text.

⚙️ Steps in the Code

Import Libraries → numpy, pandas, matplotlib, re, nltk, sklearn.

Load Dataset → Reviews (Review) and labels (Liked).

Text Preprocessing → Remove punctuation/numbers, lowercase, remove stopwords, apply stemming.

Feature Extraction → Convert text to numerical vectors using Bag of Words (top 1500 words).

Split Dataset → 80% training, 20% testing.

Train Classifier → Gaussian Naive Bayes on training data.

Predict & Evaluate → Test predictions, confusion matrix, accuracy score.

🎯 Importance

Helps businesses understand customer feedback.

Naive Bayes is fast and effective for text classification.

Pipeline can be adapted for larger datasets or other domains (e.g., product reviews).
