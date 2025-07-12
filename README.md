# 🛒 Retail Database Platform Project

## 📁 `RetailDB-Analysis`

This project focuses on designing and analyzing a relational database for a retail platform. The goal is to understand database structure, develop SQL queries for business insights, and normalize data to maintain efficiency and consistency.

---

## 🎯 Project Objectives

- Design and understand a normalized relational schema for a retail database.
- Execute meaningful SQL queries to extract key business insights.
- Analyze sales trends, customer behavior, and product performance.
- Ensure data integrity using foreign keys and normalization techniques.

---

## 🧱 Database Schema Overview

The retail database contains the following key tables:

- **Customers**: Customer details including name, contact, and region.
- **Products**: Product catalog with pricing and category.
- **Orders**: Sales transactions made by customers.
- **OrderDetails**: Line items for each order (product and quantity).
- **Suppliers**: Suppliers providing the products.
- **Employees**: Staff involved in sales and order management.
- **Categories**: Classification of products.
- **Shippers**: Shipping providers for customer orders.

---

## 🔍 ERD (Entity Relationship Diagram)

The schema maintains referential integrity with:

- **One-to-Many**: Customers → Orders, Orders → OrderDetails
- **Many-to-One**: Products → Suppliers, Products → Categories
- **Foreign Keys**: Implemented across all relationships to ensure integrity

---

## 📈 Insights & Analysis
- Sales Concentration: A few high-value customers contribute disproportionately to total sales.
- Product Trends: Top products by quantity and revenue were identified using joins and aggregations.
- Time Series: Seasonal patterns in sales were explored using month-wise groupings.

## 🛠️ Technologies Used
- SQLite: Database engine
- DB Browser for SQLite: UI-based interaction
- SQL: Data querying and aggregation
- Markdown: Report formatting
---

## 🧠 Author  
**Mohammed Saif Wasay**  
*Data Analytics Graduate — Northeastern University*  
*Machine Learning Enthusiast | Passionate about turning data into insights*  
🔗 [Connect with me on LinkedIn](https://www.linkedin.com/in/mohammed-saif-wasay-4b3b64199/)
