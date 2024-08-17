# coffee-sales-dashboard 
Overview:

This project showcases an extensive Coffee Sales Dashboard developed in Excel, offering key insights into a coffee shop's sales performance during 2019-2020. The dashboard aids in identifying trends, patterns, and potential areas for enhancement.

The Coffee Sales Dashboard delivers a thorough sales data analysis, enabling businesses to track their performance over time, pinpoint top customers, and assess product preferences. The project utilizes Excel functions such as XLOOKUP, INDEX, and MATCH to efficiently collect and analyze data, with IF statements employed to simplify the data processing.

# Data Description:

The dataset contains the following columns in the Orders sheet:

•	Order ID: A unique identifier assigned to each order.

•	Order Date: The date when the order was placed.

•	Customer ID: A unique identifier for each customer.

•	Product ID: A unique identifier for each product.

•	Quantity: The number of units sold in each order.

•	Customer Name: The name of the customer who placed the order.

•	Email: The email address of the customer.

•	Country: The country where the order was placed (derived using the XLOOKUP function from the Customers sheet).

•	Coffee Type: The specific type of coffee product sold.

•	Roast Type: The type of roast for the coffee.

•	Size: The size of the coffee product.

•	Unit Price: The price per unit of the product.

•	Sales: The total revenue generated from each sale (calculated as Quantity multiplied by Unit Price).

•	Coffee Type Name: The name of the coffee type (created using the IF function).

•	Roast Type Name: The name of the roast type (created using the IF function).

•	Loyalty Card: Indicates whether the customer has a loyalty card (retrieved using the XLOOKUP function from the Customers sheet).


# Dashboard Features:

The Excel dashboard offers the following features:

•	Sales Trends: A visual representation of sales over time, highlighting peaks and valleys.

•	Product Performance: An evaluation of how different coffee products are performing in terms of sales.

•	Revenue Breakdown: A detailed analysis of total sales revenue, segmented by product and country.

•	Customer Insights: Insights into sales patterns based on customer types and loyalty card holders.

•	Top Products: Identification of the best-selling products and their impact on overall sales.


# How to Use:

To utilize the dashboard:

•	Open the Excel file available in this repository.

•	Explore the various sheets to gain insights into different aspects of the data.

•	Apply filters and pivot tables to customize the view to your preferences.

# Snapshot of Dashboard (Excel)
# Steps followed:
# 1. Data Exploration and Initial Setup

# Step 1: Check the Data

Open the Excel file and examine the three different sheets available: Orders, Customers, and Products. Identify the key information and how it is distributed across these sheets.

# 2. Data Gathering and Preparation
   
# Step 2: Gather Customer Data

-Use the XLOOKUP function to create the Customer Name column in the Orders sheet.

=XLOOKUP([@Customer ID], Customers!A:A, Customers!B:B)

-Apply the same XLOOKUP function to create the Email, Country, and Loyalty Card columns.

=XLOOKUP([@Customer ID], Customers!A:A, Customers!C:C) ' For Email

=XLOOKUP([@Customer ID], Customers!A:A, Customers!G:G) ' For Country

=XLOOKUP([@Customer ID], Customers!A:A, Customers!I:I) ' For Loyalty Card

# Step 3: Gather Product Data
-Use the INDEX MATCH functions to create the Coffee Type, Roast Type, Size, and Unit Price columns in the Orders sheet.

Step 4: Calculate Sales

Create the Sales column by multiplying the Quantity and Unit Price.

Step 5: Simplify Coffee Type and Roast Type Names

Use the IF function to create readable names for Coffee Type Name and Roast Type Name columns.

Here is the formula;

=IF([@Coffee Type]="Rob","Robusta",IF([@Coffee Type]="Exc","Excelsa",IF([@Coffee Type]="Ara","Arabica",IF([@Coffee Type]="Lib","Liberica",""))))

# 4. Creating the Dashboard

# Step 6: Design the Dashboard Layout

Plan the layout of your dashboard, deciding which charts and tables will best display your insights.

# Step 7: Create Pivot Tables and Charts

-Use pivot tables to summarize the data by various dimensions such as date, roast type, and top 5 customers.

-Create charts to visualize trends, product performance, revenue breakdown, and customer insights.

# Step 8: Integrate Pivot Tables and Charts into the Dashboard

-Arrange the pivot tables and charts on a new sheet designated as the dashboard.

-Ensure the dashboard is interactive, using slicers and filters to allow users to explore the data dynamically.

# Step 9: Format and Finalize the Dashboard
-Apply consistent formatting to ensure the dashboard is visually appealing and easy to read.

-Add titles, labels, and legends to charts for clarity.

# Step 10: Review and Test the Dashboard

-Verify the accuracy of the data and the functionality of the dashboard.

-Test the dashboard to ensure all interactions work as expected.





