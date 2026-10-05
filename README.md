# 🚢 Toronto Island Ferry Analytics – Power BI Dashboard

## 📊 Project Overview

The **Toronto Island Ferry Analytics Dashboard** is an interactive Business Intelligence project developed using **Microsoft Power BI**.

The dashboard analyzes ferry ticket transaction data to understand **sales, redemptions, transaction activity, demand trends, and redemption performance**. It provides interactive visualizations and KPIs to support data-driven operational analysis.

---

## 🎯 Project Objectives

* Analyze total ferry ticket sales and redemptions.
* Monitor overall transaction activity.
* Identify monthly sales and redemption trends.
* Analyze the relationship between sales and redemptions.
* Calculate redemption performance using DAX.
* Identify sales–redemption gaps.
* Provide interactive filtering and navigation.
* Provide a **Reset Filters button** to quickly restore the default slicer state.
* Present business insights through an easy-to-use Power BI dashboard.

---

## 📁 Dataset

The dataset contains ferry ticket transaction records with the following fields:

* `_id` – Unique transaction identifier
* `Timestamp` – Date and time of the transaction
* `Sales Count` – Number of tickets sold
* `Redemption Count` – Number of tickets redeemed

The dataset is used to analyze passenger demand patterns, transaction activity, sales performance, and redemption behavior.

---

## 🛠️ Technologies Used

### 🔹 Business Intelligence & Visualization

* **Microsoft Power BI Desktop**
* Power BI Visualizations
* Power BI Data Modeling

### 🔹 Data Preparation

* **Power Query**
* Data Cleaning
* Data Transformation
* Data Type Management

### 🔹 Data Analysis

* **DAX (Data Analysis Expressions)**
* DAX Measures
* KPI Calculations
* Aggregations
* Time-Series Analysis

### 🔹 Power BI Interactive Features

* Slicers
* Interactive Filters
* **Reset Filters / Reset Slicers Button**
* Bookmarks
* Page Navigation Buttons
* Report Page Tooltips
* Cross-Filtering
* Interactive Dashboard Navigation

### 🔹 Visualization Techniques

* KPI Cards
* Line Charts
* Clustered Column Charts
* Line & Clustered Column Charts
* Monthly Trend Analysis
* Comparative Analysis
* Time-Series Analysis
* Performance Analysis

### 🔹 Reporting

* Power BI PDF Export
* Dashboard Screenshots
* Interactive Power BI Report

---

## 📌 Dashboard Structure

The Power BI report contains **two main dashboard pages**:

### 1️⃣ Ferry Overview

The overview page provides a high-level summary of ferry ticket activity.

**Key Components:**

* Total Sales
* Total Redemptions
* Total Transactions
* Average Sales
* Redemption Rate
* Sales & Redemption Performance
* Transaction Activity
* Monthly Sales Trend
* Monthly Redemption Trend
* Year Filter
* Month Filter
* Date Range Filter
* **Reset Filters button**
* Interactive navigation to the Performance page
* Custom report-page tooltip

The **Reset Filters button** allows users to quickly clear the selected Year, Month, and Date Range slicer selections and return the dashboard to its default filter state.

---

### 2️⃣ Ferry Performance & Demand Analysis

The performance page provides deeper analysis of transaction and demand behavior.

**Key Components:**

* Total Sales
* Total Redemptions
* Total Transactions
* Average Sales
* Redemption Rate
* Sales & Redemption Performance
* Monthly Sales Trend
* Monthly Redemption Trend
* Redemption-to-Sales Ratio
* Sales–Redemption Gap
* Interactive navigation back to the Overview page

---

## 📈 Key Dashboard Metrics

### Total Sales

Total number of tickets recorded as sold.

### Total Redemptions

Total number of tickets recorded as redeemed.

### Total Transactions

```DAX
Total Transactions =
COUNT('Toronto Island Ferry Tickets'[_id])
````

### Redemption Rate

```DAX
Redemption Rate =
DIVIDE(
    SUM('Toronto Island Ferry Tickets'[Redemption Count]),
    SUM('Toronto Island Ferry Tickets'[Sales Count]),
    0
)
```

### Sales–Redemption Gap

```DAX
Sales Redemption Gap =
SUM('Toronto Island Ferry Tickets'[Sales Count])
-
SUM('Toronto Island Ferry Tickets'[Redemption Count])
```

---

## 🎛️ Interactive Features

The dashboard includes several interactive Power BI features:

* 🔽 Year slicer
* 🔽 Month slicer
* 📅 Date range slicer
* 🔄 Cross-filtering between visuals
* 🔘 Page navigation buttons
* 🔖 Bookmarks
* 🔄 **Reset Filters / Reset Slicers button**
* 💬 Custom report-page tooltip
* 📊 Interactive KPI cards
* 📈 Dynamic charts
* 🧭 Dashboard navigation

### 🔄 Reset Filters Button

The **Reset Filters** button provides a convenient way to restore the dashboard to its default slicer state.

It resets the selections applied through:

* Year slicer
* Month slicer
* Date Range slicer

The button is implemented using a **Power BI Bookmark**, which stores the default filter state and restores it when the user clicks the button.

This improves dashboard usability by allowing users to quickly return to the original overview without manually clearing each slicer.

---

## 💡 Dashboard Insights

The dashboard enables analysis of:

* Overall ticket sales performance
* Overall ticket redemption performance
* Monthly demand patterns
* Changes in sales volume over time
* Changes in redemption volume over time
* Transaction activity
* Sales versus redemption performance
* Difference between tickets sold and redeemed
* Redemption-to-sales relationship

---

## 🎯 Key Outcomes

* Developed an interactive **Power BI Business Intelligence dashboard**.
* Created KPI-based performance monitoring.
* Implemented DAX measures for analytical calculations.
* Built monthly sales and redemption trend analysis.
* Added interactive slicers and filters.
* Added a **Reset Filters button using Power BI Bookmarks**.
* Implemented bookmark-based dashboard navigation.
* Added custom report-page tooltips.
* Created comparative sales and redemption visualizations.
* Designed a professional dark-themed dashboard interface.
* Exported the completed Power BI report as PDF for reporting and presentation.

---

## 🎨 Dashboard Design

The dashboard uses a professional **dark navy Business Intelligence theme**.

### Color Palette

* **Primary Background:** `#071A2B`
* **Panel/Card Background:** `#102A43`
* **Secondary Panel:** `#0D2235`
* **Primary Accent:** `#2196F3`
* **Secondary Accent:** `#26C6A6`
* **Highlight:** `#FFC857`
* **Primary Text:** `#FFFFFF`
* **Secondary Text:** `#B8C7D9`

The design focuses on readability, clear KPI presentation, interactive navigation, and visual consistency.

---

## 📂 Repository Structure

```text
Toronto-Island-Ferry-Analytics-PowerBI/
│
├── README.md
│
├── PowerBI/
│   └── Toronto_Island_Ferry_Analytics.pbix
│
├── Reports/
│   └── Toronto_Island_Ferry_Analytics.pdf
│
├── Dataset/
│   └── Toronto_Island_Ferry_Tickets.csv
│
└── Screenshots/
    ├── Ferry_Overview.png
    └── Ferry_Performance.png
```

---

## 🖼️ Dashboard Preview

### Ferry Overview

<img width="1227" height="692" alt="image" src="https://github.com/user-attachments/assets/20015ad4-6555-4114-bbf9-b88517865c32" />

### Ferry Performance & Demand Analysis

<img width="1006" height="557" alt="image" src="https://github.com/user-attachments/assets/57229606-ec52-4518-855e-47c12d8da884" />

---

## 📦 Project Deliverables

* 📊 Power BI Dashboard (`.pbix`)
* 📄 Dashboard PDF Report (`.pdf`)
* 📁 Dataset (`.csv`)
* 🖼️ Dashboard Screenshots (`.png`)
* 📖 Project Documentation (`README.md`)

---

## 💼 Business Value

The dashboard provides a centralized view of ferry ticket transaction performance and helps users:

* Monitor sales performance.
* Monitor redemption activity.
* Understand demand trends.
* Compare sales and redemptions.
* Identify transaction patterns.
* Analyze performance over time.
* Quickly reset applied filters for easier dashboard exploration.
* Support data-driven operational decisions.

---

## 🚀 Project Highlights

* ⭐ Interactive Power BI Dashboard
* ⭐ Professional dark-themed UI
* ⭐ 2 analytical dashboard pages
* ⭐ 5 KPI metrics
* ⭐ DAX-based calculations
* ⭐ Interactive slicers and filters
* ⭐ **Reset Filters button**
* ⭐ Bookmark navigation
* ⭐ Custom report-page tooltip
* ⭐ Time-series analysis
* ⭐ Sales vs. redemption comparison
* ⭐ Business-focused data visualization

---

## 👨‍💻 Author

### Satwik Srivastava

**BCA – Data Science & AI**
**BCA DS - 26**
**05 / 1250258395**

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.

**Built with Microsoft Power BI for interactive data-driven analysis.**
