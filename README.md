# Bike-Store-Management-System-using-SQL

![image](https://static.vecteezy.com/system/resources/previews/023/783/419/original/bicycle-shop-logo-design-image-bicycle-logo-concept-icon-simple-design-modern-free-vector.jpg)

# Overview

The Bike Store Management System is a comprehensive database management project designed to oversee various operations within a bike store. This project involves creating a robust database schema, normalizing data to eliminate redundancy and anomalies, cleaning the data for consistency, and running SQL queries to extract and analyze valuable information. The primary goal is to facilitate efficient management and analysis of data related to bike stores, including products, customers, orders, and staff.

# Dataset Description

The dataset used in this project is derived from the SQL Server Sample Database provided by SQL Server Tutorial. This sample database, named BikeStores, includes essential data for managing a bike store's inventory, sales, and staff. The dataset can be accessed and downloaded from the following link:

# SQL Server Sample Database - BikeStores

The dataset comprises two schemas: sales and production, which include the following tables:

* sales.stores: Information about each store.
* sales.staffs: Information about staff members.
* sales.customers: Customer details.
* sales.orders: Sales order headers.
* sales.order_items: Line items of sales orders.
* production.categories: Bike categories.
* production.brands: Bike brand information.
* production.products: Product details.
* production.stocks: Inventory information for products in stores.

# Data Cleaning

Data cleaning is a crucial step to ensure the dataset is accurate, consistent, and free from errors. In this project, data cleaning involved several tasks:

* Modifying Column Data Types: Ensuring columns have appropriate data types.
* Renaming Columns: Renaming columns for clarity and consistency.
* Handling Missing Data: Replacing missing values with defaults and deleting rows with missing critical values.
* Dealing with Outliers: Identifying and handling outliers to maintain data integrity.
  
Data cleaning is essential to avoid errors in data analysis, ensure data integrity, and provide accurate insights.

# Entity-Relation Diagram (ERD)

The ERD visually represents the relationships between different entities in the BikeStores database. Here are the main relationships:

* Customers to Orders: One-to-many relationship (a customer can place multiple orders).
* Orders to Order_Items: One-to-many relationship (an order can have multiple items).
* Order_Items to Products: Many-to-one relationship (an order item refers to a single product).
* Staffs to Stores: Many-to-one relationship (multiple staff members can work at one store).
* Products to Categories and Brands: Many-to-one relationship (each product belongs to a category and a brand).

# Data Normalization

Normalization is the process of organizing data to minimize redundancy and improve data integrity. The tables were normalized into the following structure:

* Customers Table: Holds customer contact and address information.
* Orders Table: Contains order details and statuses.
* Order_Items Table: Contains line items for each order.
* Staffs Table: Stores information about staff members and their managers.
* Stores Table: Contains store details.
* Categories Table: Stores bike categories.
* Products Table: Holds product details including brand and category.
* Brands Table: Contains brand information.

# Queries 

* Retrieve All Bike Categories: Lists all available bike categories from the categories table.
* Retrieve Unique Product Names: Identifies distinct product names in the inventory, ensuring no duplicates.
* Count Customers by State: Analyzes customer distribution by counting the number of customers in each state.
* Calculate Average Discount: Determines the average discount given on all orders, providing insight into pricing strategies.
* Total Items Ordered: Calculates the total quantity of items sold, reflecting overall sales volume.
* Products with Low Discounts: Finds products with discounts of 20% or less, helping to identify less-discounted items.
* Average Sale Price of High-Value Items: Computes the average sale price for items listed at $1000 or more, post-discount.
* Customers in Specific States: Filters customers based in California and New York to analyze regional customer data.
* Products Starting with 'T': Searches for products whose names begin with the letter 'T', using pattern matching.
* Orders Handled by Staff: Counts the number of orders each staff member has processed, ranked by the number of orders.
* Top Selling Products: Identifies the most sold products and calculates their total sales value.
* Product Sales Details: Retrieves product details, including the total quantity sold and list price, sorted by quantity sold.

# Visualizations 

* Line Plot of Orders Over Time: Shows the 30-day moving average of orders for each store, distinguishing trends by color.
  
* Customer Characteristics Subplots: Uses count plots to visualize customer purchase frequency, recency, and buying power, with a shared y-axis for comparison.
  
* Bar Plot of Average Units Sold by Category: Illustrates the average units sold per month, broken down by product category, with error bars for precision.
  
These visualizations help in understanding sales trends, customer behavior, and product performance, offering actionable insights for store management.

# Conclusion

The Bike Store Management System project showcases the effective use of a relational database to manage and analyze data for a bike store. Through data cleaning, normalization, and SQL querying, the project ensures data integrity and provides valuable insights into the store's operations. The complete project, including SQL scripts and documentation, can be found in the GitHub repository, offering a comprehensive resource for understanding and managing the BikeStores database.
