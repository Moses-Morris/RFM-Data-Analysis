# Customer Segmentation using RFM Analysis

## Overview

This Python script performs customer segmentation utilizing RFM (Recency, Frequency, Monetary) analysis. RFM analysis is a technique widely used in marketing to analyze customer behavior based on their transaction history. In this script, customer data is loaded from a CSV file, preprocessed, RFM scores are calculated, customers are segmented, and the segmentation is visualized using a scatter plot.

## Dependencies

- **matplotlib.pyplot:** Used for creating visualizations.
- **pandas:** Used for data manipulation and analysis.
- **numpy:** Used for numerical computations.
- **sklearn:** Used for machine learning algorithms (although not utilized in this code).
- **seaborn:** Used for statistical data visualization.
- **datetime:** Used for working with dates and times.

## Code Explanation

### Data Loading and Preprocessing

The script begins by importing necessary libraries and loading customer data from a CSV file (`rfm_data.csv`) into a Pandas DataFrame. The `PurchaseDate` column is converted to datetime format to facilitate calculations. The script then computes the difference in days between the purchase dates and the current date.

### RFM Calculation

- **Recency:** The number of days since the last purchase for each customer is calculated.
- **Frequency:** The number of purchases made by each customer is calculated.
- **Monetary Value:** The total purchase amount for each customer is calculated.

### RFM Segmentation

Customers are segmented into three categories based on their RFM scores: High Score, Mid Score, and Low Score. The segmentation logic is defined in the `checkScore` function. RFM scores and corresponding segments are added to the `rfmDataFrame`.

### Visualization

A scatter plot is generated to visualize the relationship between Recency and Frequency for segmented customers. The x-axis represents Recency, the y-axis represents Frequency, and different segments are represented by distinct colors.

## Usage

Ensure you have the required Python libraries installed before running the code. Execute the script in a Python environment to perform customer segmentation and visualize the results.

## Output

The script outputs a Pandas DataFrame (`rfmDataFrame`) containing RFM scores and segments. Additionally, it generates a scatter plot visualizing Recency vs Frequency for the segmented customers.

