# Quantium Customer Purchasing and Spending Behaviour.
*![Quantium](https://github.com/Ugondu/ExploratoryDataAnalysisforQuantium/assets/113315492/2268dc51-73a6-4996-a3d4-eac3f2e637ff)*
## Table of Contents.
- [Business Problem Overview](#business-problem-overview)
- [Project Objective](#project-objective)
- [Data Sources](#data-sources)
- [Data Processing](#data-processing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Insights and Findings](#insights-and-findings)
- [Conclusion and Recommendation](#conclusion-and-recommendation)
## Business Problem Overview.
The Category Manager for Chips, a company specialized in the sales of chips wishes to understand the category of customers that patronize the business. The manager intends to understand their purchasing and spending behavior to enable the company to target specialized promotions to these group of customers. The insights will aid the company strategy in the next half of the year.
## Project Objective.
The aim of this project is to perform exploratory data analysis on the available datasets to generate actionable insights and recommendations.
1.	Examine both transaction and customer datasets for inconsistencies, missing values, outliers, correctly identify categorical and numerical data.
2.	Define metrics such as total sales, drivers of sales, and where the highest sales are coming from.
3.	Explore the data, create charts and graphs to visualise trends and insights for business recommendations.
4.	Define the customer segments that the company should be targeting via visualisations.
## Data Sources.
The available datasets were **customer** **https://cdn.theforage.com/vinternships/companyassets/32A6DqtsbF7LbKdcq/QVI_purchase_behaviour.csv** and **transaction** **https://cdn.theforage.com/vinternships/companyassets/32A6DqtsbF7LbKdcq/QVI_transaction_data.xlsx** data over a period of time.
### Customer data features:
* LYLTY_CARD_NBR: Unique identifier given to each customer signed up to the company.
* LIFESTAGE: This feature explains whether a customer has family or not.
* PREMIUM_CUSTOMER: Category of customers that patronize the business.
### Transaction data features:
* Date: The date customer made the transaction.
* STORE_NBR: The location of the store where the customer made the transaction.
* LYLTY_CARD_NBR: Unique identifier given to each customer signed up to the company.
* TXN_ID: The unique identifier for each transaction by the customer.
* PROD_NBR: The unique identifier for each product.
* PROD_NAME: The name of each product on the company’s catalogue.
* PROD_QTY: Quantity of product sold.
* TOT_SALES: Total sales of each product.
## Data Processing.
* Dataset Merge: The customer and transaction datasets were merged on “LYLTY_CARD_NBR” column as it provides commonality for joining the datasets.
* Data type conversion: The “LYLTY_CARD_NBR” column served as the primary key, hence is converted to data type object to enhance our analysis.
* Feature Engineering: A new column “WEIGHT(G)” is created from “PROD_NAME” to able to demonstrate the weight of each product in the catalogue. 
* Missing Values: We filled the missing values with the median value for each column.
* Duplicates: Duplicates values were dropped from the merged dataset.
## Exploratory Data Analysis.
* Univariate Data Analysis: The dataset was examined for the distribution of each customer lifestage, distribution of customer segmentation, and the percentage of each customer segment. Having managed the outliers in the data processing phase, boxplots of total sales and product weights were visualized to ensure the absence of outliers in the dataset.
* Bivariate Data Analysis: We examined the relationship between total sales and variables such as customer lifestage, customer segment, top ten customers, and top three products by total sales. We further evaluated if there is a relationship between weight of product and total sales using a scatter plot. 
## Insights and Findings.
* Older singles/couples should be targeted to ensure they keep patronising the store
* Premium clients should be incentivised to buy more
* Promotions should be targeted towards the mainstream customers to keep them in the company’s books
* Kettle Tortilla chips remain the most sort after product, hence, should always be in stock.
* Business is in safe hands as the difference between the top ten clients purchasing power is relatively narrow.
## Conclusion and Recommendations
This project showcases the effectiveness of exploratory data analysis in providing useful insights in dataset that involves customer spending and purchasing behaviours. We are able to demonstrate the importance of customer segmentation and how to effectively channel the company’s campaign strategies. 
