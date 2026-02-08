Student Name: SHYAKA Billy
Course: Database Development with PL/SQL (INSY 8311)
Assignment: Individual Assignment I
DBMS: Oracle SQL Developer / Oracle Database


EXECUTIVE SUMMARY
This document presents the design and implementation of a relational database system for a multi-branch supermarket. 
The project applies SQL JOIN operations and Window Functions to analyze sales performance, customer behavior, and revenue trends.
The solution follows industry-standard database design principles and demonstrates practical analytical SQL skills.


PROJECT OBJECTIVES
• Rank top-performing products by regional revenue using RANK()
• Calculate cumulative revenue using SUM() OVER()
• Analyze month-to-month sales variation using LAG()
• Segment customers by spending behavior using NTILE(4)
• Identify inactive customers and unsold products


BUSINESS CONTEXT
Supermarkets generate high volumes of transactional data across multiple branches and regions.
Without structured databases and analytical queries, it becomes difficult to monitor performance, optimize inventory, 
and support strategic decision-making. This project addresses those challenges using Oracle SQL.


DATABASE ARCHITECTURE
Tables:
• CUSTOMERS
• BRANCHES
• PRODUCTS
• TRANSACTIONS
• TRANSACTION_ITEMS


IMPLEMENTATION
Schema creation script:
schema/create_tables.sql

Data insertion script:
schema/insert_data.sql


SQL JOIN IMPLEMENTATION
• INNER JOIN – Combines customers, transactions, and products
• LEFT JOIN – Identifies customers without transactions
• RIGHT JOIN – Finds unsold products
• FULL OUTER JOIN – Displays all customers and transactions
• SELF JOIN – Matches customers in the same region


WINDOW FUNCTIONS
• RANK() – Top-selling products per region
• SUM() OVER() – Running revenue totals
• LAG() – Monthly revenue change analysis
• NTILE(4) – Customer spending segmentation


REPOSITORY STRUCTURE
wINDOWS-26918-SHYAKA-BILLY/
- schema/
- joins/
- window_functions/
- screenshots/



CONCLUSION
This project demonstrates how relational databases and advanced SQL analytics can transform raw transaction data into actionable business insights.
