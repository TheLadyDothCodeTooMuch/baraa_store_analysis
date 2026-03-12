# BarStore Analysis - Customer & Product Insights

BarStore lacked the clear insights needed to distinguish between casual buyers and loyal advocates, or to identify which products were truly driving profitability. This project solves that by converting raw transaction logs into automated analytical views that pinpoint growth opportunities, customer loyalty patterns, and overall product health. The result is a streamlined system that allows stakeholders to identify top-tier customers and revenue trends at a glance.

---

## 🚀 Key Business Objectives
* **Automated Customer Profiling:** Built a system to instantly distinguish high-value VIP customers from new or irregular buyers.
* **Product Performance Tiering:** Established a ranking system to flag High-Performers and identify underperforming stock needing marketing intervention.
* **Retention & Engagement:** Developed Recency metrics to pinpoint inactive users, enabling data-driven win-back campaigns.
* **Revenue Efficiency:** Calculated Average Order Value (AOV) and Monthly Spend to identify the most profitable paths to growth.

---

## 🧱 Analytical Views

### 1. data_analysis_customers
**Purpose:** Identify high-value customers, detect inactive users, and uncover retention opportunities.



* **Total Spend & Order Frequency:** Tracks the absolute financial contribution of every user.
* **Customer Recency:** Measures months since last purchase to trigger re-engagement alerts for the marketing team.
* **Loyalty Classification:** Dynamically tiers customers into VIP, Regular, or New based on their spend and lifespan in the ecosystem.
* **Diversity Metrics:** Tracks how many unique products a customer has explored to gauge brand penetration.

### 2. data_analysis_products
**Purpose:** Evaluate product-market fit, monitor sales trends, and guide inventory decisions.



* **Revenue Classification:** Automatically labels products as High-Performer, Mid-Range, or Low-Performer based on a $10,000+ sales threshold.
* **Reach Analysis:** Measures unique customer engagement for every product to differentiate niche items from mass-market hits.
* **Product Lifespan & Recency:** Tracks the maturity of each product line from its launch date to its most recent sale.
* **Efficiency Metrics:** Breaks down average revenue per order and per month to identify top-tier inventory.

---

## 🧠 Design Logic
* **Safe Division:** Implemented CASE statements to prevent Division by Zero errors in AOV calculations.
* **Dynamic Age Calculation:** Uses DATEDIFF against current system time to ensure customer demographics remain accurate as time passes.
* **Medallion Ready:** These views pull directly from the Gold Layer, ensuring they utilize the most polished and validated data available in the warehouse.

---


