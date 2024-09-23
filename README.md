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

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Open%20Power%20BI.png)

**2. Get Data**
-	Clicked on the "Blank report" tab in the Power BI Desktop.
-	Clicked on the "Home" tab in the Power BI Desktop.
-	Selected "Get Data" to initiate the data import process

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Get%20Data.png)

**3. Choose Excel and Specify the File Location**
-	In the "Get Data" window, selected "Excel Workbook" as the data source.
-	Navigated to the location where the Excel file is stored.
-	Selected the Excel file I want to import and clicked "Open."

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Chosse%20File.png)

**4. Preview and Transform**
-	Select the tables to be inserted 
-	Power BI displayed a preview of the data from the Excel file.
-	Reviewed the data to ensure it is displayed correctly.
-	Click on transform data

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Preview%20and%20Transform%20Data.png)

## Data Profiling
Data profiling in Power BI involves examining and analyzing data characteristics to understand its structure, detect patterns, identify potential issues, and spot outliers. This process supports informed decisions regarding data cleaning and transformation. Power BI offers various tools for effective data profiling, including column quality, column distribution, and column profiling features.

**Data Profile on Key Column on Sales Table**

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Data%20Profilling%20on%20Sales%20Table.png)

**1. Basic Information**
-	Table Name: Sales Table
-	Number of Rows: 829,262
-	Number of Key Columns: Five

**2. Column Profile**

| Column Name | Data Type | Distinct Value | Unique Value | % Valid Values | % Error Value | % Empty Values | Min | Max |
|-------------|-----------|----------------|--------------|----------------|---------------|----------------|-----|-----|
| Sales ID | Whole Number |	50 | 50 |	100% | 0% |	0% | 1 | 829,262 |
| Date | Date | 1 | 0 |	100% | 0% |	0% | 1/1/2022 |	9/30/2023 |
| Store ID | Whole Number | 46 | 0 | 100% | 0% | 0% | 1 | 50 |
| Product ID | Whole Number | 24 | 0 | 100% | 0% | 0% | 1 | 35 |
| Units | Whole Number | 4 | 01 | 100% | 0% | 0% | 1 | 30 |

**3. Data Quality Checks**

**Missing Values:**
-	Sales ID: 0
-	Date: 0
-	Store ID: 0
-	Product ID: 0
-	Units: 0
-	Duplicates: This table has no duplicate value

## Data Profile on Key Column on Store Table

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Data%20Profilling%20on%20Store%20Table.png)

**1. Basic Information**
-	Table Name: Store Table
-	Number of Rows: 50
-	Number of Key Columns: Five

**2. Column Profile**

| Column Name | Data Type | Distinct Value | Unique Value | % Valid Values | % Error Value | % Empty Values | Min | Max |
|-------------|-----------|----------------|--------------|----------------|---------------|----------------|-----|-----|
| Store ID | Whole Number	| 50 | 50	| 100% | 0%	| 0% | 1 | 50 |
| Store Name | Text	| 50 | 50 | 100% | 0% | 0% | Maven Toys Aguascalientes 1 | Maven Toys Zacatecas 1 |
| Store City | Text | 29 | 17 | 100% | 0% | 0% | Aguascalientes | Zacatecas |
| Store Location | Text | 4 | 0 | 100% | 0% | 0% | Airport | Residential |
| Store Open Date | Date | 50 | 50 | 100% | 0% | 0% | 9/18/1992 | 5/18/2016 |

**3. Data Quality Checks**

**Missing Values:**
-	Store ID: 0
-	Store Name: 0
-	Store City: 0
-	Store Location: 0
-	Open Store Date: 0
-	Duplicates: This table has no duplicate value

**Data Profile on Key Column on Product Table**

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Data%20Profilling%20on%20Product%20Table.png)

**1. Basic Information**
-	Table Name: Product Table
-	Number of Rows: 35
-	Number of Key Columns: Five

**2. Column Profile**

| Column Name | Data Type | Distinct Value | Unique Value | % Valid Values | % Error Value | % Empty Values | Min | Max |
|-------------|-----------|----------------|--------------|----------------|---------------|----------------|-----|-----|
| Product ID | Whole Number | 35 | 35 | 100% | 0% | 0% | 1 | 35 |
| Product Name | Text | 35 | 35 | 100% | 0% | 0% | Action Figure | Uno Card Game |
| Product Category | Text | 5 | 0 | 100% | 0% | 0% | Art & Crafts | Toys |
| Product Cost | Decimal Number | 16 | 5 | 100% | 0% | 0% | 1.99 | 34.99 |
| Product Price | Decimal Number | 18 | 10 | 100% | 0% | 0% | 2.99 | 39.99 |

**3. Data Quality Checks**

**Missing Values:**
-	Product ID: 0
-	Product Name: 0
-	Product Category: 0
-	Product Cost: 0
-	Product Price: 0
-	Duplicates: This table has no duplicate value

**Data Profile on Key Column on Inventory Table**

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Data%20Profilling%20on%20Inventory%20Table.png)

**1. Basic Information**
-	Table Name: Inventory Table
-	Number of Rows: 1,593
-	Number of Key Columns: Three

**2. Column Profile**

| Column Name | Data Type | Distinct Value | Unique Value | % Valid Values | % Error Value | % Empty Values | Min | Max |
|-------------|-----------|----------------|--------------|----------------|---------------|----------------|-----|-----|
| Store ID | Whole Number | 32 | 0 | 100% | 0% | 0% |1 | 50 |
| Product ID | Whole Number | 35 | 0 | 100% | 0% | 0% | 1 | 35 |
| Stock On Hand | Whole Number | 84 | 19 | 100% | 0% | 0% | 0 | 139

**3. Data Quality Checks**

**Missing Values:**
-	Store ID: 0
-	Product ID: 0
-	Stock On Hand: 0
-	Duplicates: This table has no duplicate value

## Data modelling
Data modeling in Power BI involves organizing and structuring data to establish meaningful relationships between various tables. A well-designed data model is crucial for creating accurate and insightful reports.

![](https://github.com/OluwaseunOkundalaye/MEXICO-TOY-SALES-ANALYSIS/blob/main/Data%20Modelling.png)

Active relationships were established between tables using common fields (keys), and the relationships diagram was reviewed to ensure that all connections were correctly defined. In Power BI, an active relationship serves as the default link between tables, which is used for filtering and calculations. When a relationship is created between two tables, Power BI automatically assumes it to be active unless specified otherwise. Active relationships are typically used for most calculations and visualizations.

## Data Cleaning and Process
In Power BI, data cleaning is done using the Power Query Editor, a versatile tool designed to shape and transform data before loading it into the Power BI data model. This step is crucial for ensuring data integrity, quality, consistency, and accuracy.

After conducting data profiling, the dataset used for this analysis was found to be well-structured and consistent, with no significant issues that could impede analysis or interpretation. The data is in a standardized format, follows consistent naming conventions, and contains all required fields. The data values are accurate, columns are assigned appropriate data types, and there are no duplicate records. As a result, no further data cleaning was necessary.

The following procedures were carried out during the data processing phase.

**1. Created New Columns:** 

Several new columns were added to enhance the dataset and enable more detailed analysis. These new columns included:

- **Month Name:** This column represents the month name in which each sales was made in. 
In Power BI, the Month Name Column was created on sales table and gotten by creating a column that give the month name.

_DAX code for creating Month Name column_

```Month Name = FORMAT(sales[Date],"MMM")```

- **Day:** This column indicates the day of the week for each sales. 
In Power BI, the Day Column was created on sales table and gotten by creating a column that give the Day.

_DAX code for creating Day column_

```Day = FORMAT(sales[Date],"DDD")```

- **Day Number:** This column represents the weekday number in which each sales was made in. In Power BI, the Day Number Column was created on sales table and gotten by creating a column that give the day number.
  
_DAX code for creating Month Number column_

```Day Number = WEEKDAY(sales[Date].[Date])```

- **Quarter:*** This column denotes the fiscal quarter in which each sales occurred, providing insights into quarterly performance. 
In Power BI, the Quarter Column was created on sales table and gotten by creating a column that give the Quarter.

_DAX code for creating Quarter column_

```Quarter = "Q" & QUARTER(sales[Date].[Date])```

- **Year:** This column indicates the year for each sales. 
In Power BI, the Year Column was created on sales table and gotten by creating a column that give the Year.

_DAX code for creating Year column_

```Year = YEAR(sales[Date].[Date])```

- **Month Number:** This column represents the month nuber in which each sales was made in. In Power BI, the Month Number Column was created on sales table and gotten by creating a column that give the month number.
  
_DAX code for creating Month Number column_

```Month Number = MONTH(sales[Date])```

- **Profit:** This column represents the profit made from each sales of toy. In Power BI, the profit Column was created on product table and gotten by creating a column that give the profit.
  
_DAX code for creating Profit column_

```Profit = 'Product'[Product_Price] - 'Product'[Product_Cost]```

- **Out Of Stock:*** This column shows which store is out of stock. In Power BI, the profit Column was created on Inventory table and gotten by creating a column that give Out of Stock.

_DAX code for creating Out Of Stock column_

```Out Of Stock = IF(Inventory[Stock_On_Hand] = 0,1,0)```

Interpretation: If inventory(stock at hand) is equals to 0, return 1, else, return 0. I:e everywhere with 0 shows stock at hand is more than zero.

**2. Created Measure**

The following measure were created using various DAX code in order to aid our analaysis for better and more detailed result.

- **Total Profit:** This measure shows the total profit made from each sales of Toy from the toy stores. This was calculated by multiplying the profits by each quantity sold and summing up the entire figure in Power BI. 

_DAX code for calculating Total Profit_

```Total Profit = SUMX('sales','sales'[Units] * RELATED('Product'[Profit]))```

- **Total Revenue:** This measure shows the total money made from toy sales from the toys store from all the locatiions. This was calculated  by multiplying each quantity sold by product price.

_DAX code for calculating Total Revenue_

```Total Revenue = SUMX('sales','sales'[Units] * RELATED('Product'[Product_Price]))```

- **Total Quantity:** This measure shows the total number of quantity of toys sold by the stores. This was calculates by summing up the quantities sold in Power BI.

_DAX code for calculating Total Quantity_

```Total Quantity = SUM(sales[Units])```

- **Total Stock On Hand:** This measure shows the total amout of stock the stores have available. This was calculated by summing up the stock on hand in Power BI.

_DAX code for calculating Total Quantity_

```Total Stock On Hand = SUM(Inventory[Stock_On_Hand])```

