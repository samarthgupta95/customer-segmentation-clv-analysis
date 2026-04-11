# Customer Segmentation & Customer Lifetime Value (CLV) Analysis

## 📌 Project Overview
This project analyzes customer behavior for a UK-based e-commerce business to identify high-value segments and optimize marketing and retention strategies.

Using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering, customers were segmented based on purchasing behavior, and a CLV proxy was developed to quantify long-term value across segments.

---

## 🎯 Business Problem
The business currently treats all customers equally — applying the same marketing efforts, communication frequency, and discount strategies across the board.

This leads to:
- Inefficient marketing spend  
- Underinvestment in high-value customers  
- Poor retention of valuable segments  

The objective is to identify **who the most valuable customers are**, how value is distributed, and how strategy should differ across segments.

---

## 📊 Dataset & Scope
- **Customers:** 4,338  
- **Transactions:** 392,692  
- **Time Period:** Dec 2010 – Dec 2011  
- **Domain:** UK-based online retail  

---

## 🧠 Approach

### 1. RFM Feature Engineering
- Aggregated transaction data into customer-level profiles  
- Applied log transformation to handle skewness  
- Standardized features for clustering  

### 2. Customer Segmentation
- K-Means clustering applied on scaled RFM features  
- Optimal clusters selected using:
  - Elbow Method  
  - Silhouette Score (**0.57**)  
- Final segmentation: **4 distinct customer groups**

### 3. CLV Proxy
- Developed an annualized CLV proxy based on observed customer behavior  
- Used to compare long-term value across segments and guide strategic decisions  

---

## 🔍 Key Insights

- **Revenue is highly concentrated:**  
  Top **13% of customers (Champions)** drive **63.12% of total revenue**

- **Frequency is the primary driver of CLV**

- **Majority of customers are under-engaged**

- **Single-order customers are the biggest churn risk (~34%)**

- **Recoverable segment exists but requires selective targeting**

---

## 👥 Segment Snapshot

| Segment | Customers | Revenue Contribution | CLV (Approx) |
|--------|----------|--------------------|-------------|
| Champions | 571 | 63.12% | £139K |
| Loyal Customers | 1452 | 26.86% | £25K |
| Potential Loyalists | 1377 | 5.95% | £5.1K |
| At Risk | 938 | 4.07% | £4.8K |

---

## 💡 Business Impact

- Enables **targeted marketing investment**  
- Identifies **high-value segments for retention**  
- Highlights **revenue concentration risk**  
- Supports **CLV-based budget allocation**

👉 Customer value is highly uneven — strategy should reflect that.

---

## ⚡ Recommendation Snapshot

- **Protect Champions** → Retention-first strategy  
- **Grow Loyal Customers** → Increase purchase frequency  
- **Convert Potential Loyalists** → Push second purchase early  
- **Selective Win-Back** → Focus only on high-value at-risk customers  

---

## 📁 Project Assets

- 📓 Notebook: Full analysis and modeling  
- 📊 Dashboard: Power BI report  
- 📂 Dataset: External link below  

---

## 📁 Dataset

Due to size limitations, the dataset is hosted externally:  
👉 [Access Dataset](https://drive.google.com/drive/folders/1XSegvQC3yCJyB07ZycJ5RFc9nHoyZGNc?usp=sharing)

---

## 🛠 Tools & Technologies

- Python (Pandas, NumPy, Scikit-learn)  
- Power BI  
- Jupyter Notebook  

---

## 🚀 Final Takeaway

A small group of high-frequency customers drives the majority of revenue.  
Retention, frequency growth, and targeted engagement are the key levers for sustainable business growth.
