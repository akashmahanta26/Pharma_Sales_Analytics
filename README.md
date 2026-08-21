# 📊 Pharma Sales Analytics 

An interactive **Power BI Sales & Market Analytics Dashboard** designed to provide a comprehensive view of sales performance, market share, market growth, regional performance, brand performance, and competitive positioning for a global healthcare brand.

The dashboard transforms raw pharmaceutical sales data into actionable business insights through interactive visualizations, dynamic KPIs, DAX measures, and a structured data model.

<img width="1335" height="741" alt="image" src="https://github.com/user-attachments/assets/6f2e8768-5ac5-4209-a80c-0efca9224dcd" />


---

## 🚀 Project Overview

This project demonstrates how Power BI can be used to analyze pharmaceutical sales and market data across:

* Therapy Areas
* Regions and Countries
* Brands and Products
* Competitors
* Sales Value and Volume
* Market Share
* Market Growth
* Month-over-Month Performance
* Period-over-Period Incremental Sales

The dashboard is designed to support commercial and business teams in understanding **where sales are coming from, how brands are performing, how market position is changing, and where growth opportunities exist**.

---

## 🎯 Business Objectives

The dashboard addresses key commercial analytics questions:

* What is the total sales value across different therapy areas?
* Which brands are the strongest and weakest performers?
* Which regions contribute the most to overall sales?
* How does the brand compare with competitors?
* What is the market share across regions, countries, and therapy areas?
* How is market growth changing over time?
* Which brands are experiencing above- or below-average Month-over-Month growth?
* What are the incremental sales changes between selected periods?
* Which products rank highest based on the selected Top-N criteria?

---

## 📌 Key Dashboard Features

### 1. Sales Performance

Provides an overview of overall sales performance across therapy areas and regions.

**Key metrics include:**

* Total Sales
* Sales Volume
* Sales by Therapy Area
* Sales by Region
* Sales by Brand
* Top 10 Brands
* Bottom 10 Brands

---

### 2. Market Share Analysis

Market share is calculated as:

```text
Market Share % =
Brand Sales / Total Market Sales × 100
```

The dashboard enables users to analyze:

* Overall market share
* Market share by therapy area
* Market share by region
* Market share by country
* Competitor market share
* Leading competitors by market

---

### 3. Market Growth Analysis

Market growth is calculated using:

```text
Market Growth % =
(Current Year Market Size - Previous Year Market Size)
/
Previous Year Market Size × 100
```

This allows users to identify:

* High-growth regions
* Low-growth regions
* Growth trends over time
* Brand growth versus competitors
* Markets with significant performance changes

---

### 4. Month-over-Month Growth

The dashboard calculates Month-over-Month (MoM) sales growth:

```text
MoM Growth % =
(Current Month Sales - Previous Month Sales)
/
Previous Month Sales × 100
```

Users can analyze:

* Average MoM growth by therapy area
* Regional MoM performance
* Brands performing below the average growth rate
* Monthly sales trends

---

### 5. Incremental Sales Analysis

Incremental sales are calculated between a user-selected start and end period:

```text
Incremental Sales % =
(End Period Sales - Start Period Sales)
/
Start Period Sales × 100
```

The dashboard supports analysis of incremental performance for:

* Sales Value
* Sales Volume
* Therapy Areas
* Selected time periods

Users can dynamically select the analysis period and evaluate how sales have changed.

---

### 6. Dynamic Top-N Analysis

A dynamic Top-N selector allows users to choose the number of products they want to analyze.

For example:

```text
Top 5
Top 10
Top 15
Top 20
...
```

The corresponding visual dynamically updates based on the user's selection.

This functionality is implemented using **DAX measures and ranking logic**.

---

### 7. Competitive Analysis

The dashboard compares the focal brand against competing pharmaceutical brands.

Analysis includes:

* Competitor sales
* Competitor market share
* Brand-level comparison
* Therapy-area comparison
* Regional competitive performance

This helps identify the brand's competitive position across different markets.

---

### 8. Dynamic Brand Color Coding

Brand-level conditional formatting is implemented using DAX to dynamically assign colors to products.

This enables consistent visual identification of brands across tables and matrix visuals.

Example:

```text
Brand A → Custom Brand Color
Brand B → Custom Brand Color
Brand C → Custom Brand Color
```

The approach can be extended to accommodate additional brands without redesigning individual visuals.

---

## 📊 Dashboard Visualizations

The dashboard incorporates multiple interactive visualizations, including:

* KPI Cards
* Bar Charts
* Donut Charts
* Treemaps
* Matrix / Table Views
* Trend Analysis
* Regional Analysis
* Competitive Comparison
* Dynamic Top-N Charts

Interactive filters allow users to drill into the analysis by dimensions such as:

* Therapy Area
* Month / Year
* Region
* Country
* Brand
* Selected Period

---

## 🧮 Data Model

The project follows a **star-schema data modeling approach**, with fact and dimension tables structured to support efficient analytical queries and flexible reporting.

### Conceptual Model

<img width="1016" height="410" alt="image" src="https://github.com/user-attachments/assets/dd3538e7-99fa-4bca-88e4-feb1fee5d1a1" />

```

The model separates transactional sales data from descriptive dimensions, enabling reusable DAX measures and interactive filtering.

---

## 🛠️ Tools & Technologies

| Technology                          | Purpose                                  |
| ----------------------------------- | ---------------------------------------- |
| **Power BI**                        | Dashboard development and visualization  |
| **Power Query**                     | Data cleaning and transformation         |
| **DAX**                             | KPI calculations and analytical measures |
| **Star Schema**                     | Data modeling                            |
| **Excel / Tabular Data**            | Source data                              |
| **Power BI Bookmarks & Navigation** | Interactive user experience              |

---

## 🔄 Data Preparation

The data preparation workflow includes:

1. Importing source datasets into Power BI
2. Cleaning and standardizing fields
3. Transforming data using Power Query
4. Creating dimension tables
5. Establishing relationships between tables
6. Building a star-schema data model
7. Creating calculated measures using DAX
8. Validating KPI calculations
9. Designing interactive visualizations
10. Applying dynamic formatting and navigation

---

## 📐 Key DAX Concepts

The project demonstrates several Power BI/DAX techniques, including:

* `CALCULATE()`
* `SUM()`
* `DIVIDE()`
* `FILTER()`
* `RANKX()`
* `ALL()`
* `ALLSELECTED()`
* Time-intelligence calculations
* Dynamic Top-N filtering
* Conditional formatting measures
* Month-over-Month calculations
* Period-over-period comparisons

---

## 📈 Analytical Insights

The dashboard is designed to help commercial teams identify:

### Sales Opportunities

Identify high-performing brands, therapy areas, and regions contributing disproportionately to sales.

### Growth Opportunities

Highlight markets and brands with stronger growth trajectories.

### Underperforming Areas

Identify brands or regions with declining or below-average growth.

### Competitive Positioning

Compare sales and market share against competing products.

### Portfolio Performance

Understand the contribution of individual brands to overall business performance.

### Regional Trends

Evaluate differences in performance across countries and geographic regions.

---

## 🎨 Dashboard Design

The dashboard follows a business-oriented design philosophy focused on:

* Clear KPI hierarchy
* Minimal visual clutter
* Consistent branding
* Interactive filtering
* Intuitive navigation
* Easy comparison between categories
* Executive-friendly visualizations

The goal is to allow users to move from **high-level performance → regional performance → brand performance → competitive analysis** with minimal interaction.

---

## 📁 Project Structure

```text
PowerBI-Sales-Market-Analytics/
│
├── README.md
│
├── PowerBI/
│   └── Pharma_Sales_Analysis_AM.pbix
│
├── Data/
│   └── Diabetes_Dataset.xlsx
    |___Obesity_Dataset.xlsx
|   |___ Region_Dataset.xlsx 
│

```

> **Note:** Source datasets may not be included in this repository if they contain confidential or restricted information.

---

## 🖥️ Dashboard Preview

### Sales Performance

![Sales Performance Dashboard](Screenshots/sales-performance.png)

### Market & Competitive Analysis

![Market Analysis Dashboard](Screenshots/market-analysis.png)

> Replace the image paths above with the actual screenshots included in the repository.

---

## 🔍 Example User Journey

A typical user can:

```text
Select Therapy Area
        ↓
Select Month / Year
        ↓
Review Overall Sales
        ↓
Analyze Regional Contribution
        ↓
Identify Top / Bottom Brands
        ↓
Compare Competitors
        ↓
Analyze Market Share
        ↓
Review Growth & MoM Trends
        ↓
Identify Business Opportunities
```

---

## 💡 Key Takeaways

This project demonstrates the application of Power BI for **end-to-end commercial analytics**, covering:

* Data transformation
* Data modeling
* DAX development
* KPI design
* Market analytics
* Competitive analysis
* Dynamic ranking
* Interactive reporting
* Business storytelling

The dashboard converts complex sales and market datasets into an interactive analytical tool that can support **data-driven commercial decision-making**.

---

## ⚠️ Disclaimer

This repository is intended for **portfolio and educational purposes**.

Any company names, logos, product names, customer information, or confidential business data have been removed or generalized. The dashboard structure and analytical approach are presented as a generic example of a commercial sales and market analytics solution.

---

## 👤 Author

**Akash Mahanta**

Master of Science in Business Analytics
National University of Singapore

### Skills Demonstrated

`Power BI` · `DAX` · `Power Query` · `Data Modeling` · `SQL` · `Data Analytics` · `Business Intelligence` · `Data Visualization`
