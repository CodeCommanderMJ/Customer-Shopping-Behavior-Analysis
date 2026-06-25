# 🛍️ Customer Shopping Behavior Analysis

> Analyzing 3,900 retail transactions to uncover spending patterns, customer segments, and product preferences — driving smarter business decisions.

---

## 📌 Project Overview

A leading retail company wanted to better understand its customers' shopping behavior to improve sales, satisfaction, and long-term loyalty. This project delivers end-to-end analysis using **Excel**, **PostgreSQL**, and **Power BI** to answer:

> *"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"*

---

## 📂 Repository Structure

```
consumer-behavior-analysis/
│
├── excel/
│   └── consumer_data.xlsx           # Cleaned and transformed dataset
│
├── sql/
│   └── queries.sql                  # All PostgreSQL business queries
│
├── powerbi/
│   └── dashboard.pbix               # Interactive Power BI dashboard
│
├── data/
│   └── raw_dataset.csv              # Original dataset (3,900 rows, 18 columns)
│
└── README.md
```

---

## 🗃️ Dataset Summary

| Property | Details |
|---|---|
| Rows | 3,900 |
| Columns | 18 |
| Missing Data | 37 null values in `Review Rating` (imputed using category median) |

**Key Features:**
- **Demographics:** Age, Gender, Location, Subscription Status
- **Purchase Details:** Item, Category, Amount (USD), Season, Size, Color
- **Behavior:** Discount Applied, Previous Purchases, Frequency, Review Rating, Shipping Type

---

## 🔧 Tools & Technologies

| Tool | Purpose |
|---|---|
| **Excel / Power Query** | Data cleaning, transformation, feature engineering |
| **PostgreSQL** | Structured querying and business transaction analysis |
| **Power BI** | Interactive dashboard and data visualization |

---

## 📊 Data Preparation (Excel)

- Handled **37 missing values** in `Review Rating` using median per product category
- Renamed columns to **snake_case** for consistency
- Created `age_group` column by binning customer ages
- Created `purchase_frequency_days` from purchase frequency data
- Dropped `promo_code_used` (confirmed redundant with `discount_applied`)

---

## 🗄️ SQL Analysis (PostgreSQL)

10 business queries were run to extract actionable insights:

| # | Query | Key Finding |
|---|---|---|
| 1 | Revenue by Gender | Male: $157,890 / Female: $75,191 |
| 2 | High-Spending Discount Users | 839 customers spent above average even with discounts |
| 3 | Top 5 Products by Rating | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | Shipping Type Comparison | Express ($60.48) vs Standard ($58.46) avg spend |
| 5 | Subscribers vs Non-Subscribers | Avg spend nearly equal (~$59.49 vs $59.87) |
| 6 | Discount-Dependent Products | Hat (50%), Sneakers (49.66%), Coat (49.07%) |
| 7 | Customer Segmentation | Loyal: 3,116 / Returning: 701 / New: 83 |
| 8 | Top 3 Products per Category | Jewelry, Blouse, Sandals, Jacket lead their categories |
| 9 | Repeat Buyers & Subscriptions | 2,518 non-subscribers vs 958 subscribers among repeat buyers |
| 10 | Revenue by Age Group | Young Adult: $62,143 / Middle-aged: $59,197 / Adult: $55,978 / Senior: $55,763 |

---

## 📈 Power BI Dashboard

An interactive dashboard was built with the following KPIs and visuals:

- **KPI Cards:** 3.9K Customers | $59.76 Avg Purchase | 3.75 Avg Rating
- **Donut Chart:** 27% Subscribers vs 73% Non-Subscribers
- **Bar Charts:** Revenue & Sales by Category and Age Group
- **Slicers:** Filter by Subscription Status, Gender, Category, Shipping Type

---

## 💡 Business Recommendations

1. **Boost Subscriptions** — Only 27% of customers subscribe. Promote exclusive perks to convert the remaining 73%.
2. **Customer Loyalty Programs** — With 3,116 loyal customers, reward programs can deepen retention.
3. **Review Discount Policy** — 839 high-spenders used discounts yet still spent above average — discounts don't always hurt margins.
4. **Product Positioning** — Promote top-rated items (Gloves, Sandals, Boots) prominently in campaigns.
5. **Targeted Marketing** — Focus on Young Adults (highest revenue: $62,143) and Express Shipping users (higher avg spend).

---

## 👤 Author

**[Your Name]**  
[LinkedIn Profile URL] | [Email]

---

## 📄 License

This project is for educational and portfolio purposes.
