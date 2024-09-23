# MEXICO TOY SALES ANALYSIS
A Power BI project for sales &amp; inventory data for a toy stores in Mexico called Maven Toys, including information about products, stores, daily transactions, and current inventory levels at each location.

## Table of Content
- Project Overview
- Project Scope
- Business Objective
- Document Purpose
- Use Case
- Skills Demonstrated
- Data Source
- Data Connection Detail
- Data Profiling
- Data modelling
- Data Cleaning and Process
- Data Analysis and Insight
- Data Visualization
- Recommendation
- Conclusion

## Project Overview

This project aims to provide toy sales stores, a fictitious chain of toy stores in Mexico called Maven Toys, with actionable insights, derived from the analysis of sales and inventory data using Power BI. By understanding historical sales trends, product performance, which product categories drive the biggest profits, revenue, quantity and if this is the same across store locations, sales being lost with out-of-stock products at certain locations, the company can make informed decisions to optimize its business strategies, improve operational efficiency, and enhance overall performance in the gourmet food supply market.
The project will provide Maven Toys with the tools and knowledge needed for strategic planning and ongoing success.

## Project Scope

This project covers sales data from January 1, 2022 to September 30, 2023, focusing inventory levels, stores, sales trends, and products performance.

## Business Objective

The objective for this analysis is to identify which product categories drive the biggest profits, revenue, quantity and if this the same across store locations, seasonal sales trends or patterns in the sales data, sales being lost with out-of-stock products at certain locations, how much money is tied up in inventory at the toy stores.

## Document Purpose

This documentation serves as a guide for project stakeholders, providing insights into the project's objectives, data sources, data analysis, visualizations, and any other relevant information.

## Use Case

This analysis project for Maven Toy Stores offers valuable insights that can drive improvements across various operational areas. Different stakeholders within the organization can use these findings to enhance their respective functions. Below are the key stakeholders who could benefit from this analysis:

**1.	Operations Managers:**

Operations managers can utilize insights from the analysis to streamline order fulfillment processes, optimize inventory levels, and improve overall operational efficiency.

**2.	Marketing Team:**

The marketing team can apply the insights to better understand customer preferences, satisfaction levels, and overall market trends.

**3.	Customer Service and Sales Teams:**

Customer service and sales teams can leverage insights to improve communication channels, enable real-time order tracking, and gain a deeper understanding of customer preferences and issues.

## Skills Demonstrated
-	Data Connection in Power BI
-	Data Profiling
-	Data Cleaning and Transformation in Power Query
-	Data Modelling
-	Data Analysis
-	Data Visualization

## Data Source
The dataset for this project is sourced from Maven Analytics [website](https://www.mavenanalytics.io/data-playground?dataStructure=Multiple%20tables&order=date_added%2Cdesc&tags=Retail) designed specifically for practice purposes. The project utilizes a dataset containing information on sales, stores, inventory and products. The dataset used for this analysis was downloaded from Maven Analytics website where datasets are available for practice purpose. The dataset is an Excel file and it consist four main tables which are sales table, store table, product table, and inventory table.

Sales table contain information about the stores sales. It has 829,262 rows, and 5 columns which are Sale ID, Date, Store ID, Product ID, and Units. Sales ID is the unique identifier for each sales, Date is the date of the transaction, Store ID is the unique identifier for each store, Product ID is the unique identifier for each product, Units shows the number of units sold

Store table contain information about the toy stores. It has 50 rows, and five (5) columns which are Store ID, Store Name, Store City, Store Location, and Store Open Date. Store ID is the unique identifier for each store, Store Name is the name for each store, Store City is the city in Mexico where the store is located, Store Location is the location in the city where the store is located, and Store Open Date is the date where the store was opened.

Product table contain information about products. It has 35 rows, and 5 columns which are Product ID, Product Name, Product Category, Product Cost, and Product Price. Product ID is the unique identifier for each products, Product Name is the name of each product, Product Category is the category each product belong, Product Cost is the amount required to produce the product in USD and Product Price is the amount each product is sold in USD.

Inventory table contain information about stock at hand. It has 1,593 rows, and 3 column which are Store ID, Product ID, and Stock On Hand. Store ID is the unique identifier for each store, Product ID is the unique identifier for each product, and Stock On Hand is the Stock quantity of the product in the store (inventory).

## Data Connection Detail
In Power BI, connecting to an Excel file involves specifying the location of the Excel file and defining the data import settings. Here are the steps taken in data connection in Power BI.

**1. Open Power BI Desktop**

-	Launched Power BI Desktop on computer.
  
![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/commit/9d1d0bd8d61878c3efd24bb7dbdc7eb0d4e475ca)

