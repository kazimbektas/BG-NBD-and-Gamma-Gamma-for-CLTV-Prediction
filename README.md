# BG-NBD-and-Gamma-Gamma-for-CLTV-Prediction

# Probabilistic Customer Lifetime Value (CLTV) Estimation with Time Projection

## Project Overview

This project focuses on **Customer Lifetime Value (CLTV)** estimation using **probabilistic models** such as the **BG/NBD Model** and the **Gamma-Gamma Submodel**. The goal is to segment customers based on their purchase behaviors and predict their future transaction patterns and profitability, enabling the company to develop tailored marketing strategies.

## Business Problem

The company aims to segment its customers based on their purchase data and calculate CLTV using probabilistic models. This helps define personalized marketing strategies to enhance customer relationships, optimize revenue, and reduce churn.

## CLTV Calculation

The formula for CLTV in this project is:
## CLTV = Expected Number of Transactions x Expected Average Profit


- **Expected Number of Transactions**: Estimated using the **BG/NBD** model.
- **Expected Average Profit**: Estimated using the **Gamma-Gamma** submodel.

## Modelling Techniques

### A) BG/NBD Model (Beta Geometric/Negative Binomial Distribution)

The **BG/NBD Model** is used to estimate the **Expected Number of Transactions** for each customer over their lifetime. This model accounts for both **purchase behavior** and **churn behavior**:

- **Transaction Process**: Modeled using the **Gamma** distribution, which estimates the frequency of transactions a customer makes within a given time frame.
- **Dropout Process**: Modeled using the **Beta** distribution, representing the likelihood of a customer ceasing to make purchases ("churning"). 

The BG/NBD model predicts **repeat purchases** and **churn probabilities** for customers, making it valuable for crafting retention strategies.

### B) Gamma-Gamma Submodel

The **Gamma-Gamma Submodel** is used to estimate the **Expected Average Profit** per transaction for each customer:

- **Transaction Value**: Modeled using the **Gamma distribution** to account for variability in customer spending patterns.
- This submodel allows for more accurate predictions of customer profitability and aids in making informed pricing and marketing decisions.

## Dataset

The project uses the **Online Retail II** dataset, which contains sales data from an online UK-based retailer between **01/12/2009** and **09/12/2011**.

### Key Variables:
- **InvoiceNo**: Unique invoice number. (If it starts with 'C', the transaction was canceled).
- **StockCode**: Unique product code.
- **Description**: Product name.
- **Quantity**: Number of units sold per invoice.
- **InvoiceDate**: Date and time of the invoice.
- **UnitPrice**: Price of the product (in Sterling).
- **CustomerID**: Unique identifier for each customer.
- **Country**: Country where the customer resides.

### Dataset Source:

The dataset can be found here: [Online Retail II Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II).

## Objective

- **Customer Segmentation**: Segment customers using the **BG/NBD Model** and **Gamma-Gamma Submodel** to predict future transaction frequency and average profit.
- **Strategic Marketing**: Develop marketing strategies tailored to each customer segment to improve customer retention and optimize marketing efforts.

## Conclusion

By leveraging the **BG/NBD** and **Gamma-Gamma** models, we can accurately estimate Customer Lifetime Value (CLTV), helping businesses focus on high-value customers, improve engagement, and maximize long-term profitability.
