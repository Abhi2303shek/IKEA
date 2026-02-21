# 🛍️ IKEA Retail Sales Analysis (SQL Case Study)

## 📌 Project Overview

This project analyses a real-world retail transaction dataset using **MySQL** to uncover customer behaviour, product performance, sales trends, and business insights.

The goal was not just querying data — but answering **real business questions retailers care about**:

* When do customers shop?
* Who are the most valuable customers?
* Which products drive revenue vs volume?
* How much revenue is lost due to returns?
* Can we identify VIP customers?

---

## 🧱 Dataset Information

The dataset contains transactional retail data with the following attributes:

| Column      | Description                         |
| ----------- | ----------------------------------- |
| invoiceno   | Unique order identifier             |
| date        | Purchase date                       |
| time        | Purchase time                       |
| stockcode   | Product code                        |
| description | Product name                        |
| quantity    | Units purchased (negative = return) |
| unitprice   | Price per unit                      |
| custid      | Customer ID                         |
| country     | Customer location                   |

---

## 🧹 Data Cleaning (SQL + Pandas)

Before analysis, the dataset required cleaning:

* Split `InvoiceDate` → `Date` & `Time`
* Converted European date format → MySQL format
* Handled NULL & blank values during import
* Fixed datatype issues (`InvoiceNo` stored as VARCHAR due to cancellations)
* Managed negative quantities (returns)

---

## 📊 Key Business Insights

### 🕒 Customer Shopping Behaviour

* Sales peak during specific hours of the day
* Weekdays generate more revenue than weekends
* Evening shopping contributes high order counts

👉 Helps staffing & promotion scheduling

---

### 👤 Customer Analytics

* Identified repeat purchase cycle using purchase gap analysis
* Segmented customers into High / Medium / Low value
* Found **VIP customers (Top 5%)** using percentile ranking
* Detected one-time buyers and churned customers

👉 Helps retention & loyalty programs

---

### 🛒 Product Performance

* Top products by revenue differ from top products by quantity
* Some items sell frequently but generate low revenue
* Some premium items sell rarely but drive profit

👉 Helps inventory & pricing strategy

---

### 🔁 Returns & Revenue Loss

* Returns detected using negative quantity & cancellation invoices
* Certain products have disproportionately high return rates
* Calculated revenue lost due to returns

👉 Helps quality control decisions

---

### 🌍 Geographic Trends

* Revenue contribution varies significantly by country
* Different regions prefer different product types

👉 Helps market expansion planning

---

## 🧠 Advanced Analytics Performed

* RFM Analysis (Recency, Frequency, Monetary)
* Customer Segmentation
* Repeat Purchase Cycle Detection
* Cohort Identification
* Pareto (80/20) Customer Rule
* Order Pattern Analysis
* Time-based Sales Analysis

---

## 🛠️ Tech Stack

* **MySQL 8** → Data analysis & querying
* **Pandas** → Pre-processing & formatting
* SQL Window Functions → Advanced analytics

---

## 📈 Business Value

This project simulates how a retail company would use transaction data to:

* Optimise inventory
* Improve marketing targeting
* Identify high-value customers
* Reduce product returns
* Predict repeat purchases

---

## 📂 Project Structure

```
IKEA-Retail-SQL-Analysis/
│── dataset/
│── cleaning/
│── queries.sql
│── insights.md
│── README.md
```

---

## 🚀 What I Learned

* Handling messy real-world datasets
* Writing analytical SQL beyond basic SELECT queries
* Using window functions for behavioural analysis
* Translating data into business decisions

---

## 📬 Author

**Abhishek Singh**
Aspiring Data Analyst | SQL • Python • Power BI
