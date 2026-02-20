# Online_book_store

📚 Online Bookstore SQL Project
📌 Project Overview

This project is a SQL-based relational database analysis for an Online Bookstore system.

The objective of this project is to:

Design a structured relational database

Import CSV data into PostgreSQL

Perform business-focused SQL queries

Extract meaningful insights from transactional data

This project demonstrates practical usage of PostgreSQL, Joins, Aggregations, Filtering, and Business Analysis Queries.

🗂 Database Schema

The project consists of three main tables:

1️⃣ Books

Stores book-related information.

Book_ID (Primary Key)

Title

Author

Genre

Published_Year

Price

Stock

2️⃣ Customers

Stores customer details.

Customer_ID (Primary Key)

Name

Email

Phone

City

Country

3️⃣ Orders

Stores order transactions.

Order_ID (Primary Key)

Customer_ID (Foreign Key)

Book_ID (Foreign Key)

Order_Date

Quantity

Total_Amount

🔗 Database Relationships

One Customer → Multiple Orders

One Book → Multiple Orders

Orders table acts as a bridge between Customers and Books

📥 Data Import

Data was imported using PostgreSQL COPY command from CSV files:

Books.csv

Customers.csv

Orders.csv

🧠 Basic SQL Analysis Performed

✔ Retrieve books by genre
✔ Filter books by published year
✔ Identify customers by country
✔ Retrieve orders by date range
✔ Calculate total stock available
✔ Find most expensive book
✔ Identify low-stock books
✔ Calculate total revenue

🚀 Advanced Business Queries
📊 1. Total Books Sold Per Genre

Used JOIN + GROUP BY to identify which genre performs best.

📊 2. Average Price of Fantasy Books

Used AVG() function to analyze pricing trends.

📊 3. Customers with Multiple Orders

Used GROUP BY + HAVING to identify repeat customers.

📊 4. Most Frequently Ordered Book

Identified highest demand book using COUNT() and ORDER BY.

📊 5. Total Quantity Sold by Each Author

Business insight into author performance.

📊 6. Highest Spending Customer

Used SUM() with GROUP BY to find top revenue-generating customer.

📊 7. Stock Remaining After Orders

Calculated real-time inventory using:

LEFT JOIN

COALESCE()

Aggregation logic

📈 Key Business Insights

Certain genres generate higher total sales compared to others.

A small number of books contribute to majority of orders.

Repeat customers significantly impact total revenue.

Inventory tracking helps identify low-stock or high-demand books.

Revenue analysis helps identify top-performing customers.

🛠 Skills Demonstrated

PostgreSQL

Database Design

Primary & Foreign Keys

JOIN operations

GROUP BY & HAVING

Aggregate Functions (SUM, AVG, COUNT)

Subqueries

Inventory calculations

Business Insight Extraction

💡 Project Objective

This project helped me strengthen:

Relational database design understanding

Writing efficient SQL queries

Converting raw transactional data into business insights

Thinking like a Data Analyst

📌 How to Run This Project

Create Database:

CREATE DATABASE OnlineBookstore;

Connect to database:

\c OnlineBookstore;

Create Tables

Import CSV files using COPY command

Run the analysis queries

👨‍💻 Author

##SANJAY CHOURASIYA
Aspiring Data Analyst | SQL | Power BI | Excel | Python
