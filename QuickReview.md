# 📘 Quick Review 

## 🔹 Preprocessing (Data Cleaning & Preparation)

| Step | What It Does | Why It’s Important | Example |
|------|---------------|--------------------|----------|
| **Handling Missing Values** | Fill or remove null values. | Missing data can bias results. | Fill with mean/median using `df.fillna()` |
| **Encoding Categorical Data** | Convert text to numbers. | Models only handle numeric input. | One-hot encoding → “Male/Female” → [1, 0] |
| **Feature Scaling** | Normalize or standardize features. | Keeps features on same scale. | Use `StandardScaler()` or `MinMaxScaler()` |
| **Outlier Removal** | Remove extreme values. | Prevents model distortion. | Remove if Z > 3 or outside IQR |
| **Train/Test Split** | Split data into training & testing. | Avoids overfitting. | Use `train_test_split()` |
| **Balancing Data** | Fix imbalance in classification. | Prevents bias toward majority class. | Use SMOTE or undersampling |

---
## 🔹 PCC (Pearson Correlation Coefficient)
**What it does:**  
Measures the **linear relationship** between two variables.  

**Why we use it:**  
- Best when the relationship is **straight-line (linear)**  
- Sensitive to **outliers**  
- Great for small and clean datasets  

**Values:**  
- +1 → strong positive  
- -1 → strong negative  
- 0 → no correlation  

**Example:**  
As study hours increase, exam score increases → PCC ≈ +1  

---

## 🔹 Partial Correlation
**What it does:**  
Finds the **true effect** of a feature after removing other features’ influence.  

**Why we use it:**  
When PCC is high but the model is weak → helps detect **hidden dependencies**.  

**Example:**  
Age and income may both correlate with sales. Partial correlation shows whether age truly affects sales after removing income’s effect.  

---

## 🔹 Spearman Correlation
**What it does:**  
Measures **monotonic (rank-based)** relationships between variables.  

**Why we use it:**  
- Works when the relationship is **non-linear but ordered**  
- **Robust against outliers**  
- Best for **large datasets**  

**Example:**  
If higher education levels generally mean higher salaries (even if not linear), Spearman captures it.  

---

## 🔹 Kendall Correlation
**What it does:**  
Compares the **agreement between ranked pairs**.  

**Why we use it:**  
- Handles **ties (equal ranks)** better  
- Works best for **small datasets**  
- More statistically robust than Spearman but slower  

**Example:**  
Used to compare two ranking lists, like “performance ranking vs. promotion order”.

---

## 🔹 Heatmap
**What it does:**  
Visualizes correlations between variables using **colors**.  
- Darker → stronger relationship  
- Each square = relationship between two features  

**Why we use it:**  
Quickly detect strong or weak correlations visually.  

**Example:**  
Use `sns.heatmap(df.corr(), annot=True)` to find which features are most related to the target.

---

## 🔹 Information Gain
**What it does:**  
Measures how much a feature **reduces uncertainty** about the target.  

**Why we use it:**  
- Common in **Decision Trees**  
- Great for **categorical data**  

**Example:**  
“Income” gives more info about “Purchase Decision” than “Age” → higher Information Gain.

---

## 🔹 Feature Ranking
**What it does:**  
Orders features based on **importance or predictive power**.  

**Why we use it:**  
- Helps in **Feature Selection**  
- Reduces model complexity  

**Common Methods:**  
`PCC`, `Spearman`, `Kendall`, `Information Gain`, `Chi-Square`, `Mutual Information`, `RFE`  

---

## 🔹 Chi-Square Test
**What it does:**  
Measures dependence between **categorical variables** and the target.  

**Why we use it:**  
To find which categorical features are **statistically related** to the output.  

**Example:**  
Testing if “Gender” significantly affects “Product Choice”.

---

## 🔹 Cramer’s V
**What it does:**  
Gives a **0–1 score** of strength between **categorical variables**.  

**Why we use it:**  
- Easier to interpret than Chi-Square  
- 0 → no relation, 1 → perfect relation  

**Example:**  
Cramer’s V = 0.85 → very strong relationship between “City” and “Product Preference”.

---

## 🔹 Recursive Feature Elimination (RFE)
**What it does:**  
Removes **least important features** step-by-step.  

**Why we use it:**  
- Helps reduce overfitting  
- Keeps only features that improve performance  

**Example:**  
Used with Logistic Regression to remove irrelevant predictors automatically.  

---

## 🔹 Mutual Information
**What it does:**  
Measures **shared information** between feature and target.  

**Why we use it:**  
- Works with both **categorical and continuous** data  
- Detects **non-linear** relationships  

**Example:**  
“Time spent on site” shares more info with “Buy/Not Buy” than “Age”.

---

## 🔹 AUC (Area Under the ROC Curve)
**What it does:**  
Evaluates model’s **classification performance**.  

**Why we use it:**  
- Measures ability to **separate classes**  
- 1.0 = perfect model, 0.5 = random guessing  

**Example:**  
AUC = 0.9 → strong model  
AUC = 0.5 → weak model  

**Tip:**  
If the ROC curve is close to the top-left corner → better performance.

---

## 🔹 Regression Metrics

| Metric | Description | When to Use | Example |
|--------:|--------------|-------------|----------|
| **R²** | Explains how much of the variance in data the model captures. | General regression performance. | R² = 0.85 → model explains 85% of data behavior. |
| **Adjusted R²** | Adjusted for the number of features. | When many features exist. | Higher = better fit with fewer features. |
| **MAE** | Mean Absolute Error (average error). | When all errors are equally important. | MAE = 3 → avg. error = 3 units. |
| **MSE** | Mean Squared Error (squares large errors). | When large mistakes matter more. | MSE = 9 → avg. squared error = 9. |
| **RMSE** | Root Mean Squared Error. | When interpretability in original units is needed. | RMSE = 3 → avg. error = 3 units. |

---

## 🔹 Outlier Detection

### 1️⃣ Visual Methods (for small/medium datasets)
- **Scatter Plot:** Isolated points = outliers.  
- **Box Plot:** Points outside whiskers = outliers.  

### 2️⃣ Statistical Methods (for large datasets)
- **Z-Score:** Points far (e.g. > 3 std dev) from mean are outliers.  
- **IQR (Interquartile Range):** Points outside Q1–Q3 range = outliers.  

**Why we use them:**  
- Visual → best for small data  
- Statistical → better for big data  

---

## 🔹 P-Value
**What it does:**  
Checks if the result could happen **by chance**.  

**Why we use it:**  
- To test **statistical significance**  
- **p < 0.05** → strong evidence against random chance  

**Example:**  
p = 0.03 → statistically significant difference.

---


## 🔹 Model Evaluation Summary

| Model Type | Common Metrics | When to Use | Example |
|-------------|----------------|-------------|----------|
| **Regression** | R², Adjusted R², MAE, MSE, RMSE | Predicting continuous values | Predicting house prices |
| **Classification** | Accuracy, Precision, Recall, F1, AUC | Predicting categories | Spam detection |
| **Clustering** | Silhouette Score, Davies–Bouldin Index | Unsupervised tasks | Customer segmentation |

---

✅ **Final Tip:**  
Always preprocess your data → select the right features → evaluate the model using the right metric.  
Good preprocessing = better performance & reliable results.

---
