# Amazon Product Review Analysis: Case Study 1
by Damilola Abraham Olagunju
### Project Overview

### Table of Contents
[Company Overview](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/edit/main/README.md#company-overview)

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

### Analysis 
The data was cleaned and analyzed using Microsoft Excel 2013. 

Duplicates were removed using product ID, then the data type of the fields were changed accordingly (e.g. those that are prices to *currency datatype*). 

New columns for price bucket range, total potential revenue and a count flag were created to facilitate the analysis.

Pivot tables were then made from the cleaned dataset, and used to make inferences and charts.

### Answers to questions/Explorative data analysis
1. What is the average discount percentage by product category?

![Average discount percentage by product category](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/55876d851a2e5c46d1e362541a611efee333cedb/Average%20Discount%20by%20Product%20Category.png)

*The image above shows a chart comparing the average discount.*

It is observed that the category with the highest average discount percentage by product is **Home Improvement**, 57.50%; while the **Toy and Games** category is the lowest on the list with no discount. 


2. How many products are listed under each category?

![Products listed under each category](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/No.%20of%20Products%20Per%20Category.png)

The category with the highest number of products is **Electronics**, and the ones with the least number of products are **Toys & Games**, **Health & Personal Care** and **Car & Motorbike**.


3. What is the total number of reviews per category?

![Total Number of Reviews Per Category](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Total%20number%20of%20reviews%20per%20category.png)


4. Which products have the highest average ratings?

![Product with Highest Average Ratings](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Product%20with%20highest%20average%20ratings.png)

The top 10 products with the highest average ratings are shown in the chart depicted by their product ID. The top 3 products are **Amazon Basics Wireless Mouse**, **Syncwire LTG to USB Cable** and **REDTECH USB-C to Lightning Cable 3.3FT** all with ratings of 5.0.

5. What is the average actual price vs the discounted price by category?

![Average price vs discounted price by category](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Average%20Discount%20by%20Product%20Category.png)

6. Which products have the highest number of reviews?

![Products with Highest Number of Reviews](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Products%20with%20Highest%20Number%20of%20Reviews.png)

*The chart above shows the products with the highest number of reviews. The products are depicted by product ID*

The top 3 are:
- AmazonBasics Flexible Premium HDMI Cable (Black, 4K@60Hz, 18Gbps), 3-Foot

  Product ID: B07KSMBL2H

  Number of Reviews: 426,973

- Amazon Basics High-Speed HDMI Cable, 6 Feet - Supports Ethernet, 3D, 4K video,Black

  Product ID: B014I8SSD0

  Number of Reviews: 426,973

- Amazon Basics High-Speed HDMI Cable, 6 Feet (2-Pack),Black

  Product ID: B014I8SX4Y

  Number of Reviews: 426,973


7. How many products have a discount of 50% or more?

![Products with discount of 50% or more](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Count%20of%20products%20with%20percentage%20higher%20than%2050%25.png)

The formula used was

``` =COUNTIF('working sheet'!$G$2:$G$1352, ">=50%") ```

8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?

![Distribution of Product Ratings](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Distribution%20of%20Product%20Ratings.png)

The chart shows that the most of the products have a good rating, with most of the products - 225 of them - having a rating of 4.1.

9. What is the total potential revenue (actual_price × rating_count) by category?

![Total Potential Revenue by Category](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Total%20Potential%20Revenue%20by%20Category.png)

From the chart, we can observe that the category that brought the highest revenue is the **Electronics** category, followed by the **Computer & Accessories** and **Home and Kitchen** with total potential revenues of approximately 91 billion, 12 billion, and 10 billion respectively.

10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?

![Number of Unique Products per Price Range](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Number%20of%20Unique%20Products%20per%20Price%20Range.png)

This shows that most of the products - 1166 of them - cost more than ₹500, the ones less than ₹500 are 34 in number while the rest of the products have a cost within a range of ₹200 to ₹500. 

11. How does the rating relate to the level of discount?

![Rating vs Discount Percentage](https://github.com/the-questerr/D.-Olagunju-DSA-Ms.-Excel-Project-1/blob/main/Rating%20vs%20Discount%20Percentage%20(2).png)

It is observed that 

12. How many products have fewer than 1,000 reviews?




13. Which categories have products with the highest discounts?



14. Identify the top 5 products in terms of rating and number of reviews combined.



### Dashboard

### Observation and Recommendation
- As it has been observed that **Electronics**, **Computer & Accessories**, **Home & Kitchen** are the categories with the highest potential revenue, there should be actions to improve sales of products in these categories.
- 

- From the analysis, it was seen that rating is not exactly directly proportional to the increasing discount percentage. 
Infact, the products with the 3 lowest discount percentages have a ratingn of more than 4.0. The producst with the 
lowest discount percentages of 38.81%, 39.66% and 44.49% have a rating of 4.5, 4.4 and 4.3 respectively while the 
highest discount rates, 68.33%, 72.0% and 81.50% have ratings of 5, 2.9, and 2.8 respectively. 



### Challenges/Limitations
There were some error values which I used my discretion to take care of. 
  
