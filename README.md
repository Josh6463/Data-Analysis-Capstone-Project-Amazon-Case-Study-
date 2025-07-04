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
-````` Potential Revenue = [@[actual Price]]*[@[Rating Count]]`````

- Price Bucket(Range) = If([@[actual price]]<200,"<#200",If([@[actual price]]<=500,"#200-#500",">#500])

- Ensured proper data types were assigned (e.g.,text, number).

-  Data Exploration (Excel)
1. Used Excel functions (like SUMIFS, AVERAGEIFS, COUNTIFS) to summarize key metrics.

2. Created pivot tables and charts to uncover sales patterns, returns, and customer distribution.

- Data Visualization (Microsoft Excel)
  
1. Built interactive visuals: bar charts, slicers, pie charts.

2. Designed reports to track regional sales, category performance, top-selling products, and more.

- Business Questions Answered
  1.Analyzed metrics such as Potential Revenue, average rating, most profitable       product category, and return rates.
- Insight Generation
 1. Derived conclusions based on visual and statistical evidence.
 2. Identified high-performing category, Product rating distribution.

-  Documentation and Reporting
  1. Summarized key insights and included screenshots of dashboards.
  2. Structured the GitHub repository with clear explanations and organized folders.

### Anatical answers to the Questions Asked in the Project
#### Q1  What is the average discount percentage by product category?
- The below visuals shows the various average discount% by Category and Home Improvement Category to be the Category with the highest Average  Discount% while Toy&Game Category had no Average Discount%.
 ![QUES 1(Chart)](https://github.com/user-attachments/assets/4d0cbf0f-3419-4ed4-9097-2f3dec77757d)

 ![Question 1 Average Discount% by  Category](https://github.com/user-attachments/assets/1b790987-2d60-4f70-8627-ba6a7bd115cf)

#### Q2 How Many Products are Listed Under each Category
- The Chart below shows that Car and Motorbike has 1 product,Computer and Accessory has 453 products,Electronics has 526 products,Health and Personal care has 1 product,Home and Kitchen has 448, Home and Improvement has 2, Musical Instrument has 2,Office Products has 31 and Toys and Games has 1 Product.
- ![Question2(chart)](https://github.com/user-attachments/assets/f98537c1-46a8-43a8-84a9-66064e1a7585)

#### Q3  What is the total number of reviews per category?
![Question 3 (chart)](https://github.com/user-attachments/assets/520b9cba-4495-4501-91f0-1951fc3fc932)
- The above chart provide the Total Number of Review Per Category with Electronic to be Highest Number of review while Car and Motorbike having the Lowest Number of review and reasoned for this answer can be deduced from the Number of Product Listed Under each Category.

  #### Q4 Which products have the highest average ratings? (Question 4)
  The products with the Highest Average Rating (426973) are 
   1. Product with Product ID of B014I8SSD0
   2. Product with Product ID of B014I8X4Y

  #### Q5 What is the average actual price vs the discounted price by category?
![image](https://github.com/user-attachments/assets/83c1ced3-4c30-470e-bd77-1e6e6ca762bb)

The chart above shows the products with the highest number of reviews

The above chart shows the value for the average actual price vs the discounted price by Category
 #### Q6 Which products have the highest number of reviews?
 ![image](https://github.com/user-attachments/assets/acad78ef-15a9-46bc-972a-864e321d7415)

The product with the highest number of reviews is 
 

#### Q7 How many products have a discount of 50% or more?
The Number of Products with a discount of 50%  or more is 751 showing that the products with 50% or more Discount is more than the products with less than 50% Discount

![image](https://github.com/user-attachments/assets/6ce59073-6a39-4b77-be40-1dea0c72d888)

#### Q8 What is the distribution of product ratings (e.g., how many products are rated 3.0,
![image](https://github.com/user-attachments/assets/5cae9088-1b31-414e-adc1-e76345f26404)

The above chart shows that the most Product Rating falls within the range of 3.7-4.5 which could mean that the customers are generally satisfied and Amazon Maintains a high quality product base.

#### Q9 What is the total potential revenue (actual_price × rating_count) by category?
This provide the estimated total Income a category could generate if every Customer who rated a product actually bought the product.
 The Formulae used to format the potential revenue is 
   ```Potential Revenue = actual Price * Rating Count```
 - We can conclude from below chart that Electronics account for the highest Total potential revenue, Indicating its Dominance on Amazon. The Reason for this hug total Potential Revenue could be deduced from;
 - Product Category by Average of Discount%, Electronics has 50.8% Average Discount which happens to the category with the highest Discount.
 - Product ID by Main Category, Electronics has the highest products (526)
 - Total Number of Review By Category, Electronics has the Highest Review by Category and highet rating count.
   
-  High Revenue ≠ High Volume
Some categories may generate high revenue with fewer products, due to higher unit prices.

“Computers & Accessories has fewer products but ranks 2nd in potential revenue — a result of high-ticket items.”
- Growth Opportunity
Low-revenue categories with high ratings and low visibility may be a sign of untapped markets.

“Baby Products show strong ratings but low revenue. Scaling visibility here may yield growth.”

   ![image](https://github.com/user-attachments/assets/c5ae146a-e9f8-4e52-be01-10fdc5d9aa3f)

#### Q10 What is the number of unique products per price range bucket (e.g., <₹200,
₹200–₹500, >₹500)
- The price bucket analysis reveals that 85% of products fall within the range of >500, 12% falls within the of ₦200-₦500range and 3% falls within the range of <#200, indicating Amazon focus on Premium consumer items.
  Low end items (<#200) account for only 3% of total listings, highlighting a potential growth opportunity in the Low cost segment.”

![image](https://github.com/user-attachments/assets/f5a35f22-c865-4373-8052-8c141e165c07)

#### Q11 How does the rating relate to the level of discount?
The scatter graph below shows the following;
An analysis of the relationship between discount level and product rating shows a positive trendline, but with an R² value near zero (2E-13) and a correlation coefficient of ~0.
This indicates no significant correlation between how much a product is discounted and the rating it receives.
Customer satisfaction (as reflected by ratings) appears to be influenced more by product quality or user experience than by price discounts.

![image](https://github.com/user-attachments/assets/9bde3ef2-df6a-4889-9e5f-6ee551a91238)

#### Q12 How many products have fewer than 1,000 reviews?
 Here is a step by step process usded for the calculation of the products with less than 1000 reviews;
 - Insert a Pivot Table
 - Select the full range of your dataset.
 - Go to Insert > PivotTable.
 - Build the Pivot Table
 - Drag Product ID to the Rows area.
 - Drag Rating Count to the Values area:
 - It shows default to Sum of Rating Count.
 -  Apply a Value Filter (Less Than 1000)
 - Click the drop-down arrow on Row Labels (Product ID).
 - Choose Value Filters > Less Than...
 - In the dialog:
 - Select Sum of Rating Count
 - Set it to less than 1000
This gives the number of products with less than 1000 review to be 302.

##### The following Insight could be deduced from the Analysis;
- Products with fewer than 1000 ratings may suffer from low visibility or customer engagement.
- High-rated but low-reviewed products should be prioritized for marketing campaigns.
- Consider incentivizing reviews or bundling these products to increase exposure.
- Track their performance in future analyses to determine growth potential.


  #### Q13 Which categories have products with the highest discounts?
  The Categories that have products with the highest discouts are,
  1. Electronics
  2. Car & Motorbike
  3. Health & Personal care
     The Electronics category contains the product with the highest discount, reflecting the industry’s tendency to use aggressive discounting strategies — possibly due to product obsolescence, inventory clearance, or promotional campaigns.”

#### Q14 Identify the top 5 products in terms of rating and number of reviews combined.

The top 5 products in terms of rating and number of reviews are 
- product with ID of B014I85SSDO
- product with ID of B014I8sx4Y
- product with ID of B07KsMBL2H
- product with ID of B071Z8M4KX
- product with ID of B07GQD4k6L
 


   




