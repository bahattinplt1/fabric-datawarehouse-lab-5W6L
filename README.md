# Fabric Data Warehouse Lab - Sales Reporting Project

This repository contains the full implementation of a data warehouse and reporting workflow built using **Microsoft Fabric**. The goal of the project is to demonstrate how to design a star schema data model, populate it with sample data, run analytical queries, and visualize results using Power BI.

## 📌 Project Objective

To simulate a real-world sales reporting scenario by:
- Building a relational data warehouse (star schema)
- Loading and querying data using SQL
- Creating a semantic model with relationships
- Designing a Power BI report that summarizes total sales by product category

## 📁 Contents

- `Screenshots/`: Key visuals from each stage of the project (model design, queries, report)
- `report/Sales_Report.pdf` _(optional)_: Final Power BI report exported as PDF
- `README.md`: Project description and guidance

## 🛠️ Tools & Platform

- **Microsoft Fabric**
- SQL Analytics (T-SQL)
- Visual Query Editor
- Power BI Embedded

## 🧱 Data Model

The warehouse includes the following tables:

- `FactSalesOrder`: Core sales fact table
- `DimProduct`: Product details (category, name, etc.)
- `DimCustomer`: Customer details (region, etc.)
- `DimDate`: Calendar attributes

Relationships were defined as:
- `FactSalesOrder.ProductKey` → `DimProduct.ProductKey`
- `FactSalesOrder.CustomerKey` → `DimCustomer.CustomerKey`
- `FactSalesOrder.SalesOrderDateKey` → `DimDate.DateKey`

This forms a classic **star schema** suitable for analysis.

## 📊 Visual Reporting

Using Power BI, a bar chart was created to show:

> **Total Sales by Category**

This visual helps stakeholders quickly understand which product groups drive the most revenue.

## ✅ Outcome

At the end of the project:
- A functional warehouse was created and populated
- A semantic model was built
- A clean, insightful report was generated

This lab demonstrates how Microsoft Fabric can be used end-to-end for modern data warehousing and business intelligence workflows.

---

## 🖼 Sample Screenshots

📂 See the `Screenshots/` folder for visuals such as:

- Model layout  
- SQL queries  
- Visual query builder  
- Final Power BI report

