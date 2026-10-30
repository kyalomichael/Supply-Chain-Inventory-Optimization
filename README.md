# Supply Chain & Inventory Optimization Dashboard

An end-to-end data analytics and Power BI reporting solution designed to evaluate supply chain efficiency, identify fulfillment bottlenecks, monitor regional risk, and optimize product sales velocity across 180,519 order records.

---

## 📌 Project Overview

This project provides operational visibility into logistics performance, inventory stock status, and revenue exposure due to late shipping delays. Using a structured Python data cleaning pipeline, SQLite database staging, and dynamic DAX modeling in Power BI, the interactive 3-page report helps logistics managers pinpoint late delivery root causes and streamline fulfillment.

---

## 🎨 Design & Palette Standard

Built following the **Modern Mokkup UI Framework**:
* **Theme Accent:** Lime Green (`#84CC16`)
* **Supporting Palette:** Monochromatic Greens (`#65A30D`, `#4D7C0F`, `#A3E635`, `#365314`)
* **Background:** Light Slate (`#F8FAFC`) with clean white card containers (`#FFFFFF`)

---

## 📊 Dashboard Architecture & Page Highlights

### Page 1: Executive Overview
* **KPI Metrics:** Total Orders (180,519), Total Shipped Orders, Revenue at Risk, and Global Late Delivery Rate.
* **Order Fulfillment Trends:** Monthly tracking of total orders alongside late delivery rate percentages.
* **Global Filters:** Top header control hub with synchronized slicers (`Market`, `Shipping Mode`, `Date Range`).

### Page 2: Regional Risk
* **Bottleneck Analysis:** Ranks top bottleneck regions by average shipping latency (days).
* **Matrix Control Table:** Breakdowns by `market` and `order_region` for targeted supply chain interventions.
* **Scatter Plot:** Visualizes sales velocity against late delivery risk percentages across product categories.

### Page 3: SKU Inventory Velocity
* **SKU Health KPIs:** Total SKUs (118), Top Velocity SKU, Average Daily Velocity, and Critical Stock Alerts.
* **Top 10 Ranked SKUs:** Clean horizontal bar chart showcasing top-performing SKUs by monthly velocity.
* **Action Matrix:** Granular SKU inventory table highlighting specific operational recommendations (e.g., *Monitor Transit Delays*).

---

## 🛠️ Data Pipeline & Tech Stack

* **Data Cleaning & Analysis:** Python (`pandas`, `numpy`), Jupyter Notebooks (`notebooks/`)
* **Database & Staging:** SQLite (`database/`)
* **Business Intelligence & Visualization:** Power BI Desktop (`pbix/`, `dashboards/`)
* **DAX Measures:** Calculated measures for Sales Velocity, Critical Stock Alerts, Late Delivery Rate %, and Revenue at Risk.

---

## 📂 Repository Structure

```text
Supply-Chain-Inventory-Optimization/
├── dashboards/      # Dashboard screenshot exports & visual assets
├── data/            # Cleaned supply chain CSV dataset (180,519 rows)
├── database/        # SQLite staging database files
├── notebooks/       # Jupyter notebooks for EDA and data cleaning
├── pbix/            # Power BI project template & .pbix files
├── power_bi/        # Supporting Power BI theme JSON & assets
├── .gitignore       # Git ignore settings
└── README.md        # Project documentation