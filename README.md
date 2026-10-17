# Financial KPI & Monitoring Dashboard 📊📈

Welcome to the **Financial KPI & Monitoring Dashboard** project! This repository contains a fully optimized, end-to-end Business Intelligence solution built using **Power BI Desktop**. The project transforms fragmented financial spreadsheet tracks into an interactive, centralized analytics engine to help stakeholders track operational budgets, actual expenses, and company profitability metrics in real time.

---

## 🛠️ Key Project Features & Technical Steps

### 1. Data Transformation & Modeling (Star Schema)
*   **Cleaned Backend Architecture:** Restructured the initial dataset relationships inside the **Power Query Editor** to prevent analytical data errors.
*   **Created Lookup Dimensions:** Generated three unique dimension tables—**Department**, **Product Category**, and **Region**—to act as centralized filter bridges.
*   **Optimized Schema Layout:** Disconnected problematic many-to-many direct tables and arranged them into an industry-standard **Star Schema** (`1 to *` directional relationships).

### 2. Advanced Analytical Measures (DAX)
Developed dedicated, dynamic measures inside a centralized `_CalculatedMeasures` folder to handle financial reporting logic seamlessly:
*   **Total Revenue** = `SUM(Revenue[Revenue])`
*   **Total Cost** = `SUM(Expenses[Expenses])`
*   **Net Profit** = `[Total Revenue] - [Total Cost]`
*   **Profit Margin %** = `DIVIDE([Net Profit], [Total Revenue], 0)`

### 3. Interactive Report UI/UX Design
*   Designed a high-level **KPI Card Header Ribbon** providing executive summaries of top-line performance metrics at a glance.
*   Built interactive **Region dropdown slicers** allowing managers to filter the entire reporting canvas instantaneously.
*   Implemented monthly historical trend lines to cross-examine target distributions against actual variance cycles.

---

## 📂 Repository Directory Layout

```text
├── Budget.csv                           # Corporate target goals data sheet
├── Expenses.csv                         # Operational expenditure tracker sheet
├── Revenue.csv                          # Earned business earnings data sheet
├── KPI Measures.pbix                     # Main Power BI Desktop workspace file
└── Output/                              # Development life-cycle images
    ├── dashboard_skeleton.png           # Empty KPI block layout grid
    ├── data_model.png                   # Optimized Star Schema model view
    ├── final_dashboard.png              # Live fully-functional dashboard view
    └── measures.png                     # Calculated measures setup stage
```

---

## 🚀 How to View and Run the Project
1. Clone or download this GitHub repository to your computer.
2. Open the main data source files to see the raw metrics baseline structure.
3. Download and open **`KPI Measures.pbix`** using **Power BI Desktop** to interactively click, filter, and explore the working dashboard charts!

Developed by **Hemlata** ✨
