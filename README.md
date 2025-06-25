#  Project Title
 Amazon Product Review Analysis

##  Brief Description of the Project
This project explores Amazon's sales data to extract actionable business insights using Excel and Power BI. It involves data cleaning, exploration, visualization, and key performance indicator tracking

##   Dataset Description
The dataset contains information scraped from Amazon product pages, including:
• Product details: name, category, price, discount, and ratings
• Customer engagement: user reviews, titles, and content
• Each row represents a unique product, with aggregated reviewer data
stored as comma-separated values
Total Records: 1,465 rows
TotalFields: 16 columns

## Tools Used
- Excel [Download here](www.microsoft.com)
- Power BI

## Analysis Tasks
Use pivot tables and calculated columns where necessary to answer the following:
1. What is the average discount percentage by product category?
2. How many products are listed under each category?
3. What is the total number of reviews per category?
4. Which products have the highest average ratings?
5. What is the average actual price vs the discounted price by category?
6. Which products have the highest number of reviews?
7. How many products have a discount of 50% or more?
8. What is the distribution of product ratings (e.g., how many products are rated 3.0,
4.0, etc.)?
9. What is the total potential revenue (actual_price × rating_count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200,
₹200–₹500, >₹500)
11. How does the rating relate to the level of discount?
12. How many products have fewer than 1,000 reviews?
13. Which categories have products with the highest discounts?
14. Identify the top 5 products in terms of rating and number of reviews combined.
4. Final Task: Dashboard Creation
Using your cleaned dataset and pivot outputs, build an Excel dashboard. Unleash your
Creativity

##  Introduction
In today’s data-driven e-commerce landscape, understanding customer behavior, product performance, and regional trends is crucial for maximizing profitability and enhancing customer satisfaction. This project presents a comprehensive analysis of Amazon sales data with the aim of uncovering key business insights through data visualization and reporting.
Using tools like Microsoft Excel and Power BI, the project covers essential processes such as data cleaning, exploration, aggregation, and dashboard creation. The dataset includes various fields such as Product IDs, review content, review names, product categories,actual price, discounts Percentage, ratings,and rating count - offering a rich foundation for analysis.

The primary objective of this case study is to:

- Evaluate Products and profitability trends across the categories.
- Understand customer purchase behavior through ratings and return analysis.
- Identify underperforming poduct and highly performing product to recommend business improvements.

This analysis helps to simulate a real-world scenario in which a data analyst supports strategic decision-making at a large-scale online retailer like Amazon. Whether you are a business stakeholder or a fellow data enthusiast, this case study provides valuable insights into how raw data can be transformed into powerful business intelligence.

### Steps Taken in the Analysis
         Data Collection
Downloaded the dataset from LMs containing Amazon Product transactions, including columns such as Product ID, Rating, Rating Count, Category,Product Name, Discount, Actual Price, and some other Important Data for the Analysis.

       Data Cleaning
- Extraction of Data (Main category) from the Category usig Excel function  ````= left(D2,find("|",D2&"|")- 1)````. This formulae help to extract the First Statement before the first "|" in the category column.
- formatted a new column that contains the data set extracted from the Category and Named the Column "Main Category"
- Created the needed Column for answering the Analytical Questions like the Potential Revenue, Price Range(Bucket) using the below formula                                                        
````` Potential Revenue = [@[actual Price]]*[@[Rating Count]]`````

````` Price Bucket(Range) = If([@[actual price]]<200,"<#200",If([@[actual price]]<=500,"#200-#500",">#500"````

  
Standardized date formats and numerical values to prepare for accurate analysis.

Ensured proper data types were assigned (e.g., date, text, number).

📊 Data Exploration (Excel)
Used Excel functions (like SUMIFS, AVERAGEIFS, COUNTIFS) to summarize key metrics.

Created pivot tables and charts to uncover sales patterns, returns, and customer distribution.

Data Visualization (Microsoft Excel)
Imported the cleaned dataset into Microsoft DExcel for dynamic dashboard creation.

Built interactive visuals: bar charts, slicers, pie charts, KPIs, and maps.

Designed reports to track regional sales, category performance, top-selling products, and more.

 Business Questions Answered
Analyzed metrics such as total revenue, average rating, most profitable product category, and return rates.

Compared trends across regions and time periods to provide actionable insights.

 Insight Generation
Derived conclusions based on visual and statistical evidence.

Identified high-performing regions, areas of customer dissatisfaction, and seasonal purchase trends.

📌 Documentation and Reporting
Summarized key insights and included screenshots of dashboards.

Structured the GitHub repository with clear explanations and organized folders.

