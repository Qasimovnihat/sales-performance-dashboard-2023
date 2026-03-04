# Sales Performance Analysis (2023) — Power BI + Excel

This project cleans (in Excel), analyzes, and visualizes **2023 sales data** using an interactive **Power BI dashboard**. 
The goal is to track sales, discounts, and profit performance across key segments and evaluate how discount levels affect profit margin.

---

## Project Goals
- Monitor overall 2023 sales performance with KPI cards
- Analyze monthly sales and profit trends
- Compare performance by region, category, channel, payment method, and customer type
- Measure the relationship between **discount** and **profit margin** using correlation and **p-value** testing

---

## Dataset Overview (Main Columns)
- `Product_ID`, `Sale_Date`, `Sales_Rep`, `Region`
- `Quantity_Sold`, `Product_Category`
- `Unit_Cost`, `Unit_Price`
- `Customer_Type`, `Discount`, `Payment_Method`, `Sales_Channel`
- Calculated columns: `Total_Sales`, `Xerc` (Total Cost), `Profit`, `Profit_Marjin`

---

## Data Cleaning & Preparation (Excel)
Data preparation was performed in Excel and includes:
- Removing **duplicate** records
- Handling **missing (null)** values (filled using appropriate methods such as mean/mode/business logic)
- Cleaning incorrectly entered values (format issues / inconsistent entries)
- Applying correct **data types & formatting** (date, numeric, percentage)
- Creating calculated columns:
  - **Total Sales:** `Quantity_Sold * Unit_Price * (1 - Discount)`
  - **Total Cost:** `Quantity_Sold * Unit_Cost`
  - **Profit:** `Total_Sales - Total_Cost`
  - **Profit Margin:** `Profit / Total_Sales`

---

## Analysis & Statistical Checks
- Segment analysis by: Region / Category / Channel / Payment Method / Customer Type
- **Correlation** check (correlation matrix)
- **P-value testing** to validate relationships (e.g., `Discount` vs `Profit_Marjin`)

---

## Power BI Dashboard (2 Pages)

### 1) Sales Performance 2023
- KPI Cards: **Total Sales**, **Discount Amount**, **Total Profit**, **Profit Margin**, **Quantity Sold**
- Visual: Monthly **Sales vs Profit** trend
- Slicers: Region, Category, Payment Method, Customer Type

### 2) Discount & Profit Analysis
- Monthly **Sales vs Average Discount** trend
- **Discount share by category**
- Scatter plot: **Discount % vs Profit Margin**
- Profit margin by **discount range** (binned analysis)

---

## Key Insights (from the dashboard)
- Higher discounts tend to reduce **profit margin**, especially in the highest discount ranges.
- Discount distribution varies by category (e.g., Electronics shows a higher discount share).

