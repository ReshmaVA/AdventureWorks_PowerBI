# AdventureWorks

A Microsoft Power BI business intelligence dashboard for AdventureWorks, a fictional global manufacturing company that produces cycling equipment and accessories.

This data was derived from the [AdventureWorks sample databases](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure) available from Microsoft.

The customer base is spread across 6 countries on 3 continents: Australia, Canada, France, Germany, United Kingdom and United States. Sales and return data is available for the period between 01/01/2020 and 30/06/2022. Customer profiles include date of birth, annual income, education level, number of children, occupation and homeowner status. 

<img alt="AdventureWorks Executive Dashboard" src="./AdventureWorks Images/Screenshots/exec_dashboard.jpeg">

## Features

- Track key performance indicators (KPIs) related to sales, revenue, profit, and returns.
- Compare performance across different regions.
- Analyse product-level trends.
- Identify high-value customers.

## Project Highlights

This project involved the following tasks:

- connecting and transforming the raw data 
- building a relational data model
- creating calculated columns and measures using **DAX**
- Created a rolling calendar using **PowerQuery M code**
- building an interactive dashboard

## Dashboard Elements

#### Executive Summary View

- high-level KPIs for revenue, profit, orders and return rates
- page-level filtering by product and product category
- drill-through per product to product detail view

#### Map View

- total orders per country

#### Product Detail View

- per-product performance against order, revenue and profit targets
- "what if" analysis via price adjustment shows adjusted profit

#### Customer Detail View

- total customer and per-customer revenue analysis

#### Custom UI Elements

- filter pane for filtering by year and geography
- bookmarks to refresh page, hide and show filter pane and capture customer insight.
- Page navigation to navigate to different report pages.
- custom tooltip for product category order metrics
- Q & A report page to get the line chart for total orders by start of month
- Decomposition Tree report page to analyze which product has most orders
- Key Influencers to analyze data catgorically and continuously
- calculation groups to group the common measures together such as Time Intelligence measures.
- New Card Visual to get total revenue, total orders, total profit and return rate with additional details such as their previous month data and integrated with other custom visuals.
- Button and List slicers to check functionality.
- Visual calculations to perform DAX calculations within the visual to get running total, moving average, etc.
- DAX info.view function is used to create tables for measures, columns, relationships and tables in the report to document the information provided within them.
- Using DAX to create Data Dictionary table to integrate all the above tables into one and extract data into table visual based on slicer pane in Data Dictionary report page.


### Insights

- Approximately $24.9 million in revenue and $10.5 million in profit was generated between 01/01/2020 and 30/06/2022. There is an appreciable dip in revenue between 01/06/2020 and 01/11/2020 (possibly due to the simulated impact of the COVID-19 pandemic), after which revenue appears to grow linearly. December 2021 was an exceptional year in terms of revenue at $1.64 million, and it would be worth investigated the cause of this. Was this due to a highly successful seasonal campaign, e.g. a Black Friday promotion?

- Understandably, tires and tubes are the most ordered product type, while cycling shorts are the most returned product type. After Fender Set - Mountain, Mountain-100 Silver,44 top the list of revenue-generating products, despite having relatively high return rates:

<img src="./AdventureWorks Images/Screenshots/top_revenue_products.jpeg">

- The most revenue driving product category is bikes.

- There is a step change (on the order of 200 customers per week) in total weekly customers beginning 02/08/2021.

<img src="./AdventureWorks Images/Screenshots/total_weekly_customers.jpeg">

- However, revenue per customer has been declining year-on-year:

<img src="./AdventureWorks Images/Screenshots/revenue_per_customer.jpeg">

- While the United States is the largest market with 8,700 orders and $7.94 million in total revenue, The Australian market has the largest revenue per customer at $2,131.

- In January 2021, Mr. Larry Munoz was the High income Professional who made the most revenue of $10,852.

<img src="./AdventureWorks Images/Screenshots/Most_revenue_driving_highincomecustomer.jpeg">
