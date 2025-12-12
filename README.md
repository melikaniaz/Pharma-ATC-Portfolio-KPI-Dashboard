# Pharma ATC Portfolio & KPI Dashboard

Power BI dashboard analyzing a 6‑year pharmaceutical sales dataset (2014–2019) at ATC class level. The project focuses on turning monthly sales data into executive‑ready KPIs and visual insights that support portfolio and strategy decisions in a life‑science context.

## Dataset

- **Source:** Kaggle – pharmaceutical sales data (monthly, 2014–2019)  
- **Granularity:** Monthly sales aggregated by ATC class (M01AB, M01AE, N02BA, N02BE, N05B, N05C, R03, R06)  
- **Main fields:**
  - `Date` – month end  
  - `ATC` – Anatomical Therapeutic Chemical (ATC) classification code  
  - `MonthlySales` – aggregated sales value per ATC and month  

## Goals

- Build an executive‑style dashboard to track pharma KPIs over time  
- Analyze portfolio performance across therapeutic classes (ATC groups)  
- Provide interpretable insights for market and focus decisions (which ATC segments drive most of the volume, where growth is declining)

## Data Modeling

- Reshaped the dataset from wide format (one column per ATC) to long format (`Date`, `ATC`, `MonthlySales`) for better modeling in Power BI  
- Created a calculated `Year` column from `Date` for time‑series analysis  
- Added derived measures (e.g. ATC share, coverage metrics) using DAX

## KPIs and DAX Measures

Key measures:

- **Total Sales** – sum of `MonthlySales` across the selected period and ATC classes  
- **Total Sales YoY %** – year‑over‑year % change in total sales for the selected year  
- **Number of Months** – distinct count of months covered in the current filter context  
- **ATC Share %** – share of each ATC in total sales  
- *(Optional)* **Average Monthly Sales** – average total sales per month  

These KPIs track overall performance, growth, data coverage and the relative importance of each ATC class.

## Dashboard Layout

1. **KPI Cards**
   - Total Sales  
   - Total Sales YoY %  
   - Number of Months  

2. **Trend View**
   - Line chart: *Total Sales by Year* (2014–2019) to highlight long‑term growth/decline patterns.

3. **Portfolio View**
   - Clustered bar chart: *Total Sales and ATC Share % by ATC* to show both absolute sales and portfolio share per therapeutic class.

## How to Use

1. Open the `.pbix` file in **Power BI Desktop**.  
2. Use slicers (e.g. Year, ATC) to explore different time windows and portfolio segments.  
3. Read the visuals to:
   - Assess overall portfolio performance  
   - Compare ATC classes by sales and share  
   - Spot years with declining or accelerating growth  

## Why This Project

This project demonstrates:

- Building an end‑to‑end Power BI dashboard from a raw pharma dataset  
- Translating ATC‑level sales data into strategy‑relevant KPIs and visuals  
- Communicating portfolio and market insights for a life‑science setting, similar to strategy & transformation work in biopharma.
