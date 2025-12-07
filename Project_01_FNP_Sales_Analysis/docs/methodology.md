# 🔧 Methodology --- FNP Sales Analysis

This document explains the **data cleaning, transformation, and
modelling** steps used to build the Excel dashboard.

------------------------------------------------------------------------

## 🧼 1. Data Cleaning

Performed in Excel + Power Query:

-   Removed duplicates\
-   Standardized date formats (Order/Delivery Date)\
-   Trimmed spaces & cleaned text fields\
-   Fixed category and occasion labels\
-   Removed null values in essential fields\
-   Converted numeric columns to proper types

### ✔ New calculated fields created:

-   **Delivery Days:**\
    `= [Delivery Date] - [Order Date]`
-   **Revenue:**\
    `= Quantity * Price`
-   **Order Hour:**\
    `= HOUR([Order Date])`
-   **Month:**\
    `= TEXT([Order Date], "MMMM")`

------------------------------------------------------------------------

## 🔄 2. Power Query (ETL Steps)

    Source → Promoted Headers → Changed Type →
    Trimmed Text → Removed Duplicates → Filled Down →
    Added Custom Column (DeliveryDays) →
    Added Custom Column (Revenue) →
    Formatted Dates → Loaded to Excel Data Model

------------------------------------------------------------------------

## 📈 3. Pivot Models

Created pivot tables for:

-   Revenue by Occasion\
-   Revenue by Category\
-   Revenue by Hour\
-   Monthly Sales Trend\
-   Top 10 Cities\
-   Top 5 Products\
-   Delivery Time vs Order Quantity

Connected slicers for:

-   Occasion\
-   Category\
-   City

------------------------------------------------------------------------

## 📊 4. Dashboard Development

-   KPI Cards (Revenue, Orders, Avg Spend)\
-   Line & Column charts\
-   Hourly trend visual\
-   Category & Occasion heat maps\
-   Clean UI layout\
-   Slicers + Timeline for interactivity

------------------------------------------------------------------------

## ✔ Output

A dynamic Excel dashboard enabling real-time exploration and business
insights for FNP's sales operations.
