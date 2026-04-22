# 📊 Customer Segmentation using RFM Analysis (Python)

## 🚀 Project Overview

This project performs **RFM (Recency, Frequency, Monetary) analysis** on an e-commerce dataset to segment customers based on purchasing behavior using a **3-tier scoring model (1–3 scale)**.

The objective is to identify customer value groups and support better marketing and retention strategies.

---

## 📁 Dataset

* **Dataset Name:** Online Retail Dataset
* **Source:** UCI Machine Learning Repository / Kaggle
* **Records:** ~500,000 transactions

### Key Features:

* CustomerID
* InvoiceDate
* InvoiceNo
* Quantity
* UnitPrice

---

## 🛠️ Tools & Technologies

* Python 🐍
* Pandas
* NumPy
* Jupyter Notebook

---

## ⚙️ Project Workflow

### 1️⃣ Data Cleaning

* Removed missing Customer IDs
* Filtered out negative/zero quantities
* Converted date columns to datetime
* Created **TotalPrice = Quantity × UnitPrice**

---

### 2️⃣ RFM Metric Calculation

* **Recency:** Days since last purchase
* **Frequency:** Number of unique transactions
* **Monetary:** Total spending

---

### 3️⃣ RFM Scoring (1–3 Scale)

Customers were scored using **tertiles (quantiles into 3 groups)**:

* **R Score (1–3):** Higher = more recent
* **F Score (1–3):** Higher = more frequent
* **M Score (1–3):** Higher = higher spending

👉 Final Score:

```bash
RFM_Score = R + F + M
```

👉 Score Range:

* Minimum = 3
* Maximum = 9

---

### 4️⃣ Customer Segmentation

Based on total RFM score:

| Score Range | Segment              |
| ----------- | -------------------- |
| 8 – 9       | High Value Customers |
| 6 – 7       | Potential Loyalists  |
| 4 – 5       | Low Value Customers  |
| 3           | Lost Customers       |

---

## 📊 Sample Output

| CustomerID | Recency | Frequency | Monetary | RFM Score | Segment              |
| ---------- | ------- | --------- | -------- | --------- | -------------------- |
| 17850      | 10      | 50        | 5000     | 9         | High Value Customers |
| 13047      | 120     | 5         | 300      | 4         | Low Value Customers  |

---

## 📈 Key Insights

* A small group of customers contributes the highest revenue
* Many customers fall into mid-tier (potential growth segment)
* Identified low-engagement customers who may churn

---

## 🎯 Business Impact

* Helps target **high-value customers** for retention
* Identifies **potential customers** for upselling
* Detects **lost customers** for re-engagement campaigns

---

## 📌 Future Improvements

* Add visualizations (Matplotlib / Seaborn)
* Build dashboard (Power BI / Streamlit)
* Automate segmentation pipeline

---

## 📎 How to Run the Project

```bash
# Clone repository
git clone https://github.com/your-username/rfm-analysis.git

# Install dependencies
pip install pandas numpy

# Run notebook
jupyter notebook
```

---

## 🙋‍♂️ Author

**Your Name**
Aspiring Data Analyst
