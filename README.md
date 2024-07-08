ShopNow Database Management System
This project consists of a MySQL database for an e-commerce platform named "ShopNow" and a Python interface for interacting with the database. The Python script allows users to perform various operations such as viewing customers, managing orders, updating products, and more.

Getting Started
Prerequisites
Before running the Python script, ensure you have the following software installed:

Python 3.x
MySQL
mysql-connector-python
Installing Dependencies
To install the necessary Python dependencies, run:

sh
Copy code
pip install mysql-connector-python
Setting Up the Database
Create the Database: Use the provided SQL file to set up the database.
sql
Copy code
CREATE DATABASE shopnow;
USE shopnow;

-- Create tables and insert initial data
-- Include your provided SQL statements here
Load Data into the Database: Execute the SQL script to create the necessary tables and populate them with initial data.
Running the Python Interface
Configure Database Connection: Ensure the database connection parameters in the Python script match your local MySQL configuration.
python
Copy code
mydb = mysql.connector.connect(
    host="localhost",
    user="root",
    passwd="your_password",
    database="shopnow"
)
Run the Script: Execute the Python script to start interacting with the database.
sh
Copy code
python shopnow_interface.py
Python Script Functions
The Python script provides a menu-based interface for performing various operations on the "ShopNow" database. Below are the available options:

View Customers from a Specific State: Display all customers from a specified state.
View Orders Made by a Specific Customer: Display all orders made by a specified customer.
Update Products in a Specific Category: Update the category ID of products within a specific category.
View Customers Who Made Orders and Payments: Display customers who have made orders and payments along with their total payment amount.
Delete Categories and Their Respective Products: Delete a category and all its products from the database.
View Total Revenue Generated: Display the total revenue generated from all payments.
View Products in a Customer's Wishlist: Display all products in a specified customer's wishlist.
View Top 5 Customers by Amount Spent: Display the top 5 customers based on the total amount spent.
View Orders Placed Within a Specific Date Range: Display orders placed within a specified date range.
Update the Quantity of a Product: Update the quantity of a specified product.
Add Product into Cart: Add a specified product to a customer's cart.
Add a New Customer: Add a new customer to the database.
Exit: Exit the program.
