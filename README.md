# Financial Intelligence Suite: Dynamic P&L, Balance Sheet, & Cash Flow

## 📌 Project Overview
This project is a comprehensive Power BI solution designed to transform raw ledger data and periodic snapshots into automated, interactive financial statements. Unlike standard reports, this suite uses a **layout-driven DAX architecture**, allowing for highly customizable financial reporting (P&L, Balance Sheet, and Cash Flow) that mirrors professional accounting standards.

## 📊 Key Features
* **Dynamic Financial Statements:** Fully automated Income Statement, Balance Sheet, and Cash Flow Statement using custom layout mapping.
* **Budget vs. Actuals (BVA):** Real-time variance analysis comparing actual performance against budget and forecast versions.
* **Multi-Geography Consolidation:** Ability to filter and consolidate financial data across various regions (UK, France, Germany, etc.).
* **Snapshot Logic:** Implements periodic snapshot processing to handle Balance Sheet accounts (Assets/Liabilities) alongside transactional data (Revenue/Expenses).
* **Forecasting:** Integrated forecast data to visualize future financial health and runway.

## 📁 Repository Structure
* **`/PowerBI_Files`**: Contains `.pbix` files for the core reports:
    * `Income Statement.pbix`: Detailed P&L with hierarchical drill-downs.
    * `Balance Sheet.pbix`: Asset, Liability, and Equity tracking.
    * `Cash Flows Complete.pbix`: Operating, Investing, and Financing activities.
* **`/Data_Inputs`**: The underlying structure (represented here by CSV/Excel logic):
    * `_Ledger Mapping`: Connects Sub-Ledger codes to financial statement lines.
    * `_Layouts`: Defines the specific order and calculation logic for report rows.
    * `_Transactions`: The raw actuals data.

## 🛠️ Technical Stack
* **Tool:** Power BI Desktop
* **Language:** DAX (Data Analysis Expressions) for complex financial calculations (YoY, Running Totals, Variances).
* **Data Modeling:** Star Schema involving Fact tables (Actuals, Budget, Snapshots) and Dimensions (Date, Organization, Ledger).
* **Data Prep:** Power Query (M) for cleaning and reshaping ledger exports.

## 🚀 How to Use
1.  **Clone the repo:** `git clone https://github.com/your-username/financial-analytics-suite.git`
2.  **Open .pbix files:** Use Power BI Desktop to open any of the statement files.
3.  **Data Source Update:** If using your own data, update the file paths in Power Query to point to your local versions of the `Data Inputs.xlsx`.
4.  **Explore:** Use the slicers to toggle between different Geographies, Years, or Statement Levels.
