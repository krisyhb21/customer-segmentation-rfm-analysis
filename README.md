# Customer Segmentation Analysis – RFM Model

# Krisna Lathu Syahbana - Business Intelligence

## A. Project Overview

**INDUSTRY:** MSME – Laundry Services

A laundry service business operating in the MSME sector, serving customers with busy lifestyles and limited time for daily household activities. Located near a university campus, the business serves a customer base that may be influenced by academic schedules, student mobility, and seasonal demand patterns.

**ROLE:** Business Intelligence Analyst

Analyzed daily operational transaction data from September 2025 to February 2026, covering late-year activity (September–December 2025) and early-year trends (January–February 2026). The analysis focuses on transforming transactional records into customer behavior insights to support retention strategies, improve customer engagement, and strengthen long-term business performance.

**OBJECTIVE:** Implement RFM Customer Segmentation

Transform raw transactional records into a structured RFM segmentation pipeline by evaluating customer behavior through Recency, Frequency, and Monetary metrics. The objective is to categorize customers into actionable behavioral segments, identify retention opportunities, and support targeted marketing strategies to improve customer lifetime value (CLV).

---

## B. Methodology

### 1. Raw Transaction Data Preparation

Clean and preprocess raw transactional data to ensure consistency and reliability. Aggregate transaction records at the customer level to calculate:

- **Recency:** Number of days since the customer's most recent purchase.
- **Frequency:** Total number of transactions made by each customer.
- **Monetary:** Total spending accumulated by each customer.

### 2. RFM Scoring

Standardize customer behavior by assigning relative quintile scores ranging from 1 to 5 for each RFM metric.

- Recency scores reflect how recently customers made their purchases.
- Frequency scores measure how often customers transact.
- Monetary scores represent customers' total spending.

The scoring process provides a consistent basis for comparing customer purchasing behavior.

### 3. RFM Segmentation

Combine individual RFM scores into three-digit identifiers and apply rule-based mapping using regular expressions (regex) to classify customers into actionable business segments.

The resulting segments include categories such as Champions, Loyal Customers, At Risk, About to Sleep, Need Attention, and Hibernating.

### 4. Data Visualization

Develop interactive treemap visualizations to illustrate the distribution and proportion of customers across RFM segments.

The visualization provides an overview of customer base composition and helps identify segments that require different retention and engagement strategies.

---

## C. Key Findings & Business Implications

### The Insight

The RFM segmentation reveals that **49.2% of customers (221 out of 449)** belong to declining or inactive customer segments: Hibernating, At Risk, About to Sleep, and Need Attention.

This indicates a substantial proportion of customers with weak recent purchasing activity or declining engagement.

Conversely, **Champions and Loyal Customers account for 32.3% of the customer base**, representing a relatively strong core of repeat buyers who contribute to recurring business activity.

Given the business's proximity to a university campus, seasonal demand fluctuations during academic holidays may be one possible factor contributing to customer inactivity. However, further time-series analysis would be required to establish this relationship.

### The Business Implication

The business should prioritize customer reactivation and retention strategies based on each segment's purchasing behavior.

- **At Risk:** Prioritize personalized reactivation campaigns for customers who previously purchased frequently but have not returned recently.
- **Hibernating:** Introduce seasonal promotions and targeted incentives, particularly when university activities and customer mobility begin to recover.
- **About to Sleep & Need Attention:** Encourage repeat purchases through timely reminders, promotional offers, and improved customer engagement.
- **Champions & Loyal Customers:** Strengthen loyalty programs and personalized rewards to maintain purchasing frequency and encourage long-term customer relationships.

By differentiating retention strategies across customer segments, the business can make more efficient use of its marketing resources, strengthen recurring revenue, and reduce excessive dependence on new customer acquisition.

## D. Tools & Technologies

- Python
- Pandas
- Numpy
- Plotly
- Jupyter Notebook

## E. Project Structure

```text
user-retention-analysis/
│
├── data/
│   └── rekapitulasi_transaksi_irlo.xlsx
│
├── docs/
│   └── Project LO II - RFM Segmentation.pdf
│
├── notebooks/
│   └── LO_Project2.ipynb
│
├── outputs/
│   └── treemap_chart.png
│
└── README.md
```

## F. Project Scope

- **Business Domain:** MSME Laundry Services
- **Analysis Period:** September 2025 – February 2026
- **Primary Analysis:** Customer Segmentation with RFM Analysis
- **Business Focus:** Customer Segmentation and Customer Base Evaluation

---

*This project uses anonymized business transaction data for analytical and portfolio purposes.*
