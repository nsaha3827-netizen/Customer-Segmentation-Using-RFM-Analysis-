# Customer-Segmentation-Using-RFM-Analysis-
# 📊 Customer Segmentation using RFM Analysis (Python)

## 🚀 Project Overview

This project performs **RFM (Recency, Frequency, Monetary) analysis** on a real-world e-commerce dataset to segment customers based on their purchasing behavior.

The goal is to help businesses identify:

* High-value customers
* Loyal customers
* At-risk customers
* Low-engagement customers

---

## 📁 Dataset

* **Dataset Name:** Online Retail Dataset
* **Source:** UCI Machine Learning Repository / Kaggle
* **Records:** ~500,000 transactions
* **Features Used:**

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
* Converted date columns to datetime format
* Created **TotalPrice** column

---

### 2️⃣ RFM Metric Calculation

* **Recency:** Days since last purchase
* **Frequency:** Number of transactions
* **Monetary:** Total amount spent

---

### 3️⃣ RFM Scoring

* Applied **quantile-based scoring (1–4 scale)**
* Generated individual scores:

  * R Score
  * F Score
  * M Score

---

### 4️⃣ Customer Segmentation

Customers were segmented into groups such as:

* 🏆 Champions
* 🤝 Loyal Customers
* ⚠️ At Risk
* 💤 Others

---

## 📊 Key Insights

* A small percentage of customers contribute to a large portion of revenue
* High-frequency customers are not always the highest spenders
* Identified customers who are likely to churn

---

## 📈 Sample Output

| CustomerID | Recency | Frequency | Monetary | Segment   |
| ---------- | ------- | --------- | -------- | --------- |
| 17850      | 10      | 50        | 5000     | Champions |
| 13047      | 120     | 5         | 300      | At Risk   |

---

## 🎯 Business Impact

* Enables targeted marketing campaigns
* Improves customer retention strategies
* Helps in personalized recommendations

---

## 📌 Future Improvements

* Add data visualization (Seaborn / Matplotlib)
* Build interactive dashboard (Power BI / Streamlit)
* Deploy as a web app

---

## 📎 How to Run the Project

```bash
# Clone repository
git clone https://github.com/your-username/rfm-analysis.git

# Install dependencies
pip install pandas numpy

# Run Jupyter Notebook
jupyter notebook
```

---

## 🙋‍♂️ Author

**Your Name**
Aspiring Data Analyst

---
