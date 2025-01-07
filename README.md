---
### **Credit Card Fraud Detection**
---
#### **Context:**

Credit card fraud detection is crucial to protect customers from unauthorized charges and ensure the integrity of financial transactions. Accurate and timely identification of fraudulent transactions helps prevent financial losses and maintains customer trust.

#### **Dataset Overview:**

This dataset contains credit card transaction records from European cardholders during a two-day period in September 2013. It includes 284,807 transactions, of which only 492 (0.172%) are fraudulent, making it highly imbalanced.

Key characteristics of the dataset:

**Features:**

1. Numerical variables derived from a Principal Component Analysis (PCA) transformation.

2. Original feature details are unavailable due to confidentiality constraints.

3. V1, V2, … V28: Principal components from PCA.

4. Time: Seconds elapsed since the first transaction in the dataset.

5. Amount: Transaction value, useful for cost-sensitive learning.


**Target Variable:**

Class: Indicates whether a transaction is fraudulent (1) or not (0).


#### **Challenge:**

The extreme class imbalance poses a significant challenge: fraud cases account for just 0.172% of all transactions.


#### **Objective:**

To address the imbalance and ensure robust evaluation, we recommend using the Area Under the Precision-Recall Curve (AUPRC) as the primary performance metric. This measure is particularly suited for datasets with skewed class distributions and helps assess the model's ability to correctly identify frauds while minimizing false positives.


**Dataset Link:**

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
