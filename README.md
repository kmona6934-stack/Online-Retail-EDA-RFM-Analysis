#  E-Commerce Sales & Customer Behavior Analysis

##  Business Overview
This project presents an end-to-end data analysis of an online retail dataset containing over **541,000 transaction records**. The primary objective is to derive actionable business insights, identify key sales drivers, analyze temporal purchasing patterns, and implement **RFM Customer Segmentation** to optimize marketing strategies and customer retention.

---

##  Key Metrics & Findings
* **Total Revenue Generated:** ~$8.91M
* **Average Order Value (AOV):** ~$480
* **Peak Purchasing Hours:** 10:00 AM – 3:00 PM (Highest order volume at 12:00 PM).
* **Seasonal Trends:** Significant revenue spikes during Q4 (September – November), aligned with holiday shopping seasons.
* **Top International Markets:** Netherlands, EIRE (Ireland), and Germany (excluding the UK).

---

##  Project Architecture & Workflow

### 1. Data Cleaning & Feature Engineering
* Handled missing values (e.g., missing `CustomerID` entries).
* Filtered out negative quantities and unit prices corresponding to cancelled orders and adjustments.
* Engineered critical datetime features (`Year`, `Month`, `Hour`, `DayOfWeek`) and calculated `TotalAmount` ($Quantity \times UnitPrice$).

### 2. Exploratory Data Analysis (EDA)
* **Product Performance:** Identified top revenue-generating items vs. top sold items by volume.
* **Geographic Distribution:** Analyzed country-level performance to spot key international expansion targets.
* **Temporal Patterns:** Tracked monthly revenue velocity and hour-of-day order density.

### 3. Customer Segmentation (RFM Analysis)
Customers were evaluated across three core behavioral metrics:
* **Recency ($R$):** Days elapsed since the customer's last purchase.
* **Frequency ($F$):** Total number of completed orders.
* **Monetary ($M$):** Aggregate monetary value spent.

Using quantile scoring ($1–4$), customers were classified into distinct business segments:
* **VIP / Champions:** High-frequency, high-value active shoppers.
* **Loyal Customers:** Consistent buyers maintaining regular interaction.
* **At-Risk / Need Attention:** Historically valuable customers showing declining recent activity.
* **Lost Customers:** Inactive accounts requiring targeted win-back campaigns.

---

##  Strategic Recommendations
1. **Win-Back Campaigns:** Target the large *Lost Customers* segment with automated email re-engagement discounts.
2. **VIP Retention:** Establish exclusive perks and priority support for *VIP / Champions* to maximize CLV (Customer Lifetime Value).
3. **Marketing Timing:** Align push notifications and ad spend with peak ordering hours ($10 \text{ AM} - 3 \text{ PM}$).
4. **Regional Expansion:** Scale localized logistics and promotions in high-performing international hubs like the Netherlands and Germany.

---

##  Tech Stack
* **Language:** Python
* **Environment:** Jupyter Notebooks / VS Code
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
