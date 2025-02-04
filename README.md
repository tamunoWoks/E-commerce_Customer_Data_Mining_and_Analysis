# E-commerce Customer Data Mining and Analysis
This is a data-driven study with Python that focuses on customer satisfaction from Ecommerce data

## Data Overview
The [dataset](https://github.com/tamunoWoks/E-commerce_customer_satisfaction_analysis/blob/main/npa.csv) used for this case study was sourced from [staso.io](https://statso.io/customer-satisfaction-case-study/). It comprises various attributes related to customer demographics, purchasing behavior, and satisfaction ratings for an e-commerce platform. Key features include:

- CustomerID: Unique identifier for each customer.
- Age: Age of the customer.
- Gender: Gender of the customer (Male/Female).
- PurchaseAmount: Total amount spent by the customer.
- PurchaseFrequency: Number of purchases made by the customer.
- ProductQualityRating: Customer rating for product quality (1-5).
- DeliveryTimeRating: Customer rating for delivery time (1-5).
- CustomerServiceRating: Customer rating for customer service (1-5).
- WebsiteEaseOfUseRating: Customer rating for website ease of use (1-5).
- ReturnRate: Proportion of products returned by the customer.
- DiscountUsage: Amount of discount used by the customer.
- LoyaltyProgramMember: Whether the customer is a loyalty program member (Yes/No).

## Problem Statement
The primary goal is to perform a comprehensive analysis of customer satisfaction to identify key factors influencing satisfaction and areas needing improvement. This involves:

- **Understanding Satisfaction Drivers:** Identifying which aspects (product quality, delivery time, customer service, website usability) most significantly impact overall customer satisfaction.
- **Demographic and Behavioral Insights:** Analyzing how satisfaction varies across different demographic groups (age, gender) and purchasing behaviors (purchase amount, frequency, discount usage).
- **Loyalty Program Effectiveness:** Evaluating the impact of loyalty program membership on customer satisfaction and retention.
- **Root Cause Analysis:** Identifying the root causes of dissatisfaction to provide actionable recommendations for enhancing customer experience.
- **Net Promoter Score (NPS):** Calculating the NPS to gauge overall customer loyalty and identify areas to convert detractors into promoters.

## Insights
- The statistical summary of the dataset provided insights into the central tendency, dispersion, and range of the numeric data, and here are some key observations:
  - **Age:** The average customer age is around 44 years, with a range from 18 to 69 years.
  - **Purchase Amount:** The average purchase amount is $1065, with a significant standard deviation indicating variability in spending.
  - **Purchase Frequency:** Customers purchase on average about 14 times, with some making up to 29 purchases.
  - **Ratings:** The average ratings for product quality, delivery time, customer service, and website ease of use are around 3, indicating moderate satisfaction levels. These ratings range from 1 (poor) to 5 (excellent).
  - **Return Rate:** The average return rate is 25%, with some customers having a return rate as high as 50%.
  - **Discount Usage:** The average discount usage is around $251, with high variability.

- The histogram portraying the numerical columns in the dataset revealed the following:
  - Age distribution is relatively even with slight peaks in the 30s and 60s;
  - Purchase amounts are right-skewed, indicating most customers spend less than $1000;
  - Purchase frequency is varied, with notable peaks around 10 and 20 purchases;
  - Discount usage is evenly spread, showing no significant trend.
  - Satisfaction ratings for product quality, delivery time, customer service, and website ease of use show a wide distribution, with most ratings clustering around the middle values;
  - Return rates are varied with peaks around 0.1 and 0.4.  
These findings suggest that customer experiences and behaviours are diverse, with varying levels of satisfaction across different service aspects.

- After segmenting the customers based on demographic and behavioral factors, the data shows the average satisfaction ratings by age group and gender for different aspects of service. Here are some insights:
  - Younger customers (18-29) generally rate product quality slightly higher.
  - Females in the 40-49 age group give the highest ratings, while males in the 60-69 age group give the lowest.
  - Delivery time satisfaction is relatively consistent across age groups, with minor variations.
  - The highest ratings for delivery time satisfaction are from females aged 60-69, while the lowest are from males aged 30-39.
  - Customer service ratings are fairly consistent, with a slight peak among younger males (18-29).
  - Males in the 60-69 age group rate customer service the lowest.

- After segmenting the numeric columns by the loyalty program, the data shows mean satisfaction ratings, return rates, and discount usage for loyalty program members versus non-members. Here are the insights:
  - **Product Quality Rating:** Loyalty program members rate product quality slightly higher (2.95) compared to non-members (2.92).
  - **Delivery Time Rating:** Loyalty program members are more satisfied with delivery time (3.09) than non-members (2.92).
  - **Customer Service Rating:** Members rate customer service higher (3.16) compared to non-members (2.99).
  - **Website Ease of Use Rating:** Non-members rate the website slightly higher (3.11) than members (3.06).
  - **Return Rate:** The return rates are almost identical between members (0.25) and non-members (0.25).
  - **Discount Usage:** Members use slightly more discounts ($260) compared to non-members ($241).

- Net Promoter Score (NPS) is a metric used to gauge customer loyalty and satisfaction by asking customers how likely they are to recommend a company’s product or service to others on a scale of 0 to 10. Respondents are classified into three categories:
  1. Promoters (9-10)
  2. Passives (7-8)
  3. Detractors (0-6).  
The NPS is calculated by subtracting the percentage of Detractors from the percentage of Promoters.  
A higher NPS indicates more customer loyalty and positive word-of-mouth, which are critical for business growth.  
To calculate the NPS, we will use customer service ratings as a proxy for overall satisfaction.  

    The NPS calculation shows:  
          - **Detractors:** 100% of customers fall into the Detractors category.  
          - **Passives:** 0%.  
          - **Promoters:** 0%.  
      This results in an NPS score of -100, which indicates extremely low customer satisfaction.  
      This score is a critical indicator that significant improvements are needed in customer service to convert detractors into promoters.

- After performing root cause analysis to analyze customers who gave low ratings (≤ 2) in different aspects (ProductQualityRating, DeliveryTimeRating, CustomerServiceRating, and WebsiteEaseOfUseRating), and then visualizing the characteristics of these customers using histograms for age, purchase amount, purchase frequency, and return rate. here are some insights:
  - Customers giving low ratings span a wide age range, with notable peaks around ages 30-40 and 50-60, which suggests age-related dissatisfaction trends.
  - Purchase amount and frequency distributions reveal that low ratings are not limited to low spenders or infrequent buyers; even high spenders and frequent buyers express dissatisfaction, which shows service quality issues.
  - The return rate distribution shows that higher return rates correlate with low ratings, particularly for product quality and website ease of use, which indicates dissatisfaction with product and website experiences.

- After analyzing customer satisfaction by examining the ratings provided by customers for Product Quality, Delivery Time, Customer Service, and Website Ease of Use. Here's are some insights:
  - Product Quality has the lowest average rating.
  - Website ease of use has the highest average rating.

- After performing analysis on the Return rate, Here are some insights:
  - Product quality Ratings is not correlated with the return rate with a negative correlation 
