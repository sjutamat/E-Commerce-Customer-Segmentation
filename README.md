# RFM Analysis Project

## Overview
This project analyzes customer behavior using Recency, Frequency, and Monetary (RFM) metrics. The goal is to segment customers and identify high-value groups.

## Data Description
The dataset includes information about products, orders, payments, and reviews, extracted from a relational database.

## Key Steps
1. Load Data from CSV files.
2. Clean the data 
    1. Remove missing or duplicated values, remove rows with missing values or fill them with appropriate values. 
    2. Format Numeric Columns ensure columns like Qauntity, UnitPrice, and TotalPrice are numeric and free of negative values.
    3. Collect Data Type ensure collumns like InvoiceDate are converted to datetime format.
3. Combine the data 
    1. Join Tables to Calculate TotalPrice to calculate TotalPrice, join order_items with products to get the product price and calculate the total cost for each item.
    2. Combine with Orders. Next, merge order_items with orders to link the TotalPrice to each order.
1. Feature engineering (TotalPrice, RFM metrics).
2. Outlier detection using boxplots and IQR.
3. Scaling with MinMaxScaler.
4. Insights from visualizations.

## Results
- Boxplots for RFM metrics.
- Scaled RFM metrics for further analysis.
- Cleaned dataset for clustering.

## How to Run
1. Clone this repository.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
