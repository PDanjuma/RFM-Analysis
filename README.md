# 📊 RFM Customer Segmentation Analysis

> **Behaviour-based customer segmentation using Recency, Frequency & Monetary scoring — powered by real transactional data.**

---

## 🔍 What is RFM Analysis?

RFM is a **behaviour-based customer segmentation method** that ranks every customer across three dimensions, enabling you to target marketing and retention efforts with precision.

| Dimension | Definition | Why It Matters |
|-----------|-----------|----------------|
| **R — Recency** | How recently a customer made their last purchase | More recent buyers are more engaged and more likely to convert again |
| **F — Frequency** | How often a customer purchases within a given period | Frequent buyers tend to be more loyal and responsive to offers |
| **M — Monetary** | How much a customer has spent in total | Higher spenders are more valuable and worth extra retention effort |

---

## ⚙️ How RFM Scoring Works

### Step 1 — Compute R, F, M
Calculate **recency**, **frequency**, and **monetary** values per customer from order history.

### Step 2 — Assign Decile Ranks
Score each dimension using **decile ranks (1–10)**, where:
- **10 = best** performance on that dimension
- **1 = worst** performance on that dimension

> 1–10 decile scoring is used for finer granularity compared to simpler quintile approaches.

### Step 3 — Combine into a Single RFM Score
Sum R + F + M to produce a **3–30 composite RFM score**.

### Step 4 — Map to Segments
Translate scores into actionable customer segments:

| Score Range | Segment | Description |
|-------------|---------|-------------|
| 27 – 30 | 🏆 **Champion** | Bought recently, buy often, spend the most |
| 21 – 26 | ⭐ **Loyal Customer** | Regular buyers with strong engagement |
| 15 – 20 | 🌱 **Potential Loyalist** | Recent customers with growth potential |
| 10 – 14 | ⚠️ **At Risk** | Were good customers but haven't returned |
| 3 – 9 | 💤 **Inactive / Lost** | Low scores across all three dimensions |

> A score of **30** = perfect Champion. A score of **3** = least engaged customer.

---

## 📈 Dashboard Visuals (Power BI)

The analysis is visualised through three Power BI components:

### 1. 📊 Customer Distribution by Segment *(Bar Chart)*
Shows the count of customers in each RFM segment — quickly reveals where the bulk of your customer base sits and which segments need attention.

### 2. 🎯 KPI Cards
At-a-glance metrics including:
- Total number of customers analysed
- Average RFM score across the base
- Proportion of Champions vs At-Risk customers

### 3. 📋 RFM Segmentation Table
Full customer-level breakdown with individual R, F, M scores, composite RFM score, and assigned segment label — enabling direct CRM action or export.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **SQL** | Data extraction, RFM calculation, decile ranking |
| **Power BI** | Dashboard, visualisations, segmentation table |
