# Insurance-Product-Analysis
Developed a customer profiling prediction pipeline using decision tree modeling and data visualization

## Project Overview
A U.S. insurance company launched a medical add-on product targeting customers aged 65+.  
The goal of this project was to identify high-purchase-propensity users and support targeted marketing.

## My Role
**Data Analyst**

- Built end-to-end customer profiling pipeline
- Performed feature engineering and modeling
- Delivered interpretable decision rules for business teams

## Business Impact
- Constructed customer persona system from scratch
- Improved customer acquisition by **14%**

---

## Methodology

### 1. Exploratory Data Analysis
- Grouped features by semantic categories
- Cleaned abnormal and unmapped labels
- Analyzed demographics, health, investment, income, and lifestyle attributes
- Visualizations: frequency plots, histograms, density plots, correlation heatmaps

### 2. Data Preprocessing
- Train/test split before imputation
- Missing value handling: median, mode, replacement strategies

### 3. Feature Engineering
- Binary encoding (0-1 variables)
- One-hot encoding for categorical variables
- Column standardization before encoding

### 4. Modeling
Model: **Decision Tree Classifier**

- Baseline performance evaluation
- Hyperparameter tuning via Grid Search
- Evaluation metrics:
  - Accuracy
  - Precision
  - Recall
  - ROC-AUC
- Extracted interpretable decision rules

---

## Key Concepts Applied
- Correlation analysis for feature selection
- Categorical variable encoding
- Grid Search parameter optimization
- Classification performance evaluation (ROC-AUC)

---

## Tech Stack
Python: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

## Evaluation Metrics

### Confusion Matrix

|               | Actual Positive | Actual Negative |
|--------------|---------------:|---------------:|
| Pred Positive | TP | FP |
| Pred Negative | FN | TN |

---

### Metric Definitions

$$
\[
\textbf{Precision} = \frac{TP}{TP + FP}
\]

\[
\textbf{Recall (TPR)} = \frac{TP}{TP + FN}
\]

\[
\textbf{FPR} = \frac{FP}{FP + TN}
\]
$$

---

### Interpretation

| Metric | Denominator | Question Answered | Intuition |
|------|------|------|------|
| Precision | TP + FP | Are predicted positives accurate? | Recommendation quality |
| Recall / TPR | TP + FN | Are real positives captured? | Coverage ability |
| FPR | FP + TN | How many negatives are falsely flagged? | False alarm rate |

---

**Precision** measures the quality of selected customers — how many predicted positives actually purchase.  

**Recall** measures the coverage — how many actual buyers are successfully captured by the model.​​​
