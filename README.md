# Capstone Sales Data 
An Analysis of Capstone Project Sales Data

## Title: SALES DATA ANALYSIS##



## PROJECT OVERVIEW.
This repository contains the Analysis of Capstone sales data, providing valuable insights into customer purchasing behaviour and market trends with keen attention to the products with the highest performance.


## DATA SOURCES
- Microsoft Excel [Download Here](https://www.microsoft.com)
  
- Incubator Hub Sales Data
  
- Capstone Project Sales Data

## Data Cleaning And Preparation
- Microsoft Excel
  
                1. Data cleaning
   
                2. For Data Analysis
    
                3. For visualization

- SQL Structured Query Language...For Querying Data

- Git Hub for Portfolio Building

- Power BI...for building visualizations based on data received.
  
## DATA ANALYSIS

Variables used are 

Products

Regions

Quantity

Revenue

Unit price 

Customer ID

Order ID

To get Total Revenue I used

```
=F2*G2
```

To get the Transaction Category

```
=IF(F2<=5,"Low",IF(F2<=10,"Medium","High"))
```
Total Quantity Sold
```
=SUM(F2:F9922)
```
Average Quantity Sold
```
=AVERAGE(F2:F9922)
```

Total Revenue Or Total Sales
```
=SUM(H2:H9922)
```
Average Revenue
```
=AVERAGE(H2:H9922)
```
Total Quantity Sold for Each Product
```
=SUMIF(C2:C9922,"productname",F2:F9922)
```
Total Revenue for each Product
```
=SUMIF(C2:C9922,"productname",H2:H9922)
```

Below are pivot tables on Excel

![sales pivot table](https://github.com/user-attachments/assets/24b2fcc0-c95d-4c5b-8af8-2c61324f7362)
![Screenshot 2024-11-08 090604 sales pivot table](https://github.com/user-attachments/assets/787cbd16-872e-496e-8557-b52e75a3bbfc)
![Screenshot 2024-11-08 091118 sales pivot table](https://github.com/user-attachments/assets/5331817d-bef3-4778-b34a-e318990c9148)
![Screenshot 2024-11-08 091033 sales Pivot table](https://github.com/user-attachments/assets/972e4fb9-25cf-4c71-bf8a-cea8fafc0290)
![Sales pivot jpg 1](https://github.com/user-attachments/assets/7969427c-dd4e-4d9e-9e0f-4075bd93516c)
![sales data 2](https://github.com/user-attachments/assets/b2711ce4-b315-415d-9b1f-0eb1660d6e18)
![sales data 3](https://github.com/user-attachments/assets/3b022364-fe18-40d1-9b10-2bf00e7185ad)
![pivot chart 1](https://github.com/user-attachments/assets/6e3c8030-5192-43b3-bfc8-267856ad3b0f)
![pivot chart 2](https://github.com/user-attachments/assets/8aa07a12-8bfc-448f-93be-1a9c733368ad)

## Analysis On SQL

These are the queries executed on SQL

To retrieve the total sales for each product category
```
select product,sum(revenue) as Total_Revenue
from[dbo].[SALES_DATA_] Group by Product
```
Number of sales transaction in each Region
```
Select Region,sum(Revenue) as Total_Sales
from  [dbo].[SALES_DATA_] Group by Region
```
Highest selling product by total sales value
```
Select Product, sum(Quantity) as Total_sales_or_Total_Quantity_Sold
from [dbo].[SALES_DATA_] Group by Product
Order by Total_sales_or_Total_Quantity_Sold Desc
```
Total revenue per product
```
Select Product,sum(Revenue) as Total_Revenue_per_Product
from [dbo].[SALES_DATA_]
Group by Product 
```
Total revenue per Region
```
Select Region,sum(Revenue) as Total_Revenue_per_Region
from [dbo].[SALES_DATA_]
Group by Region
```




## Analysis on Power BI

Cleaned data from Excel was imported to power BI. and here are some visuals

![Power BI sale data 2](https://github.com/user-attachments/assets/ad757a66-b3ab-4e48-89cf-2ec8e344d051)

![sales data visual 1](https://github.com/user-attachments/assets/ffe03452-8013-44b8-b807-f9c1a41331da)



















## KEY FINDINGS/ INFERENCE:


..Trend Analysis: Sales have consistently increased 

...Product Performance: Top selling product is HAT 

## RECOMENDATION

The company has to improve on making their presence felt in the market place by having constant promotions and advertisment of the products that has low demands in each regions. 
