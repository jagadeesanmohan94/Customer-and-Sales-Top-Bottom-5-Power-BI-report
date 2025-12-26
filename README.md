# Customer-and-Sales-Top & Bottom 5 Power-BI-report

Dashboard Link:

https://capgemini-my.sharepoint.com/personal/jagadeesan_mohan_capgemini_com/Documents/Customer%20sale%20From%20Excel.pptx?web=1

![Image](https://github.com/user-attachments/assets/3bafc3aa-6203-437f-b593-b28d9a75df7d)

⭐ SUMMARY

This Power BI report demonstrates a highly structured, analytical, and business‑oriented sales intelligence solution. The data model uses a clean Star Schema supported by dual date tables for comparative analysis. The visuals successfully uncover insights into product performance, profitability, customer behavior, promotional effectiveness, and long‑term sales trends.
Strengths of the Report:

![Image](https://github.com/user-attachments/assets/1a0fd9af-b7e3-4901-973b-75e2b3f5edd5)

Clear KPI visibility (Orders, Sales, Profit)
Strong use of Top/Bottom N analytics
Insightful product segmentation (Top 5 & Bottom 5)
Correlation analysis validating business consistency
Geo‑level insights showing city performance
Well‑implemented dual date filter for period comparison
Customer‑level granularity for deeper insights
Professional data modeling with correct relationships


1️⃣ Date Table Creation Using CALENDARAUTO()
Your report uses the DAX expression:
Date Table 1 = CALENDARAUTO()

![Image](https://github.com/user-attachments/assets/08b027d9-b9de-43e4-9d6b-e85ec3f6c09c)

What This Means:

CALENDARAUTO() automatically scans the entire data model, detects the earliest and latest date values, and builds a continuous date table.
This table enables:

Time intelligence (YTD, MTD, QTD)
Year‑on‑year comparisons
Accurate trend analysis

![Image](https://github.com/user-attachments/assets/5b4c9936-2d03-4cab-86ff-4f837b0b55b1)

Your report contains two date tables, meaning you have set up:

Date Table 1 → Main timeline filtering
Date Table 2 → Comparison filtering
This design is commonly used for dual‑period comparison dashboards.


2️⃣ Data Model – Table Structure
Your model includes:
Fact Table
Contains:

CustomerID
Date
Product ID
Promotion ID
Net Sales
Total Sales
Profit
Discount
Units Sold
Price per Unit



Dimension Tables

![Image](https://github.com/user-attachments/assets/f42b2d7c-6ddb-4576-bd28-f2df1e5f5028)

Dim Customers (City, Customer Name, Contact, Pin Code, State)
Dim Product (Price, Product Line, Product Name, Product ID)
Dim Promotion (Promotion Type, Discount, Coupon Code)
Date Table 1
Date Table 2

What This Shows:

![Image](https://github.com/user-attachments/assets/a82e2842-4b16-4873-874f-de5f06bf656b)

This is a perfect Star Schema (Fact table in the center, surrounded by dimension tables).
All relationships appear to be one‑to‑many, which is ideal.
Using two date tables allows side‑by‑side comparisons without slicer conflicts.


3️⃣ Top N / Bottom N Filtering
You are using a Top N filter configured as:

![Image](https://github.com/user-attachments/assets/1a0313ac-453d-48c9-bcc1-60bf0ab0cf06)

Type: Top N
Mode: Bottom 5
Metric: Sum of Net Sales

This filter drives the Bottom 5 Product charts, helping identify:

Lowest sales contributors
Products needing strategic correction (pricing, marketing, stocking)


4️⃣ KPI & Overview Dashboard Analysis
Your main dashboard page includes:
KPIs

Total Orders: 3510
Average Discount by Promotion Category
Profit vs Net Sales Correlation
Sales Trend from 2020–2024
City‑wise Sales Distribution

Insights:

Major cities like Mumbai, Delhi, Bengaluru show higher sales.
Weekend Flash Sale offers the highest discount.
A strong linear relationship between Profit and Net Sales suggests:

Profitability scales consistently with revenue.


Sales trend shows periodic spikes—likely linked to promotions and festive seasons.


5️⃣ Bottom 5 Product Performance
You evaluated products on:

Sales
Quantity
Profit

![Image](https://github.com/user-attachments/assets/151b632f-d9ca-43c9-8259-a6aec9bad786)

Key Observations:

Items like Tupperware Lunch Box, Dove Soap Pack, and Colgate Toothpaste are underperforming.
FMCG products have low profitability despite volume.
Tupperware appears low in all three categories → candidate for review.


6️⃣ Top 5 Product Performance
You identified the strongest performers by Sales, Quantity, and Profit.
Insights:

Apple iPhone 14 leads in:

Sales
Quantity Sold
Profit
This shows a high‑value, high‑demand, high‑margin product.

![Image](https://github.com/user-attachments/assets/b02f9b09-9af2-4432-8c84-db68dd195678)

Electronics dominate the top ranks.
Apparel and kitchen appliances appear in quantity‑based rankings, indicating:

High volume
Lower margin




7️⃣ Profit vs Net Sales Correlation
A scatter plot reveals almost a perfect upward trend.
Interpretation:

![Image](https://github.com/user-attachments/assets/6d4be828-d8d2-4575-9a23-0be5931b15a2)

As Net Sales increase, Profit increases proportionally.
No major loss‑making outliers.
Suggests consistent pricing strategy and healthy margins.


8️⃣ Promotional Discount Analysis
Promotion categories show varying average discount levels.
Key Findings:

![Image](https://github.com/user-attachments/assets/9534ea81-0bc8-4a85-9e52-dec74161cc97)

Weekend Flash Sale → Highest discount
Festive Diwali → Lowest discount
Clearance and Summer sales offer moderate discounts.

This helps evaluate:

Which promotions drive volume
Which promotions maintain profitability


9️⃣ Sales Trend Analysis (2020–2024)
You presented a long‑term sales trend with point markers.
Insights:

Sales spikes occur periodically each year.
Peak values around mid‑2021, 2023, and festive periods.
No drastic drop year‑to‑year, indicating stable business performance.

![Image](https://github.com/user-attachments/assets/1f3e1636-b35d-4b11-ad77-fa8c35c72be2)

🔟 Dual Date Filter Comparison (Period vs Period)
Your dashboard uses two independent date slicers, each tied to separate date tables.
Purpose:

Compare:

Year vs Year
Season vs Season
Promotion Period vs Non‑Promotion
Before vs After Covid periods



Metrics compared:

Total Sales
Total Profit
Total Quantity

Both date sets display side‑by‑side results.

![Image](https://github.com/user-attachments/assets/467dea93-d87d-493d-a7b6-34f340fc4c3d)



1️⃣1️⃣ Customer‑Level Transaction Details
The detailed table shows:

CustomerID
OrderID
Date
Discount
Net Sales
Product ID
Units Sold
Profit
Promotion details

This dataset supports:

Customer profiling
Repeat purchase analysis
High‑value customer targeting


![Image](https://github.com/user-attachments/assets/05bf904f-499c-4184-86f2-7c769e980447)
