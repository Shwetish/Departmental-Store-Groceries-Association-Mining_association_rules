# Departmental-Store-Groceries-Association-Mining_association_rules
Analyzes daily departmental store transactions using market basket analysis to uncover frequent itemsets, generate actionable association rules, and improve bundle marketing strategies.

# 🛒 Departmental Store: Market Basket Analysis & Association Mining

## 1. Business Problem

### 1.1. What is the business objective?
* **Optimizing Inventory & Sales:** Analyze daily transaction records from a local departmental store to understand consumer purchasing behavior[cite: 2].
* **Association Mining:** Uncover hidden item associations (e.g., what products are frequently bought together) to implement strategic product bundling, cross-selling, and targeted promotional campaigns.

### 1.2. Are there any constraints?
* **High Item Variety:** Managing a dense matrix of diverse grocery products without creating an overwhelming volume of redundant or trivial association rules.
* **Support & Confidence Tuning:** Selecting optimal thresholds to ensure generated rules are statistically sound and actionable for store management.

---

## 2. Data Dictionary (`Groceries.csv`)

| Feature Name | Data Type | Description |
| :--- | :--- | :--- |
| **Transaction / Basket ID** | Integer / String | Unique identifier representing a single customer checkout session. |
| **Item / Product Description** | Categorical | Names of the individual grocery items purchased in a transaction. |

---

## 3. Data Pre-processing

### 3.1. Data Cleaning & Feature Engineering
* **Data Transformation:** Processed raw transactional records into a one-hot encoded boolean matrix (items as columns, transactions as rows) suitable for association rule mining.
* **Missing Value Check:** Inspected and cleaned data rows for formatting anomalies or incomplete item entries.

---

## 4. Model Building

### 4.1. Application of Apriori Algorithm
* Implemented the Apriori algorithm via Python libraries (e.g., `mlxtend`) to extract frequent itemsets meeting the minimum support criteria.
* Filtered and evaluated the rules based on **Confidence** and **Lift** metrics to identify strong product relationships.

### 4.2. Frequent Itemsets & Rule Visualization
* Generated frequent itemsets and visualized association metrics using support-confidence scatter plots and network graphs to interpret product affinity clearly.

### 4.3. Work on Codes
* The complete source code implementation is stored in the `Groceries.py` file.

---

## 5. Deployment

### 5.1. Deploy Solutions
* The insights can be deployed as an automated reporting script for store managers or integrated into point-of-sale recommendation displays and weekly promotional flyers.

---

## 6. Business Impact & Benefits
* **Optimized Product Placement:** Placing strongly associated items near each other in store aisles to encourage impulse buying and increase average basket size.
* **Targeted Discounts:** Designing bundle offers for high-lift product pairs to drive overall departmental sales and enhance customer satisfaction.
