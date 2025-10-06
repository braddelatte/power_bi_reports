Excellent — here’s your **updated README**, now incorporating the actual tab (sheet) names and column context from your Excel file.
I’ve restructured the **Data Sources** and **Sample Data Replacement** sections to directly reflect your workbook contents.

---

# Power BI Example Report

![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Modeling%20%26%20Visualization-yellow?logo=powerbi)
![SQL](https://img.shields.io/badge/SQL-Data%20Transformation-blue?logo=databricks)
![Power Query](https://img.shields.io/badge/Power%20Query-ETL-green?logo=microsoft)
![License](https://img.shields.io/badge/Data-Anonymized-orange)

---

## 📘 Table of Contents

* [Overview](#-overview)
* [Data Sources](#-data-sources)
* [Sample Data Replacement](#-sample-data-replacement)
* [How It Works](#-how-it-works)
* [Data Disclaimer](#-data-disclaimer)
* [Skills Demonstrated](#-skills-demonstrated)
* [Getting Started](#-getting-started)
* [Dashboard Assets](#-dashboard-assets)
* [Repository Contents](#-repository-contents)
* [About](#-about)

---

## 📊 Overview

This repository contains **`example_stats_report.pbix`**, a **Power BI example report** that demonstrates how SQL-based datasets can be integrated, transformed, and visualized.

The project models a **real-world analytics workflow**, where all data originated from a SQL database before being exported to Excel for demonstration purposes.
It highlights expertise in **SQL transformations**, **Power Query ETL**, and **Power BI data modeling and visualization**.

---

## 🗂️ Data Sources

All data in this report originates from a **SQL Server database** and has been consolidated into a single Excel workbook:

> **`sample_data.xlsx`**

This workbook contains the following tabs (each corresponding to a dataset in the original SQL environment):

### **1. Sales**

Contains information on item-level sales transactions.
**Columns include:**
`SaleDate`, `SaleItemId`, `SaleNum`, `SaleItem`, `ProjectNum`, `ExtSalePrice`, `FSC`, `ReqItemId`, `PartId`, `ExtCost`, `Vendor`.

### **2. Req**

Captures requisition and quote-level data used for cost and pricing analysis.
**Columns include:**
`ReqDate`, `SbmtdQteDate`, `ReqItemId`, `ReqNum`, `ReqItem`, `ProjectNum`, `QuotePrice`, `ExtQuotePrice`, `FSC`, `PartId`, `ReqQty`, `SaleQnty`, `DaysToQuote`, `SOLD`, `Cost`, `ExtCost`.

### **3. Prog_Desc**

Provides program-level metadata and project descriptions.
**Columns include:**
`ProjectNum`, `Prog_Desc`, `ProjectDesc`.

### **4. Receivable**

Contains accounts receivable and invoice summary data.
**Columns include:**
`InvNum`, `ProjectNum`, `InvDate`, `ARAmt`, `Misc`, `Freight`, `depAmnt`.

---

## 💾 Sample Data Replacement

To make this example report **portable and shareable**, all SQL-derived datasets were exported into:

> **`sample_data.xlsx`**

The workbook consolidates final tables representing cleaned and modeled outputs from SQL and Power Query transformations.
All **dollar-related fields** (e.g., `Cost`, `QuotePrice`, `ExtCost`, `ExtSalePrice`, etc.) have been **anonymized** while preserving realistic data structure and proportional relationships.

---

## ⚙️ How It Works

1. Power BI imports all datasets from `sample_data.xlsx`.
2. Relationships between tables (e.g., by `ProjectNum`, `ReqItemId`, `PartId`) mirror production SQL relationships.
3. Power Query applies transformations identical to those used in the live SQL database.
4. DAX measures and visuals replicate the production logic for comparison and demonstration.

> 💡 **Tip:** In **Power BI Desktop**, hold **CTRL** while clicking navigation buttons to move between report pages.

---

## 🔐 Data Disclaimer

This report’s design and logic reflect a production-grade system, but **all numeric and monetary values have been anonymized**.
No proprietary or sensitive data is present.
The dataset structure, naming, and relationships are retained to illustrate realistic modeling and visualization scenarios.

---

## 🚀 Skills Demonstrated

* SQL scripting and relational modeling
* Power Query (M) for ETL and data shaping
* Power BI data modeling and relationship management
* DAX measures and calculations
* Report design, navigation, and visualization best practices
* Integration of multiple data sources into a unified model

---

## 🧭 Getting Started

1. Clone or download this repository.
2. Open **`example_stats_report.pbix`** in **Power BI Desktop**.
3. Ensure **`sample_data.xlsx`** is in the same folder (or update the Power Query path).
4. Refresh the data model.
5. Hold **CTRL + Click** on report icons to navigate between pages.

---

## 🖼️ Dashboard Assets

The **`images/`** folder includes:

* PowerPoint layouts used to design dashboard backgrounds
* Visual and theme design notes for Power BI

These assets demonstrate the planning and consistency behind the dashboard layouts, color usage, and spacing.

---

## 📁 Repository Contents

| File                        | Description                                            |
| --------------------------- | ------------------------------------------------------ |
| `example_stats_report.pbix` | The Power BI report                                    |
| `sample_data.xlsx`          | Anonymized, SQL-derived dataset                        |
| `images/`                   | PowerPoint design files and dashboard layout resources |
| `README.md`                 | Project documentation                                  |

---

## 📬 About

**Created by:** Brad Delatte
*Systems Coordinator & Business Data Analyst*

Demonstrating end-to-end analytics workflows using **SQL**, **Power Query**, and **Power BI**.

🔗 [LinkedIn Profile](https://www.linkedin.com/in/brad-delatte-790975149/)

---

Would you like me to add a short **“Data Model Overview”** section (showing how the four tables relate — e.g., `Req` links to `Sales` and `Receivable` via `ProjectNum`)? That’s often a great touch for documentation or portfolio readers.
