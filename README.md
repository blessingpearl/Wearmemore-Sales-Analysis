# Wearmemore-Sales-Analysis
## TABLE OF CONTENT
### Project Overview
### Tools And Technology

### Data Cleaning And Power BI Dashboard
### Key Insights
### Recommendations
### Future Works 
### Repository Structure

### Project Overview
Mr piper started a business of selling and distributing technology, furniture and office appliances earlier last year, and his capital was enough to produce goods and ship them locally and internationally. Business has been thriving for months now the company isn't experiencing any exponential growth but its been static. We want to analyse to demystify the reason behind the issue. 

### Tools And Technology
Power bi 

### Datasets overview
Row ID,	Order Priority,	Discount,	Unit Price,	Shipping Cost,	Customer ID	,Customer Name,	Ship Mode,	Customer Segment,	Product Category,	Product Sub-Category,	Product Container,	Product Name,	Product Base, Margin,	Country,	Region,	State or Province,	City,	Postal Code,	Order Date,	Ship Date	Profit	Quantity ordered new	Sales	Order ID

### Data Cleaning And Power BI Dashboard
Extract, transform and Load in Power BI
Changed data type
Removed unwanted columns
Created a calender table using query editor for the purpose of creating days of week and name of days before loading

Data Modeling:
Order Table - Fact Table,
User Table - dimension Table,
Return Table - dimension Table,
Calender Table - dimension Table

Dax Measure:
total sales = SUMX(Orders, Orders[Sales] * Orders[Quantity ordered new]),
total revenue = SUMX(Orders, Orders[Quantity ordered new] * Orders[Unit Price]),
total profit = SUM(Orders[Profit]),
total cost = CALCULATE([total sales] - [total profit])

Data Visualisation:
Card, clustered bar chart, pie chart, line chart and map

### Key Insights
### Recommendations
### Future Works 
