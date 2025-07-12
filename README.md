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

## 📊 Sample SQL Queries

### 🧾 Top 5 Selling Products

```sql
SELECT p.ProductName, SUM(od.Quantity) AS TotalSold
FROM OrderDetails od
JOIN Products p ON od.ProductID = p.ProductID
GROUP BY p.ProductName
ORDER BY TotalSold DESC
LIMIT 5;
