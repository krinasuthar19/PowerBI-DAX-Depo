DAX Depo 
Project Overview

This project demonstrates the use of DAX (Data Analysis Expressions) in Power BI to perform analytical calculations on sales and returns data. The focus is on backend calculations and data modeling, with results presented using Matrix visual only.

Objective

Create calculated columns and measures using DAX

Perform sales, profit, and return analysis

Apply time intelligence functions (YTD, YoY, MoM)

Organize all measures using a dedicated Measure Table

Follow the requirement of using only Matrix visual

Dataset Used
Fact Tables

Sales_Fact

Returns_Fact

Dimension Tables

Customer_Dim

Product_Dim

Date_Dim

Region_Dim

Data Model

Star schema is used

Sales_Fact is connected to all dimension tables

Returns_Fact is connected to Sales_Fact using SalesID

Date_Dim is marked as the Date Table

Calculated Columns
Profit (Sales_Fact)

Profit = SalesAmount − Cost

ReturnFlag (Sales_Fact)

Indicates whether a sale was Returned or Not Returned

Customer Full Name (Customer_Dim)

First Name and Last Name combined and converted to uppercase

Measure Table

A separate table named Measures is created to store all DAX measures in one place for better organization and maintainability.

Key Measures Created

Total Sales

Total Cost

Total Profit

Total Quantity

Average Sale per Transaction

Total Returns

Return Rate (%)

Advanced Measures
Time Intelligence

Sales Last Year (LY)

Year-over-Year (YoY) Growth

Month-over-Month (MoM) Growth

Running Total Sales

Year-to-Date (YTD) Sales

Filter Context

Sales with all regions (ignores filters)

Sales with applied filters

Other Logic

Sales Category (Low / Medium / High)

Profit calculated using SUMX

DAX Functions Used

SUM, AVERAGE, COUNTROWS

CALCULATE, FILTER, ALL

SUMX

IF, SWITCH

TOTALYTD, SAMEPERIODLASTYEAR, PREVIOUSMONTH

Visual Used

Only Matrix visual is used

No charts or other visuals are included

Data is grouped by Region, Date, Product, and Customer

Tools Used

Power BI Desktop

DAX (Data Analysis Expressions)
