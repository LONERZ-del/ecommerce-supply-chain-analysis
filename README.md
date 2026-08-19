# E-Commerce Supply Chain Analysis

## Project Objective

To analyze e-commerce supply chain data and identify patterns in sales, order status, shipping performance, product categories, markets, and regions. The project uses Python, SQL, and Power BI to transform raw data into meaningful insights that can support better business and supply chain decisions.

## Problem Statement

E-commerce businesses generate large amounts of data related to orders, sales, products, customers, markets, and shipping. Without proper analysis, it is difficult to identify sales patterns, understand product performance, and evaluate delivery and shipping efficiency.

This project analyzes the available supply chain data using Python, SQL, and Power BI to identify important patterns and provide clear business insights.

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQL
* Power BI

## Dataset

The project uses the **DataCo Supply Chain dataset**, which contains information related to orders, customers, products, sales, shipping, markets, regions, and order status.

The dataset contains approximately **180,000 records** and multiple attributes related to e-commerce supply chain operations.

## Project Workflow

1. Data Collection
2. Data Inspection
3. Data Cleaning and Preprocessing
4. Feature Engineering
5. Exploratory Data Analysis
6. SQL Analysis
7. Data Visualization using Power BI
8. Business Insights
9. Documentation

## Data Inspection

The dataset was first inspected to understand its structure and quality.

The following checks were performed:

* Number of rows and columns
* Column names
* Data types
* Missing values
* Duplicate records
* Unique values
* Descriptive statistics

The dataset contained approximately **180,519 records and 53 columns** before cleaning.

## Data Cleaning and Preprocessing

The following cleaning steps were performed:

* Checked missing values in all columns.
* Checked for duplicate rows.
* Verified that there were no complete duplicate rows.
* Filled missing customer last names with `"Unknown"`.
* Filled missing customer zipcodes using the mode.
* Removed `Order Zipcode` because a very large proportion of its values were missing.
* Removed `Customer Email` because it was not required for the analysis.
* Removed `Customer Password` because it was not required for the analysis.
* Converted order date and shipping date columns into datetime format.

## Feature Engineering

New columns were created to support the analysis.

### Order Year

The year was extracted from the order date to support yearly analysis.

### Order Month

The month was extracted from the order date to support monthly analysis.

### Shipping Days

Shipping duration was calculated by subtracting the order date from the shipping date.

### Shipping Status

Orders were classified into two groups:

* On Time
* Delayed

For this analysis, orders with shipping time of more than 3 days were classified as delayed.

## Exploratory Data Analysis

Python was used to perform exploratory analysis and create visualizations.

### Order Status Distribution

A count plot was used to understand the distribution of different order status categories.

### Shipping Status Distribution

The shipping status was analyzed to compare on-time and delayed shipments.

The analysis showed:

* **On Time:** 95,120 orders
* **Delayed:** 85,399 orders

This corresponds to approximately:

* **On Time:** 52.69%
* **Delayed:** 47.31%

### Sales Distribution

A histogram was created to understand the distribution of sales values.

The sales distribution showed that most observations were concentrated at lower sales values, with some much larger values.

### Sales Outlier Analysis

A box plot was created to identify the spread and possible outliers in the Sales column.

The visualization showed several higher-value sales observations outside the main distribution.

### Sales and Order Quantity Analysis

A scatter plot was created to examine the relationship between Order Item Quantity and Sales.

The correlation between the two variables was approximately:

**0.106**

This indicates a **weak positive relationship** between order quantity and sales in this dataset.

### Category Sales Analysis

The data was grouped by Category Name and total sales were calculated for each category.

The category totals were sorted in descending order and the top 10 categories were identified.

A bar chart was then created to visualize the highest-selling categories.

## SQL Analysis

SQL was used to analyze the cleaned supply chain data and answer business-related questions.

The SQL stage focused on areas such as:

* Sales analysis
* Order analysis
* Product and category analysis
* Customer-related analysis
* Regional analysis
* Shipping analysis
* Aggregation and grouping
* Filtering and comparison of business data

The SQL analysis helped convert the cleaned data into structured business information that could be used for reporting and decision-making.

## Power BI Visualization

Power BI was used for the visualization and dashboard stage of the project.

The analyzed data was used to create interactive dashboards and visualizations covering:

* Sales KPIs
* Sales by Market
* Sales by Category
* Sales over Time
* Sales by Region
* Delivery Status
* Shipping Mode
* Order Status
* Profit Ratio by Category
* Shipping Days by Shipping Mode
* Product Sales
* Sales and Profit Ratio
* Average Shipping Days by Region

Filters and slicers were also added to allow users to explore the data interactively.

## Business Insights

The project provides insights into:

* Overall sales performance
* Product category performance
* Sales performance across markets and regions
* Order status distribution
* Shipping performance
* Delayed versus on-time orders
* Shipping performance by shipping mode
* Product-level sales performance
* Profitability across categories
* Relationship between order quantity and sales

## Conclusion

This project demonstrates an end-to-end data analysis workflow using Python, SQL, and Power BI.

Python was used for data inspection, cleaning, preprocessing, feature engineering, exploratory data analysis, and visualization.

SQL was used to analyze the cleaned data and answer business-related questions.

Power BI was used to present the results through interactive dashboards and visualizations.

The project demonstrates how raw e-commerce supply chain data can be transformed into meaningful business information for understanding sales, products, orders, regions, and shipping performance.

## Skills Demonstrated

* Data Cleaning
* Data Preprocessing
* Feature Engineering
* Exploratory Data Analysis
* Data Visualization
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQL
* Power BI
* Business Analysis
* Dashboard Development


