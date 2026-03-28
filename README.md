# Black Friday Sales Analysis for Walmart (Industry : Retail)
This project explores Walmart’s Black Friday transaction data to analyze how customer spending patterns vary across different demographics — focusing on gender, age group, marital status, and city category.

# Project Overview
This project examines Walmart’s Black Friday transaction data to uncover how spending behavior varies across gender, age group, marital status, and city category. It aims to answer key questions such as: Do women spend more than men? Which age groups are the biggest spenders? The insights derived can help Walmart refine its marketing and sales strategies for better customer targeting.

# Problem Statement
Walmart seeks to analyze customer purchase behavior during Black Friday sales to determine how spending habits vary across gender, marital status, age group, and city categories. The objective is to leverage these insights to enhance marketing strategies and optimize inventory planning.

# Objectives
 - Explore and clean the dataset to address basic data quality issues.
 - Analyze and compare average spending across different groups — gender, marital status, and age.
 - Apply the Central Limit Theorem (CLT) and confidence intervals to estimate population means and measure uncertainty.
 - Provide clear, actionable recommendations to help Walmart improve marketing and inventory decisions.

# Data Set
 - User_ID:	User ID
 - Product_ID:	Product ID
 - Gender:	Sex of User
 - Age:	Age in bins
 - Occupation:	Occupation(Masked)
 - City_Category:	Category of the City (A,B,C)
 - StayInCurrentCityYears:	Number of years stay in current city
 - Marital_Status:	Marital Status
 - ProductCategory:	Product Category (Masked)
 - Purchase:	Purchase Amount

# Milestones
 - Load and inspect the dataset
 - Check data quality — identify missing values and outliers
 - Analyze group-wise spending - sum, mean, median
 - Estimating Confidence Intervals - Finding the overlaps
 - Exploring the strength and direction of the relationship among the attributes using Correlation in Heatmap
 - Use CLT to draw assumptions on sample distributions
 - Findings and inferences
 - Recommendations

# Findings
  - As per CLT, the Smaple Ditribution follows Gaussian regardless of the population as the sample size for both the samples are much bigger than 30
  - We have outliers in Purchase Data
  - Count of purchase by male (Count : 414259) is much higher than count of purchases made by female (Count : 135809) i.e. 75.31% are transactions are made by male and 24.69% transactions made by female
  - Total purchases by male (Total : USD 3909580100) is much higher than total purchase made by female (USD 1186232642). Similar ratio as transaction count, persists from Total Purchase perspective
  - Mean Purchase amount for Male is 9437.53 and for Female it's 8734.57. Mean is impacted by Outliers.
  - Median pruchase amount for male is 8098 and for female it's 7914. Here the differnce in purchase amount shrinks as Males have more / higher value outliers than Female buyers.
  - Males have higher Total, Mean and Meadian purchases with respect to Females and it's statistically proven through Hypothesis Testing
  - Based on Confidence Interval study, we can conclude, The confidence intervals of average male and female spendings are not overlapping. That means, there is a statistically significant difference between the average spending of male and female customers — and specifically, males spend more on average than females
  - Regardless of Marital_Status, Mean and Median purchase amount per transaction for Male is higher than that of female
  - Regardless of City_Category, Mean and Median purchase amount per transaction for Male is higher than that of female
  - Only Product_Category has a moderate negative correlation (-0.34) with Purchase amount
  - There is no significant evidence to conclude mean purchase by married and unmarried buyers are different.
  - At least one age group has a significantly different Mean Purchase

# Recommendations
 - Target Male Customers with Premium or High-Value Product (Product Category) Offerings as male buyers have spent highest from total, mean and median stand point
 - Develop Strategies to Increase Female Buyer Engagement like targeted discounts etc.
 - Promote Product categories with higher product price
 - Promote the higher priced products in each product category
 - Demographic based personalization to done for sales promotions
    - Gender : As gender has stronger relationship with purchase amount than any other parameter
    - Age : At least one group has significantly different mean purchase
    - City_Category : Personalized sales promotion for City_Categories
 - Explore and target high-spending male subsegment as males have more and high value outliers

# Colab Link 
 - https://colab.research.google.com/drive/1NcKgZSNa0ysY_3XdhR-XhSX5930WcyIW

# Data Link
 - https://drive.google.com/file/d/1YTDX1lRpG-IjG4YAwl5L1SRkxJbuIaCh/view?usp=drive_link
