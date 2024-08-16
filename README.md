# coffee-sales-dashboard
Overview
This project showcases an extensive Coffee Sales Dashboard developed in Excel, offering key insights into a coffee shop's sales performance during 2019-2020. The dashboard aids in identifying trends, patterns, and potential areas for enhancement.
The Coffee Sales Dashboard delivers a thorough sales data analysis, enabling businesses to track their performance over time, pinpoint top customers, and assess product preferences. The project utilizes Excel functions such as XLOOKUP, INDEX, and MATCH to efficiently collect and analyze data, with IF statements employed to simplify the data processing.

Data Description
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



