# D.-Olagunju-DSA-Capstone-Project-1
This is the documentation of my Excel Project for the DSA Data Analysis Course.

## Project Topic: Amazon Product Review Analysis: Case Study 1
### Project Overview
#### Company Overview
You are working as a Junior Data Analyst at RetailTech Insights, a company that provides e-commerce analytics solutions to sellers on platforms like Amazon. Your team has been tasked with analysing product and customer review data to generate insights that can guide product improvement, marketing strategies, and customer engagement.
  
#### Dataset Description
The raw dataset(I want to put a link to the Excel file given to us here) contains information scraped from Amazon product pages, including:
- Product details: name, category, price, discount, and ratings
- Customer engagement: user reviews, titles, and content
- Each row represents a unique product, with aggregated reviewer data stored as comma-separated values

Total Records: 1,465 rows

Total Fields: 16 columns

#### Analysis Tasks
 Use pivot tables and calculated columns where necessary to answer the following:
1. What is the average discount percentage by product category?
2. How many products are listed under each category?
3. What is the total number of reviews per category?
4. Which products have the highest average ratings?
5. What is the average actual price vs the discounted price by category?
6. Which products have the highest number of reviews?
7. How many products have a discount of 50% or more?
8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?
9. What is the total potential revenue (actual_price × rating_count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?
11. How does the rating relate to the level of discount?
12. How many products have fewer than 1,000 reviews?
13. Which categories have products with the highest discounts?
14. Identify the top 5 products in terms of rating and number of reviews combined.

*Final Task: Dashboard Creation*
Using your cleaned dataset and pivot outputs, build an Excel dashboard. Unleash your creativity

### Data Source(s)
The data was given by DSA, The Incubator Hub.

### Analysis (how it was analyzed, steps, methods)
The data was cleaned and analyzed using Microsoft Excel 2013. 

Duplicates were removed using product ID, then the data type of the fields were changed accordingly (e.g. those that are prices to *currency datatype*). 

New columns for price bucket range, total potential revenue and a count flag were created to facilitate the analysis.

Pivot tables were then made from the cleaned dataset.

### Answers to questions/Explorative data analysis

### Dashboard

### Recommendation
### Challenges/Limitations
  
