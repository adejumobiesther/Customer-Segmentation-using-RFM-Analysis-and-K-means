# Customer Segmentation using RFM Analysis and K-means

## Overview

This project analyzes data from retail transactions to perform customer segmentation. It focuses on a dataset from a UK-based online retail company that specializes in unique all-occasion gift-ware. The dataset covers the period between 01/12/2009 and 09/12/2011 and includes both individual and wholesale customers. The dataset was obtained via this [link](kaggle.com/datasets/mathchi/online-retail-ii-data-set-from-ml-repository)

## Dataset Description

The dataset contains the following columns:

- **InvoiceNo**: A 6-digit integral number uniquely assigned to each transaction. Transactions starting with 'c' indicate cancellations.
- **StockCode**: A 5-digit integral number uniquely assigned to each distinct product.
- **Description**: The name of the product.
- **Quantity**: The quantity of each product per transaction.
- **InvoiceDate**: The date and time when a transaction was generated.
- **UnitPrice**: The price per unit of the product in sterling (£).
- **CustomerID**: A 5-digit integral number uniquely assigned to each customer.
- **Country**: The name of the country where a customer resides.

## Data Processing

The data was initially loaded into a PostgreSQL database. SQL was used to clean the data by removing missing values and cancelled orders. Additionally, python was used to engineer new features to calculate the Recency, Frequency, and Monetary values for each customer.

## Customer Segmentation

Based on the calculated Recency, Frequency, and Monetary values, customers were segmented into groups using k-means. This segmentation helps the company make informed decisions regarding different customer segments and tailor their strategies accordingly.

## Visualization with Tableau

Tableau was used to create visualizations to enhance more understanding of the data. Some of the visualizations include the company's income from different products and countries per year, the number of countries patronising the company. The dashboard can be viewed via this [link](https://public.tableau.com/views/WOW202219_16844900305140/Dashboard1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link).

## Conclusion

By combining RFM analysis, K-means clustering, and data visualization, this project provides actionable insights for customer segmentation and strategic decision-making in the retail industry.
