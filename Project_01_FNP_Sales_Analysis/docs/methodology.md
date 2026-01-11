# Methodology — FNP Sales Analysis

This document outlines the end-to-end methodology used to clean, transform, analyze, and visualize sales data for Ferns N Petals (FNP) using Microsoft Excel and Power Query.

The workflow follows a structured analytics approach to ensure data accuracy, consistency, and actionable business insights.

---

## 1. Data Cleaning & Preparation

Data cleaning was performed using **Excel and Power Query** to improve data quality before analysis.

### Cleaning Steps Performed:
- Removed duplicate records to prevent double counting  
- Standardized date formats for **Order Date** and **Delivery Date**  
- Trimmed extra spaces and corrected inconsistent text values  
- Normalized product categories and occasion labels  
- Handled missing or null values in critical columns  
- Converted numeric fields to appropriate data types  


### New calculated Derived Fields Created:

-   **Delivery Days:**\
    `= [Delivery Date] - [Order Date]`
-   **Revenue:**\
    `= Quantity * Price`
-   **Order Hour:**\
    `= HOUR([Order Date])`
-   **Month:**\
    `= TEXT([Order Date], "MMMM")`

These derived fields enabled time-based, revenue-based, and operational performance analysis.

------------------------------------------------------------------------

## 2. Power Query (ETL Process)

Power Query was used to perform **ETL (Extract, Transform, Load)** operations and prepare a clean analytical dataset.

### ETL Workflow:

        Source Data
        → Promoted Headers 
        → Changed Data Types
        → Trimmed Text Fields 
        → Removed Duplicates
        → Filled Down Missing Values
        → Added Custom Columns (Delivery Days, Revenue) 
        → Date Formatting 
        → Loaded into Excel Data Model

This process ensured repeatability, scalability, and clean data transformation.

---

## 3. Pivot Tables & Data Modeling

Pivot tables were created to analyze sales performance across multiple business dimensions.

### Pivot Analyses Included:
- Revenue by Occasion  
- Revenue by Category  
- Hourly Order Distribution  
- Monthly Sales Trends  
- Top 10 Cities by Orders  
- Top 5 Products by Revenue  
- Delivery Time vs Order Quantity  

### Interactivity:
- Slicers connected across all pivot tables for:
  - Occasion  
  - Category  
  - City  

This enabled dynamic filtering and cross-analysis.

---

## 4. Dashboard Design & Visualization

An interactive dashboard was designed to present insights clearly and effectively for business stakeholders.

### Dashboard Components:
- KPI Cards (Total Revenue, Total Orders, Average Order Value)  
- Line and Column Charts for trend analysis  
- Hourly order trend visualization  
- Category and Occasion performance heat maps  
- Clean, business-focused UI layout  
- Slicers and Timeline controls for user interactivity  

The dashboard supports quick interpretation and executive-level reporting.

---

## Final Output

The final deliverable is a **dynamic Excel dashboard** that enables real-time exploration of sales performance, customer behavior, and operational efficiency for FNP’s sales operations.

This methodology demonstrates a complete Excel-based analytics workflow—from raw data to actionable business insights.

