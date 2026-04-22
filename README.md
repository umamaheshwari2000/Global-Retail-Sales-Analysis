# 🌐 Global Superstore Sales Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-0078D4?style=for-the-badge&logo=databricks&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

> **An end-to-end interactive business intelligence dashboard built on the Global Superstore dataset — transforming 51,000+ raw transactional records into executive-level insights across 7 global regions, 3 product categories, and 4 years of business history.**

## 📸 Dashboard Preview

![Global Superstore Sales Dashboard](./dashboard_preview.png)

## 📊 Key Metrics at a Glance

| Metric | Value |
|---|---|
| 💰 Total Sales | $12.64M |
| 📈 Total Profit | $1.47M |
| 📉 Profit Margin | 4.74% |
| 🔁 Return Rate | 4.68% |
| 🌍 Regions Covered | 7 Global Regions |
| 🗂️ Years Covered | 2011 – 2014 |

## 🧠 Project Overview

This project delivers a fully interactive Power BI dashboard designed to help business stakeholders monitor global sales performance, identify profitability leaks, and evaluate shipping efficiency. The dashboard integrates order data, return records, and regional segments to surface insights that drive real strategic decisions — not just pretty charts.

## 📁 Dataset Details

The raw dataset `GlobalSuperstore_Data.xlsx` contains **51,000+ order records** across the following fields:

| Column | Description |
|---|---|
| `Order ID / Date` | Unique transaction identifier and timestamp |
| `Customer Name / Segment` | Consumer, Corporate, Home Office |
| `Region / Market` | 7 regions — APAC, EU, EMEA, LATAM, US |
| `Category / Sub-Category` | Technology, Furniture, Office Supplies |
| `Sales / Profit / Discount` | Core financial performance metrics |
| `Ship Mode` | Standard Class, Second Class, First Class, Same Day |
| `Order Priority` | Critical, High, Medium, Low |
| `Shipping Cost` | Logistics cost per transaction |

## 🔬 Visual-by-Visual Insights

### 🃏 1. KPI Cards — Total Sales · Total Profit · Profit Margin · Return Rate

**📌 What it shows:** Four headline metrics that give an instant health check of the entire business in one glance.

**💡 Insight:** Sales stand strong at $12.64M but the profit margin is a concerning 4.74% — meaning for every $100 sold, only $4.74 is actually kept. The return rate of 4.68% compounds this by adding reverse logistics costs on top.

**🔎 Why this is happening:** Aggressive discounting across multiple sub-categories is the primary margin killer. Returns are not being tracked or actioned at a regional level, so losses quietly stack up.

**✅ What to do:** Set a company-wide discount ceiling of 20% enforced through CRM approval workflows. Launch a return root-cause analysis by product and region to stop losses at the source, not after the fact.

### 📊 2. Total Sales and Total Profit by Region — Bar Chart

**📌 What it shows:** A side-by-side comparison of Sales and Profit across all global regions, ranked from highest to lowest revenue.

**💡 Insight:** Central leads all regions with $3.13M in sales — nearly double South ($1.74M). However, regions like Africa and Caribbean generate very low profit despite moderate order volumes, suggesting their cost-to-serve far exceeds what their revenue justifies.

**🔎 Why this is happening:** Central and South benefit from mature customer bases, higher average order values, and efficient delivery infrastructure. Smaller regions like Caribbean suffer from high per-order shipping costs and fragmented, low-volume demand that inflates operational expenses.

**✅ What to do:** Invest aggressively in Central and South — loyalty programs, upselling, and category expansion. For Caribbean and Canada, evaluate whether a regional distribution partner model can reduce fulfilment costs, or consider narrowing the product catalogue to only high-margin SKUs in those markets.

### 📈 3. Total Sales and Profit by Year and Month — Area Chart

**📌 What it shows:** A time-series view of revenue and profit growth from 2011 to 2014, plotted month by month as stacked areas.

**💡 Insight:** Sales grew from $2.26M in 2011 to $4.80M in 2014 — a 91% increase in four years. However, profit growth has not kept pace with sales growth. The business is scaling volume without proportionally scaling earnings, which is a red flag at this stage.

**🔎 Why this is happening:** Discounting was used as the primary engine of growth when entering new markets. More orders came in, but at thinner margins. Operational costs also scaled with volume without matching efficiency improvements in logistics or procurement.

**✅ What to do:** Shift from volume-led growth to value-led growth. Introduce dual KPIs — revenue AND profit — for every region and category owner. Run margin analysis by quarter to catch erosion early. Prioritise high-margin segments like Corporate Technology over low-margin bulk orders.

### 🍩 4. Total Profit by Ship Mode — Donut Chart

**📌 What it shows:** Profit contribution split across the four shipping methods — Standard Class, Second Class, First Class, and Same Day.

**💡 Insight:** Standard Class contributes a dominant 60.69% of total profit ($890.6K). Same Day delivery contributes barely anything despite being the most expensive option. First Class at 14.18% ($208.1K) is underperforming relative to its cost premium.

**🔎 Why this is happening:** Same Day and First Class have high fulfilment costs that eat into per-order margin. Customers are not being charged prices that offset those logistics costs, so premium shipping becomes a profit drain rather than a revenue driver.

**✅ What to do:** Reprice First Class and Same Day shipping to fully reflect the cost premium. Promote Standard Class to customers with flexible timelines using small incentives like loyalty points. Analyse which customer segments choose premium shipping and determine whether their order values actually justify the cost — if not, restrict premium options to orders above a minimum value threshold.

### 📦 5. Total Orders and Returned Orders by Region — Grouped Bar Chart

**📌 What it shows:** A region-level comparison of total orders placed versus the number of those orders that were returned, showing both volume and return burden side by side.

**💡 Insight:** Central leads with 5.2K total orders and South follows at 3.3K. Canada has a disproportionately high return count relative to its actual order volume — a clear signal of a product-market fit or fulfilment quality issue specific to that region.

**🔎 Why this is happening:** High return rates in Canada and Caribbean are often driven by product descriptions not matching customer expectations, shipping damage on long international routes, or a mismatch between the global product catalogue and what local customers actually need.

**✅ What to do:** Conduct a focused root-cause analysis for Canada — categorise every return by product type and return reason code. Improve and localise product descriptions for regional audiences. Introduce a quality checkpoint before dispatching to historically high-return regions. Study what EMEA and South are doing right in fulfilment and replicate it.

### 📉 6. Return Rate % by Region — Bar Chart

**📌 What it shows:** The percentage return rate per region, revealing which markets have the highest proportion of returned orders relative to total orders placed.

**💡 Insight:** Canada dominates return volume with 583 returned orders — more than 4x the next highest region (Caribbean at 137). EMEA and South show the best return efficiency, suggesting strong product-customer alignment and reliable fulfilment in those markets.

**🔎 Why this is happening:** Canada's outlier return rate likely reflects longer delivery windows causing condition issues on arrival, product catalogue mismatches with local preferences, and possibly a more quality-conscious customer base with higher expectations on accuracy and packaging.

**✅ What to do:** Build a Canada-specific returns monitoring report to track which SKUs are being returned most frequently. Introduce pre-shipment quality checks for all Canada-bound orders. Study the EMEA and South fulfilment model — their low return rates are a competitive asset worth understanding deeply and replicating in underperforming regions.

### 🔵 7. Discount vs Profit Margin — Scatter Plot

**📌 What it shows:** Each bubble represents a product sub-category, plotted on average discount (X-axis) against profit margin % (Y-axis), with bubble size indicating order volume.

**💡 Insight:** Every sub-category with average discounts above 0.20 falls into negative or near-zero profit margin territory. Tables and Binders show deeply negative margins at high discount rates. In contrast, Accessories and Copiers maintain positive margins even at moderate discounts — proving that not all sub-categories respond to discounting the same way.

**🔎 Why this is happening:** Discounts are being applied uniformly across all sub-categories with no consideration for individual cost structures. A high-cost item like a Conference Table simply cannot absorb a 25–30% discount and remain profitable. Low-cost accessories have enough margin buffer to handle moderate discounts without collapsing.

**✅ What to do:** Implement category-specific discount caps in the CRM and sales approval system immediately. Tables, Bookcases, and Machines should have a hard cap of 10–15%. Accessories and Copiers can safely allow up to 20%. Run A/B pricing tests to find the optimal discount floor per sub-category that maximises both conversion rate and profit margin simultaneously.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard design, DAX measures, interactive visuals |
| **Microsoft Excel** | Raw data storage and initial exploration |
| **DAX** | Profit Margin %, Return Rate %, YOY Growth calculations |
| **Power Query** | Data cleaning, type formatting, null handling |

## 🚀 How to Run This Project

```bash
# Step 1: Clone the repository
git clone https://github.com/yourusername/global-superstore-dashboard.git

# Step 2: Open the dataset
# Load GlobalSuperstore_Data.xlsx into Power BI via Get Data → Excel

# Step 3: Open the dashboard
# Open GlobalSuperstore_Dashboard.pbix in Power BI Desktop

# Step 4: Refresh data
# Click Home → Refresh to reload all visuals from source
```

## 📂 Project Structure

```
global-superstore-dashboard/
│
├── GlobalSuperstore_Data.xlsx        # Raw dataset (51,000+ records)
├── GlobalSuperstore_Dashboard.pbix   # Power BI dashboard file
├── dashboard_preview.png             # Dashboard screenshot
└── README.md                         # Project documentation
```

## 💡 Skills Demonstrated

`Data Cleaning` `Exploratory Data Analysis` `DAX Calculations` `KPI Design` `Business Intelligence` `Data Storytelling` `Trend Analysis` `Profit Margin Analysis` `Return Rate Analysis` `Executive Reporting` `Discount Optimisation`

## 🤝 Let's Connect

<table>
  <tr>
    <td align="center" width="50%">
      <a href="mailto:umamaheshwaripoloju@gmail.com">
        <img src="https://img.shields.io/badge/📧_Drop_me_a_Mail-FF6B6B?style=for-the-badge" />
        <br><sub><b>umamaheshwaripoloju@gmail.com</b></sub>
      </a>
    </td>
    <td align="center" width="50%">
      <a href="https://www.linkedin.com/in/poloju-uma-maheshwari-114764222/">
        <img src="https://img.shields.io/badge/💼_Connect_on_LinkedIn-0A66C2?style=for-the-badge" />
        <br><sub><b>Poloju Uma Maheshwari</b></sub>
      </a>
    </td>
  </tr>
</table>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&pause=1000&color=00B4D8&center=true&vCenter=true&width=600&lines=Open+to+Data+Analyst+Opportunities+%F0%9F%9A%80;Let%27s+turn+data+into+decisions+together+%F0%9F%93%8A;Always+curious%2C+always+learning+%F0%9F%92%A1" alt="Typing SVG" />
</p>

<p align="center"><i>"Data is not just numbers — it's the story of every decision a business ever made."</i></p>
<p align="center">⭐ If this project added value to you, a star would make my day!</p>
