# Tableau Data Analysis

## Sales and Customer Insights.

### Table of Contents

- [Project Description](#project-description)
- [Data Source](#data-source)
- [Data Cleaning and Modeling](#data-cleaning-and-modeling)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)

### Project Description
The project aims to find the sales and customer spending behavior in 2023 and 2022 and compare the spending over the years. Different KPIs and charts are made to compare the sales by subcategory and weekly trend of sales. In the customer dashboard, we have found the top 10 customers who are spending in the company and what are the average spend per customer, and other insights.

### Data Source
1. Orders Data: The primary dataset used for analysis is the "orders.csv" file which consists of all the orders placed. It acts as the Factual data table.
2. Products Data: The secondary dataset used for analysis is the "product.csv" file which contains all the products and their details available for sale. It acts as the Dimension data table.
3. Customers Data: The secondary dataset used for analysis is the "customer.csv" file which contains details about each customer. It acts as the Dimension data table.
4. Location Data: The secondary dataset used for analysis is the "location.csv" file which contains details about the location from where orders are placed. It acts as the Dimension data table.

### Tools
- Tableau Public: For data cleaning, modeling the different data tables, and visualization.

### Data Cleaning and Modeling
- In the Tableau Public, we have inserted the csv data. In the data source field, I have checked each column for checking for missing values and formatting issues. I have also checked whether the datatypes that are assigned to each column are correct. For the data modeling, I have created one-to-many relationships between the Factual table(order) and the Dimension table(products, customers, and location) so that connections are created among the different tables for analyzing the data properly.

### Exploratory Data Analysis
Performed some exploratory data analysis to find some information about key questions like
- What are the total sales and percentage change in sales in both years?
- What are the total profit and percentage change in profit in both years?
- What are the total quantity sold and percentage change in quantity sold in both years?
- What are the total sales per customer?
- Who are the top 10 customers according to money spent?

### Data Analysis
To find the answer to the key questions, I have created some calculated fields in the Tableau as
```Tableau
% diff customers = (COUNTD([CY Customer]) - COUNTD([PY Customer]))/COUNTD([PY Customer])
```

### Results/Findings
- Sales and Quantity sold are high in November but the profit earned from the sale is similar to the previous year's profit even though sales surge in November.
- The company registers the highest profit difference in March even though sales are similar to the previous year's sales.
- The company earns the highest profit by selling the Copiers and the highest loss by selling the tables.
- The phone sales have increased the most from the previous year.
- Most of the customers are ordering either 1 time or 2 time.

### Recommendations
- Sales are low from April to June so the company needs to promote their product more in these months and come up with different offers so the sales increase in these months.
- Copiers have provided the highest profit in the category so the company should focus on selling the product more.
- Phone sales have increased the most so the company should push the ad campaign and offers towards it to increase more sales of it.
- The frequency of customers placing orders is 1 or 2 times so the company should come up with different offers so that the customer can re-visit again.
   



