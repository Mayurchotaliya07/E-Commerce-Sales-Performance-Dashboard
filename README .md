<div align="center">

# 📊 E-Commerce Sales Performance Dashboard (2021–2023)

### An Interactive Microsoft Excel Dashboard for Retail Sales & Customer Behavior Analysis

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-0078D4?style=for-the-badge&logo=powerquery&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Data%20Analytics-0A66C2?style=for-the-badge&logo=googleanalytics&logoColor=white)
![Dashboard](https://img.shields.io/badge/Dashboard-FF6F00?style=for-the-badge&logo=databricks&logoColor=white)
![Pivot Table](https://img.shields.io/badge/Pivot%20Table-2E8B57?style=for-the-badge&logo=microsoftexcel&logoColor=white)

</div>

![Dashboard Banner](assets/dashboard_banner.png)
<p align="center"><em>📌 Replace this with a full-width screenshot or GIF of the live dashboard</em></p>

---

## 📌 1. Project Overview

This project is a fully interactive **Excel-based sales performance dashboard** built on a real-world **E-Commerce Customer Shopping dataset** covering transactions from **January 2021 to March 2023** across ten shopping malls in Istanbul. The dataset contains **99,457 individual transactions**, each capturing customer demographics, product category, quantity purchased, price, payment method, and shopping mall.

The goal was to turn a flat, unformatted transactional dataset into a **decision-ready business intelligence tool** — the kind of dashboard a retail analytics or e-commerce team could actually use to track revenue, understand customer segments, and identify growth opportunities. Everything was built natively in Excel: from data cleaning in **Power Query**, to calculated fields with **formulas**, to a fully **slicer-driven, chart-rich dashboard** that updates in real time as filters are applied.

This project demonstrates the complete analytics workflow — **ingest → clean → transform → analyze → visualize → recommend** — using only spreadsheet tools, making it a strong showcase of practical, job-ready Excel skills.

## 🎯 2. Objectives

- 🧹 Clean and structure raw transactional data using Power Query
- 🧮 Engineer calculated fields (Total Revenue, Month, Year, Age Group) to enable deeper analysis
- 📊 Build dynamic Pivot Tables and Pivot Charts to summarize sales across multiple dimensions
- 🎛️ Design an intuitive, slicer-driven dashboard for non-technical stakeholders
- 📈 Surface actionable insights on category performance, customer demographics, mall performance, and payment behavior
- 💼 Present findings in a way that supports real business decision-making

## 🖼️ 3. Dashboard Preview

![Dashboard Preview](assets/dashboard_preview.png)
<p align="center"><em>📌 Replace this with an annotated screenshot of the KPI cards, charts, and slicers in action</em></p>

<details>
<summary>📽️ Click to view a walkthrough GIF (optional)</summary>

![Dashboard Demo](assets/dashboard_demo.gif)

</details>

## 🗂️ 4. Dataset Information

The dataset (`customer_shopping_data.csv`) contains **99,457 rows** and spans **10 shopping malls** in Istanbul over roughly **26 months** of activity.

**Raw Columns**

| Column | Description |
|---|---|
| Invoice | Unique invoice/order number |
| Customer ID | Unique customer identifier |
| Gender | Male / Female |
| Age | Customer age (18–69) |
| Category | Product category purchased (8 categories) |
| Quantity | Number of items purchased in the order |
| Price | Unit price of the item(s) |
| Payment Method | Cash, Credit Card, or Debit Card |
| Invoice Date | Date the transaction occurred |
| Shopping Mall | Mall where the purchase was made (10 malls) |

**Calculated Columns**

| Column | Formula Logic |
|---|---|
| Total Revenue | `Quantity × Price` |
| Month | Extracted from Invoice Date |
| Year | Extracted from Invoice Date |
| Age Group | Bucketed via `IFS()` into Teen, 20–29, 30–39, 40–49, 50–59, 60+ |

## 📊 5. Dashboard KPIs

Six KPI cards sit at the top of the dashboard, each driven by a Pivot Table and updating live with every slicer selection.

| KPI | Description | Value |
|---|---|---|
| 💰 Total Revenue | Sum of revenue across all transactions | **$251,505,794.25** |
| 🧾 Total Orders | Count of unique invoices | **99,457** |
| 👥 Total Customers | Count of unique customer IDs | **99,457** |
| 📦 Average Order Value | Total Revenue ÷ Total Orders | **$2,528.79** |
| 🛍️ Average Items per Order | Total Quantity ÷ Total Orders | **3.00** |
| 🔢 Total Quantity Sold | Sum of all units purchased | **298,712** |

## 📈 6. Dashboard Visualizations

<details>
<summary><strong>1️⃣ Total Sales by Product Category</strong></summary>

A bar chart ranking all 8 categories by revenue. It immediately shows that **Clothing ($113.99M)** dominates, followed by **Shoes ($66.55M)** and **Technology ($57.86M)**, while Cosmetics, Toys, Food & Beverage, Books, and Souvenirs together make up a much smaller share. This chart helps merchandising teams prioritize inventory and marketing spend.
</details>

<details>
<summary><strong>2️⃣ Monthly Sales Trend</strong></summary>

A line chart plotting revenue by calendar month (aggregated across 2021–2023) to reveal seasonality. January ($28.9M) and February ($26.6M) are the strongest months, with a gradual dip through the spring and summer before recovering slightly in Q4 — useful for planning promotions and staffing around demand cycles.
</details>

<details>
<summary><strong>3️⃣ Gender-wise Sales Distribution</strong></summary>

A pie/donut chart splitting revenue between Female (**59.7%, $150.21M**) and Male (**40.3%, $101.30M**) customers, highlighting where the core spending base sits.
</details>

<details>
<summary><strong>4️⃣ Total Spending by Age Group</strong></summary>

A column chart across six age brackets. Revenue is spread remarkably evenly across adult segments — **40–49 ($49.23M), 20–29 ($49.04M), 60+ ($48.29M), 30–39 ($48.29M), and 50–59 ($47.59M)** each contribute roughly 19% of total revenue — while **Teens contribute just 3.6% ($9.05M)**. This tells a clear story: purchasing power here isn't concentrated in one generation, it's broad-based across every adult age group.
</details>

<details>
<summary><strong>5️⃣ Revenue Generated by Shopping Mall</strong></summary>

A horizontal bar chart ranking all 10 malls. **Mall of Istanbul ($50.87M)** and **Kanyon ($50.55M)** lead by a wide margin, followed by **Metrocity ($37.30M)**, while the remaining seven malls each generate between $12M–$25M.
</details>

<details>
<summary><strong>6️⃣ Payment Method Distribution</strong></summary>

A chart comparing Cash, Credit Card, and Debit Card usage by both transaction count and revenue. **Cash leads with 44,447 orders (44.9% of revenue, $112.83M)**, followed by **Credit Card (34,931 orders, $88.08M)** and **Debit Card (20,079 orders, $50.60M)**.
</details>

## 🎚️ 7. Interactive Slicers

The dashboard includes six slicers — **Year, Month, Payment Method, Gender, Age Group,** and **Category** — connected to every Pivot Table and Pivot Chart via shared Pivot Cache connections. Clicking any slicer button instantly filters every visual and KPI card simultaneously, letting a user drill from "all-time revenue" down to, for example, "Female customers aged 20–29 who paid by Credit Card for Clothing in March 2022" in a few clicks — no formulas need to be touched.

## ❓ 8. Business Questions Solved

- 🏆 **Which product category generates the highest revenue?** → Clothing, at $113.99M
- 🏬 **Which shopping mall contributes the most revenue?** → Mall of Istanbul, narrowly ahead of Kanyon
- 📅 **How do monthly sales trends change over time?** → Strongest in Jan–Feb, softer through mid-year
- 💳 **Which payment method is preferred by customers?** → Cash, by both order count and revenue
- 🚻 **Which gender contributes more revenue?** → Female customers, at 59.7% of total revenue
- 🎂 **Which age group spends the most?** → 40–49, though adult groups are nearly tied
- 💵 **What is the average order value?** → $2,528.79
- 🛒 **What is the average number of items purchased per order?** → 3.00
- 📦 **What is the total quantity sold?** → 298,712 units

## 💡 9. Key Business Insights

1. **Clothing is the clear revenue engine**, generating 45% of total revenue — more than Shoes and Technology combined.
2. **Mall of Istanbul and Kanyon are the top two performing locations**, together accounting for over 40% of total mall revenue.
3. **Female shoppers drive the majority of revenue** (59.7% vs. 40.3% for male customers), suggesting marketing and inventory could lean further into categories popular with this segment.
4. **Cash remains the dominant payment method**, both in transaction volume (44,447 orders) and revenue ($112.83M) — notable in an increasingly digital retail landscape.
5. **Adult age groups spend almost identically**, each contributing 18.9%–19.6% of revenue; this is not a business skewed toward one generation.
6. **Teen customers are a minor segment**, contributing only 3.6% of revenue — a potential growth opportunity if targeted correctly.
7. **January and February are peak revenue months**, likely tied to New Year and post-holiday shopping behavior, while mid-year months (Apr–Sep) run comparatively flatter.
8. **The Average Order Value is high, at $2,528.79**, and each order contains an average of exactly 3 items — pointing to a customer base that shops in moderate-to-large basket sizes rather than single-item purchases.
9. **Technology, despite low transaction volume (just 4,996 orders), punches well above its weight in revenue** ($57.86M), reflecting high per-unit prices in that category.
10. **Revenue is heavily concentrated among the top 3 malls** (Mall of Istanbul, Kanyon, Metrocity), which together generate over 55% of total revenue — the remaining 7 malls split the rest fairly evenly.
11. **Debit Card is the least-used payment method**, suggesting customers strongly prefer either the immediacy of cash or the flexibility/rewards of credit.
12. **With 99,457 unique customers behind 99,457 orders**, the dataset reflects largely first-time or single-visit purchases in this window — a strong signal for retention and loyalty-focused strategy.

## 🚀 10. Business Recommendations

- **Double down on Clothing and Shoes** with expanded assortments, cross-category bundling, and targeted promotions, since these two categories alone drive over 71% of revenue.
- **Invest further in Mall of Istanbul and Kanyon** locations — flagship stores, premium placements, or exclusive launches — while testing growth tactics in mid-tier malls like Metropol AVM and Istinye Park.
- **Design campaigns around female shoppers' preferences**, given they generate the majority of revenue, without alienating the substantial male customer base.
- **Introduce loyalty or cashback incentives for card payments** to gradually shift transaction mix away from cash, improving traceability and enabling richer customer analytics.
- **Launch a Teen-focused marketing initiative** (student discounts, social-media-driven campaigns) to grow this currently under-indexed segment.
- **Plan inventory and staffing around the January–February peak**, and design mid-year promotions to smooth out the seasonal dip.
- **Build a repeat-customer loyalty program**, since the current data shows almost entirely single-visit customers — retention represents significant untapped revenue.
- **Protect and grow the Technology category's margins**, since its high average order value makes it disproportionately valuable despite lower order volume.

## 🛠️ 11. Excel Skills Demonstrated

| Skill | Application in this Project |
|---|---|
| **Pivot Tables** | Core engine behind every KPI and summary table |
| **Pivot Charts** | Built directly from Pivot Tables for all 6 visualizations |
| **Slicers** | Six shared slicers driving cross-filtering across the dashboard |
| **Power Query** | Cleaned, typed, and shaped the raw CSV before loading to the data model |
| **Excel Tables** | Structured source data for dynamic ranges and formula stability |
| **IFS()** | Bucketed ages into Age Group categories |
| **SUMIFS()** | Conditional revenue aggregation across category/mall/date combinations |
| **COUNTIFS()** | Conditional counts for order and customer metrics |
| **UNIQUE()** | Extracted distinct malls, categories, and payment methods for validation |
| **COUNTA()** | Row and record counting for data QA |
| **Custom Number Formatting** | Currency, thousands separators, and percentage displays on KPI cards |
| **Data Cleaning** | Removed duplicates, fixed data types, standardized text fields |
| **Dashboard Design** | Layout, color theory, alignment, and visual hierarchy |
| **KPI Development** | Translated raw metrics into recruiter/stakeholder-ready cards |

## 🔄 12. Dashboard Workflow

```
Raw Data → Cleaning → Power Query → Calculated Columns → Pivot Tables → Pivot Charts → KPI Cards → Dashboard → Insights
```

1. **Raw Data** — Imported the 99,457-row `customer_shopping_data.csv`
2. **Cleaning** — Checked for duplicates, blanks, and inconsistent formatting
3. **Power Query** — Set correct data types, standardized date formats, and shaped the table for loading
4. **Calculated Columns** — Added Total Revenue, Month, Year, and Age Group using formulas
5. **Pivot Tables** — Built summary tables by Category, Mall, Gender, Age Group, Payment Method, and Month
6. **Pivot Charts** — Converted each Pivot Table into a corresponding visual
7. **KPI Cards** — Linked six headline metrics to Pivot Table outputs with custom formatting
8. **Dashboard** — Assembled charts, KPI cards, and slicers into a single, cohesive sheet
9. **Insights** — Interpreted the visuals into the business insights and recommendations above

## 📁 13. Folder Structure

```
├── Dataset/
│   └── customer_shopping_data.csv
├── Dashboard.xlsx
├── Dashboard Screenshot.png
└── README.md
```

## 🔮 14. Future Improvements

- 🔁 Recreate the dashboard in **Power BI** for cloud sharing and richer DAX-based analysis
- 📉 Add **year-over-year and month-over-month growth** calculations
- 🌍 Layer in **geographic mapping** if mall-level location data is expanded
- 🧠 Apply **RFM (Recency, Frequency, Monetary) segmentation** to better understand repeat-purchase potential
- 🔔 Add **conditional-formatting-based alerts** for underperforming categories or malls
- 📱 Explore a **mobile-friendly** version of the dashboard layout

## 📚 15. Learning Outcomes

Building this project reinforced how far native Excel tools can go in delivering a genuinely interactive BI product — not just static charts. Key takeaways included structuring a clean Power Query pipeline before any formula work, designing calculated columns that make downstream Pivot Tables far simpler, and building a slicer architecture that keeps six different visuals perfectly in sync. It also sharpened the skill of translating raw numbers into narrative — moving from "what does the data say" to "what should the business do about it."

## ✅ 16. Conclusion

This E-Commerce Sales Performance Dashboard turns nearly 100,000 raw transaction records into a clear, interactive story about where revenue comes from, who is driving it, and how the business can grow further. It's built entirely with core Excel tools — Power Query, Pivot Tables, Pivot Charts, and Slicers — proving that with the right structure and design discipline, spreadsheets can deliver dashboard experiences on par with dedicated BI platforms. This project reflects both technical Excel proficiency and the ability to think like a business analyst: asking the right questions, finding the answers in the data, and communicating them clearly.

---

<div align="center">

⭐ If you found this project useful or interesting, consider giving it a star!

</div>
