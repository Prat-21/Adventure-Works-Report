![AdventureWorks_Logo](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/68b7dc07-0956-4639-a522-753a4935799b)

# Adventures Works Data Analysis
I had the opportunity to complete a project with Adventure Works Data set.
I worked as a Business Intelligence Analyst for Adventures Works, a fictitious global manufacturing company that produces cycling equipment and accessories.
The management team needed a way to track KPIs (sales, revenue, profit, returns), compare regional performance, analyze product-level trends and identify high-value customers.
I analyzed their sales and returns data using Microsoft Power BI Desktop.
I used power bi desktop to-

                           1.Connect and transform the raw data.
                           2.Build a relational data model.
                           3.Create calculated columns & measures with DAX.
                           4.Design an interactive dashboard to visualize the data.
                          

This was an end to end project beginning with importing and data cleaning and ending with the creation of visuals and optimization of those visuals.

## Data Cleaning

The raw data set came in .csv format and was imported to Power BI directly. A total of 8 files were imported, each being their own table. Here, I was able to get a general overview of the data set and saw that I would primarily be working with Sales and Returns data. I then began cleaning the data by ensuring that columns were titled appropriately and they were in their correct data types, looking for missing data (which there was none) and began looking for what relationships I might be able to create between these tables.

## Data Modeling

After ensuring my data’s accuracy and consistency, I began the process of creating a data model for my tables. I first established my data tables which are ‘Sales Data’ and ‘Returns Data’, then, began work by creating relationships between tables. For this project I did not find it necessary to use any relationships other than one to many. A picture of the completed model is provided below for greater understanding.



![Screenshot (1)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/a5032d5d-fc94-4091-9727-6810353fd9b9)



## DAX Functions

Now that I had established my table relationships, I could begin utilizing some DAX functions to analyze the data set. I started by creating basic KPI’s such as Revenue, Profit, and Total Orders which would help me to calculate more advanced metrics later on. Some of the DAX functions I used the most include:

  **ITERATOR** **FUNCTIONS** **(**SUMX**)**: These are formulas which evaluate an expression based on each row and then aggregate the results.

  **CALCULATE**(): It acts as an overriding filter to give you a new filter context. It was incredibly useful for establishing Previous Months Orders, Revenue, Profit, Returns and Overall Average Price.

  **RELATED**(): This function allows you to pull data from different tables as long as there is an established many to one relationship.

  **Date** **Functions**(**DATEADD**, **DATESINPERIOD**): These date functions were very helpful when establishing a 90 Day Rolling Profit as well as the Previous Months Order, Profit, Revenue and Returns.

The measures which were created for this project were placed into their own specific Measure Table.

## Data Visualization

A total of 6 visualization pages were created for this report. These include:


**1**.**Executive Dashboard**: It includes company wide KPIs, Trending Revenue, most ordered products, monthly returned products and several other important details.


![Screenshot (2)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/d2d27fac-d41e-4984-9582-a6ef7b7e5a1e)



This dashboard is meant to be a general overview of company performance for anyone to understand.

A slicer Panel located in the top left is also available to further filter down visuals based on the year and continent providing a more granular look at the most important KPI’s.



![Screenshot (3)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/27495ef3-c229-4a4b-8c39-d3fe6b2786d6)



**2**.**Map**: This is an interactive visual of the company’s order distribution throughout the world broken down by continent.



![Screenshot (4)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/b6765275-c929-4b66-93b2-a186da8b0ef9)



Some key insights found from this page were that while the United States makes up the majority of Adventure Work’s Orders (8,700), the Pacific also shares a significant share of the total orders as well (6,060).

Germany had least orders with 2294.

Additionally, no sales have taken place in Asia, Africa, or South America indicating a potential for new markets to break into.

**3**.**Product detail**: This page provided an in-depth and interactive look at the relationship between the products of Adventure Works and their respective revenue, orders, profit, returns and return rate.

For the selected product I have chosen “Water Bottle - 30 oz.”. Here we can see this item is not meeting the any of the monthly targets for Orders, Revenue or Profit.

Additionally, we can see in the bottom area chart that the reason for this is likely due to a sharp increase in returns for this product which may indicate a potential defect with the product.



![Screenshot (8)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/ba3a5cde-4e85-4464-a1de-47c8dfd60841)




**4**.**Customer Detail**:  Multiple visuals of the relationship between customers and business metrics can be found on this page.




![Screenshot (9)](https://github.com/Prat-21/Adventure-Works-Report/assets/165648053/a11b881e-cf00-42f5-93c8-939b31d3e4d3)



On this page I was able to break our customers down by occupation and income level as represented in the Donut Charts in the bottom left.

A steep increase in total customers can be seen in July 2021 which can possibly explained by it being the summer months with biking being more popular.

The Top 100 Customers Table has several interesting factors. In addition to providing an overview of the Top 100 customers, it also provides their total orders and it was here that some interesting insights were found.
Take for example, the top customer displayed in the bottom right corner or first row of the table. Mr. Shan was able to secure the top position in terms of Revenue with only 6 total orders. In fact, the top 5 customers all created Revenue greater than 11,000$ and all did this with 7 or less orders.

To contrast this, Mr. Fernando Barnes ordered a total of 26 products and only brought in 1,839$ dollars. This demonstrates the wide range in cost of the products sold by Adventure Works.



