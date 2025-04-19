# Insurance-Claims-Data-Analysis-Case-Study

## Overview

This project is a hands-on case study focused on analyzing insurance claim data. The goal is to derive actionable insights from customer claim behaviors by merging two datasets—claims and customer demographics. It includes data preparation, feature engineering, hypothesis testing, segmentation, and visualization.

---

## 📁 Files in the Repository

- `Insurance Claims Case Study.ipynb`: Jupyter notebook performing end-to-end analysis.
- `claims.csv`: Dataset containing claim details (assumed location based on script).
- `cust_demographics.csv`: Dataset containing customer demographic information.

---

## Key Tasks Performed

### 1. Data Preparation
- Read and merged two datasets: claims and customer demographics.
- Converted columns like `claim_date`, `DateOfBirth` to datetime.
- Cleaned `claim_amount` by removing dollar signs and casting to float.
- Created an `alert_flag` for claims not reported to police.
- Removed duplicate customers to maintain one row per customer.

### 2. Missing Value Treatment
- Imputed missing values:
  - Continuous: mean (`claim_amount`)
  - Categorical: mode (`total_policy_claims`)

### 3. Feature Engineering
- Calculated `age` from `DateOfBirth` and `claim_date`.
- Categorized customers into `Children`, `Youth`, `Adult`, and `Senior`.

### 4. Segment Analysis
- Analyzed average claim amounts across different customer segments.
- Analyzed total claim amounts based on incident causes.
- Filtered claims done at least 20 days before a specific date.

---

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Insights & Outcomes

- Identified behavioral differences between segments.
- Created useful customer age categories.
- Found patterns in police reporting behavior and claim types.
- Performed temporal and categorical analysis on claims.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/insurance-claims-analysis.git
