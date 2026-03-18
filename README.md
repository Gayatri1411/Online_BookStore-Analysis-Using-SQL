# Online_BookStore-Analysis-Using-SQL

### 1. PROJECT OVERVIEW:
This project focuses on analyzing an online bookstore dataset using SQL to extract meaningful insights related to sales performance, customer behavior, and inventory management.

### 2. PROBLEM STATEMENT:
An online bookstore collects large amounts of transactional data, but lacks clarity on how to use this data effectively for decision-making.
The business is facing the following challenges:
- Which **genres and books** are performing well?
- Who are the most valuable and **repeat customers**?
- What is the overall **revenue generated**?
- Which books are at risk of going **out of stock**?
- Which **regions or cities** generate higher revenue?

Without answering these questions, the business cannot:
- **Optimize inventory**
- Improve **marketing strategies**
- Identify **high-value customers**
- **Maximize revenue** opportunities

### 3. OBJECTIVE: 
The goal of this project is to use SQL to:
- Analyze book **sales and pricing trends**
- Understand **customer purchasing patterns**
- Identify **high-performing products and customers**
- Generate insights to **support business decisions**

### 4. DATABASE SCHEMA:
The analysis is performed using structured query language (SQL) by working with three relational tables: Books, Customers, and Orders.
 - **BOOKS TABLE:** Stores information about all available books in the bookstore.
   
| Column Name      | Data Type        | Description                          |
|------------------|------------------|--------------------------------------|
| Book_ID          | SERIAL (PK)      | Unique identifier for each book      |
| Title            | VARCHAR(100)     | Name of the book                     |
| Author           | VARCHAR(100)     | Author of the book                   |
| Genre            | VARCHAR(50)      | Category of the book                 |
| Published_Year   | INT              | Year the book was published          |
| Price            | NUMERIC(10,2)    | Price of the book                    |
| Stock            | INT              | Number of books available in stock   |

-- Helps in analyzing book performance
-- Used for pricing analysis
-- Supports inventory management

- **Customers TABLE:** Stores details about customers who place orders.
  
| Column Name   | Data Type     | Description                        |
|--------------|--------------|------------------------------------|
| Customer_ID  | SERIAL (PK)  | Unique customer identifier         |
| Name         | VARCHAR(100) | Customer name                      |
| Email        | VARCHAR(100) | Customer email address             |
| Phone        | VARCHAR(15)  | Contact number                     |
| City         | VARCHAR(50)  | City of the customer               |
| Country      | VARCHAR(150) | Country of the customer            |

-- Used for regional analysis -- Supports customer segmentation
  
- **Orders TABLE:** Stores all transaction-related data.
  
| Column Name   | Data Type        | Description                              |
|--------------|------------------|------------------------------------------|
| Order_ID     | SERIAL (PK)      | Unique order identifier                  |
| Customer_ID  | INT (FK)         | References Customers(Customer_ID)        |
| Book_ID      | INT (FK)         | References Books(Book_ID)                |
| Order_Date   | DATE             | Date when the order was placed           |
| Quantity     | INT              | Number of books purchased                |
| Total_Amount | NUMERIC(10,2)    | Total amount for the order               |

-- Tracks sales transactions -- Used for revenue analysis -- Helps identify buying patterns

### 5. SQL CONCEPTS USED: 
This project covers:
- **Data Definition Language (DDL):** CREATE DATABASE, CREATE TABLE, DROP TABLE
- **Data Query Language (DQL):** SELECT, WHERE
- **Aggregation Functions:** SUM(), AVG(), COUNT()
- **Filtering & Sorting:** WHERE, BETWEEN,  DISTINCT, ORDER BY, LIMIT
- **Joins:** INNER JOIN
- **Grouping:** GROUP BY, HAVING

### 6. ANALYSIS AND BUSINESS QUESTIONS: 
### 7. KEY INSIGHTS: 
### 8. HOW TO RUN THIS PROJECT:
### 9. KEY SKILLS DEMONSTRATED:
### 10. RESULT AND CONCLUSION: 







