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

