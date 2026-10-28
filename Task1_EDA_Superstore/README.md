# Task 1: Exploratory Data Analysis on Superstore Retail Sales

Datheon Data Analytics & Power BI Internship

**Author:** Promise Jeneka Taiwo

## What this project is about
I cleaned the Superstore sales data and explored it to see how customers buy, how sales change through the year, which categories make money, and how discounts affect profit.

## Files
- `Task1_Superstore_EDA.ipynb`: the full notebook with code, charts and written findings
- `superstore_sales.csv`: the dataset used

## Tools
Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

## Data cleaning
- The CSV had about 800 extra rows at the bottom. They were the Superstore "People" and "Returns" tables pasted under the sales data. I used the returns part for a returns check and removed the rest.
- 11 rows had no postal code (all Burlington, Vermont), so I filled them with the city's ZIP code.
- Converted the date columns and fixed the data types.
- Removed 1 duplicate row.
- The clean data has 9,993 rows covering January 2015 to December 2018.

## Main findings
1. The top 10% of customers bring in 30.6% of sales, but 155 of 793 customers have negative profit.
2. September, November and December make up 42.9% of sales. Sales grew 29.5% in 2017 and 20.4% in 2018.
3. Furniture has only a 2.5% margin. Tables, Bookcases and Supplies lose money.
4. Discounts above 20% push the margin negative, and every order line above 40% discount lost money.
5. The Central region has the heaviest discounting (24% average) and the lowest margin (7.9%).

Total sales were about $2.30M and total profit about $286K, an overall margin of 12.5%.
