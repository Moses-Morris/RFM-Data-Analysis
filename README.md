# RFM-Data-Analysis
How to Conduct The recency, frequency, monetary value (RFM) model which assigns a firm's customer base a particular trait. Improving market analysis.


# RFM Analysis with Python

This repository contains a Python script for conducting RFM (Recency, Frequency, Monetary) analysis using customer transaction data. RFM analysis is a marketing technique used to segment customers based on their purchasing behavior.

## Prerequisites

Before running the script, make sure you have the following libraries installed:

- `matplotlib`
- `pandas`
- `numpy`
- `sklearn`
- `seaborn`
- `datetime`

You can install these libraries using `pip`:

```bash
pip install matplotlib pandas numpy sklearn seaborn
```

## Usage

### Clone the Repository:

```bash
git clone <repository_url>
cd <repository_directory>
```

## Prepare Your Data:

To get started with RFM analysis, follow these steps to prepare your data:

1. **Place your transaction data:**
   - Create a CSV file named `rfm_data.csv` within the repository directory.
   - Insert your transaction data into this CSV file. Ensure that it includes columns such as `CustomerID`, `PurchaseDate`, and `TransactionAmount`.

## Run the Script:

After preparing your data, run the Python script `rfm_analysis.py` using a Python interpreter. Here's how you can do it:

```bash
python rfm_analysis.py
```



## View Output:

Upon running the script, the RFM analysis results will be displayed in the terminal or command prompt:

- **Recency:** Number of days since the last purchase for each customer.
- **Frequency:** Number of purchases made by each customer.
- **Monetary Value:** Total purchase amount for each customer.
- **RFM Scores:** Calculated scores based on Recency, Frequency, and Monetary Value.
- **RFM Segments:** Customers segmented into High Score, Mid Score, and Low Score categories.

## Explanation

### Data Loading and Preprocessing:

- The script loads customer transaction data from the `rfm_data.csv` file.
- It preprocesses the data by converting the 'PurchaseDate' column to datetime and calculating the difference in days from the current date.

### RFM Calculation:

- **Recency:** Number of days since the last purchase for each customer.
- **Frequency:** Number of purchases made by each customer.
- **Monetary Value:** Total purchase amount for each customer.

### RFM Segmentation:

- The customers are segmented into three categories: High Score, Mid Score, and Low Score based on their RFM scores.
- RFM scores are calculated using the percentile rank of Recency, Frequency, and Monetary Value.
- The segmentation results are displayed in the 'RFM_Segment' column of the output DataFrame.

### Visualization:

- The script generates a scatter plot illustrating Recency vs Frequency for the segmented customers.

## Result Interpretation

- **High Score:** Customers with a high frequency of purchase, high monetary value, and recent purchases.
- **Mid Score:** Customers with moderate purchasing behavior.
- **Low Score:** Customers with low frequency, low monetary value, and less recent purchases.
