# June 2025 Shop Sales Analysis
<img width="1149" height="652" alt="ta" src="https://github.com/user-attachments/assets/fffa3eca-c3dc-40c4-8e7d-6f96916270a4" />
A Power BI Business Intelligence Report

## 1. Executive Summary
This project involved a comprehensive business intelligence analysis of shop sales data for June 2025. The goal was to transform raw sales data into a professional and interactive Power BI dashboard, providing key insights into overall business performance, top-performing shops, product sales, and customer behavior. The final report delivered actionable recommendations to drive strategic decision-making.

## 2. Problem Statement & Objectives
The management team required a clear, data-driven report to understand the previous month's sales performance. The key business questions to be answered were:

* What was the total revenue and total quantity sold for the month?
* Which retail shops were the top performers?
* Which specific products (PROFILE SOLD) were generating the most revenue?
* What was the sales performance of different profile types (PF vs. Coloured)?
* What was the total amount of discounts applied?
* How did sales break down across different payment methods (Cash, POS, Bank Transfers)?
* How many repeat customers were there during the month?

## 3. Data Source
The data was provided in a single CSV file, JUNE 2025 SHOP SALES (Autosaved).csv, containing granular transaction details.

## 4. Methodology & Process
The project followed a standard business intelligence workflow, from data preparation to visualization and reporting.

### Data Preparation & Transformation (Power Query)
The raw CSV file was loaded into Power Query for a series of data cleaning and transformation steps to ensure data quality and structure were suitable for analysis. This included:

* Creating a Unique Identifier: A calculated column, Customer Visit ID, was created to uniquely identify each transaction.
* Unpivoting Columns: To facilitate charting of bank transfers, the ZENITH BANK TRANSFER, ACCESS BANK TRANSFER, and FIRST BANK TRANSFER columns were unpivoted into a single Bank Name column and a Bank Sales Amount column. This was crucial for visualizing bank performance in a clustered column chart.
* Categorization: A conditional column, Profile Type Category, was added to categorize each sale as a "PF Profile," "Coloured Profile," or "Other" based on the rate columns.

### Data Modeling & Measures (DAX)
A simple data model was established, and the following key DAX measures were created to drive the dashboard's insights:

* Total Revenue: Sum of all amounts.
* Total Quantity Sold: Sum of all quantities.
* Total Discount Given: Sum of all discounts.
* Customer Total Visits: A measure using DISTINCTCOUNT on Customer Visit ID to accurately count unique visits per customer.

### Visualization & Dashboard Design
<img width="1152" height="647" alt="taa" src="https://github.com/user-attachments/assets/8e240471-9d8a-474f-b23d-a7a90e9a3243" />

<img width="1156" height="645" alt="taaa" src="https://github.com/user-attachments/assets/dacfc4b6-e89c-461f-a821-97d5b7fa48cd" />

<img width="1152" height="650" alt="taaaa" src="https://github.com/user-attachments/assets/fdcd291e-c8a0-4228-80e6-3598df0e9c47" />

<img width="1151" height="648" alt="taaaaa" src="https://github.com/user-attachments/assets/a0feb1fc-cb2f-43b5-a38e-8611c965aa9e" />

Two primary dashboards were designed in Power BI to provide a clear and organized view of the data. The design was clean and focused on readability.

* **June 2025 Sales Dashboard Overview**: This dashboard provides a high-level summary of the entire month's performance. It includes key performance indicator (KPI) cards, top-performing shops, top-selling products, and a breakdown of sales by payment method.
* **Retail Shop Performance Dashboards**: A separate, detailed dashboard was created for each retail shop (Shop 1, Shop 2, Plaza, Ifelodun). These dashboards use a RETAIL SHOP slicer to allow users to drill down into individual shop performance, including revenue, product sales, and customer visit frequency.

## 5. Key Findings & Business Insights
* Concentrated Performance: Total revenue was ₦45M, with Shop 2 alone contributing over 55% of total sales, highlighting a significant performance gap.
* Coloured Profiles Dominate: Coloured Profiles were the primary revenue driver, accounting for over 61% of total sales.
* Top Products: DECURVE GREY, DECURVE WHITE, and TRANZIUM DARK GREY were the highest-earning products.
* Payment Channels: Access Bank transfers proved to be the most used bank transfer method.
* Customer Loyalty: 93 unique customers were identified, with a few making repeat visits, suggesting a small but present loyal customer base.

## 6. Tools & Technologies
* Power BI: Data visualization, modeling, and reporting.
* Power Query: Data cleaning, transformation, and shaping.
* DAX (Data Analysis Expressions): Creating custom measures for advanced calculations.

 this dashboard to Power BI Service, you can include a link here so others can interact with it.]

