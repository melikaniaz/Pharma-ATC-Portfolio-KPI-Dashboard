
Pharma ATC Portfolio & KPI Dashboard
Power BI dashboard analyzing a 6‑year pharmaceutical sales dataset (2014–2019) at ATC class level. The project focuses on turning raw monthly sales data into executive‑ready KPIs and visual insights that support portfolio and strategy decisions in a life‑science context.

Dataset
Source: Kaggle – pharma sales data (monthly, 2014–2019)

Granularity: Monthly sales aggregated by ATC class (M01AB, M01AE, N02BA, N02BE, N05B, N05C, R03, R06)

Key fields used:

Date – month end

ATC – Anatomical Therapeutic Chemical (ATC) classification code

MonthlySales – aggregated sales value per ATC and month

Goals
Build an executive‑style dashboard to track pharma KPIs over time

Analyze portfolio performance across therapeutic classes (ATC groups)

Provide interpretable insights for market and focus decisions (e.g. which ATC segments drive most of the volume and where growth is declining)

Data Modeling
Reshaped the dataset from wide format (one column per ATC) to long format (Date, ATC, MonthlySales) for better modeling in Power BI

Created a calculated Year column from Date for time‑series analysis

Added derived fields (e.g. ATC share, coverage metrics) using DAX measures

KPIs and DAX Measures
Key measures implemented:

Total Sales – sum of MonthlySales across the selected period and ATC classes

Total Sales YoY % – year‑over‑year percentage change in total sales for the selected year

Number of Months – distinct count of months covered in the filtered context

ATC Share % – share of each ATC in total sales for the selected context

(Optional) Average Monthly Sales – average total sales per month

These measures are used to track overall performance, growth, data coverage and the relative importance of each ATC class.

Dashboard Layout
The main report page contains:

KPI Cards

Total Sales

Total Sales YoY %

Number of Months

Trend View

Line chart: Total Sales by Year (2014–2019) to highlight long‑term growth and decline patterns.

Portfolio View

Clustered bar chart: Total Sales and ATC Share % by ATC to show both absolute sales and portfolio share per ATC class.

This view allows quick identification of high‑volume and high‑share therapeutic classes (e.g. analgesics, psycholeptics, respiratory, antihistamines).

How to Use
Open the .pbix file in Power BI Desktop.

Interact with slicers (years, ATC classes if added) to explore different time windows and portfolio segments.

Use the visuals to:

Assess overall portfolio performance

Compare ATC classes by absolute sales and share

Spot years with declining or accelerating growth

Role in My Portfolio
This project showcases:

Building an end‑to‑end Power BI dashboard from a raw pharma dataset

Translating ATC‑level sales data into strategy‑relevant KPIs and visuals

Communicating portfolio and market insights for a life‑science setting, similar to strategy and transformation work in biopharma environments.

