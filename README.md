# Amazon Clothing Sales Analysis – Power BI Project

## Overview

This project analyses more than twenty thousand Amazon clothing sales records to understand customer behaviour, pricing patterns, discount effectiveness, and delivery performance. The dataset includes product attributes, customer demographics, device usage, and transactional details. The goal of the project is to develop an interactive Power BI dashboard that supports sales, marketing, and operations teams with clear, data-driven insights.

## Project Objectives

The project aims to transform raw sales data into meaningful business intelligence by:

- Cleaning, transforming, and modelling the dataset.  
- Creating a star-schema data model with a DAX-based Calendar table.  
- Designing fully interactive dashboards that highlight trends across revenue, orders, customer demographics, product categories, returns, and delivery times.  
- Enabling stakeholders to filter and explore insights through slicers and dynamic visuals.

## Dataset Description

The dataset contains more than twenty thousand transactional clothing records with the following feature groups:

### Product Attributes
- Product name  
- Brand  
- Main category  
- Sub-category  

### Pricing and Discounts
- Price  
- Discount percent  
- Final price  

### Customer Details
- Region  
- Age group  

### Purchase Behaviour
- Device type  
- Payment method  

### Order Information
- Order date  
- Delivery days  
- Quantity  

### Feedback Metrics
- Review rating  
- Return status  

All columns were checked for missing, invalid, and duplicate values before modelling.

## Data Cleaning and Transformation

Main steps completed:

- Removed blank rows and blank columns.  
- Treated missing values using mean, median, or mode depending on the variable type.  
- Verified discount and pricing consistency through recalculated fields.  
- Created additional calculated columns, including:  
  - Discount Amount  
  - Unit Price  
  - Order Month, Order Year, Weekday  
  - Delivery Speed Category  
- Ensured consistent formatting for dates, numeric fields, and category labels.

## Data Modelling

A star schema was created with:

- **Fact Table:** Amazon Clothing Sales  
- **Dimension Table:** Calendar (created using DAX)

The Calendar table includes Year, Month, Quarter, and Weekday columns to enable time-series analysis. Relationships were built using Order Date as the key.

## Key Insights

### Sales Overview
- Total Orders, Total Revenue, Average Order Value, and Average Rating were calculated as core KPIs.  
- Monthly and weekly trends showed clear seasonality across product categories.  
- The Women’s category generated the highest revenue, followed by Men’s clothing.  
- The South and West regions contributed the largest share of total sales.  
- Credit Card and PayPal were the most commonly used payment methods.

### Product, Category, and Brand Performance
- Certain brands consistently ranked as top sellers in terms of revenue.  
- Sub-categories such as Shirts, Dresses, and Jackets recorded the highest volumes.  
- Categories varied in their average customer rating.  
- Age-group analysis showed distinct purchasing patterns between Teen, Adult, and Senior groups.  
- A summary table highlighted orders, revenue, average rating, and customer counts by brand.

### Customer Reviews and Delivery Insights
- Mobile devices accounted for the majority of orders.  
- Older age groups tended to give higher review ratings.  
- Delivery speed analysis showed that medium-speed deliveries (three to five days) were most common.  
- Map visualisation identified regions with the highest revenue.

## Dashboard Features

The dashboard includes:

- KPI cards for revenue, orders, and rating  
- Line charts for monthly and weekly sales trends  
- Bar charts for top categories and brands  
- Scatter plots for discount versus quantity sold  
- Maps highlighting regional revenue  
- Tables summarising product-level performance  
- Slicers for Category, Age Group, Region, Brand, and Date Range  

The visuals were designed with clarity, consistent formatting, proper alignment, readable labels, and strong use of white space.

## Deliverables

- Power BI file (.pbix)  
- Cleaned dataset  
- Dashboard pages for:  
  - Sales Overview  
  - Category and Brand Insights  
  - Review and Delivery Analysis  
