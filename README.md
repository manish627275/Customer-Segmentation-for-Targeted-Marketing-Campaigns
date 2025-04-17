# Customer Segmentation for Targeted Marketing Campaigns

## Overview

This project segments customers based on their purchasing behavior using **RFM analysis** and **machine learning techniques**. The insights are used to develop targeted marketing strategies to improve customer engagement, retention, and revenue.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Key Insights](#key-insights)
5. [Installation](#installation)

---

## Project Overview

This project aims to segment customers to better understand their purchasing behavior and tailor marketing strategies accordingly.

---

## Dataset

The dataset used is the **Online Retail Dataset**, which contains transactional data for an online retail store. It includes the following columns:

- `InvoiceNo`: Unique identifier for each transaction  
- `StockCode`: Unique identifier for each product  
- `Description`: Description of the product  
- `Quantity`: Number of units purchased  
- `InvoiceDate`: Date and time of the transaction  
- `UnitPrice`: Price per unit of the product  
- `CustomerID`: Unique identifier for each customer  
- `Country`: Country where the transaction occurred  

**Dataset Source**: Online Retail Dataset

---

## Methodology

### Data Cleaning
- Handled missing values and removed canceled orders  
- Created new features like `TotalSpend`  

### Exploratory Data Analysis (EDA)
- Analyzed customer distribution by country  
- Identified top products and total spend trends  

### Customer Segmentation
- Used **RFM analysis** to calculate Recency, Frequency, and Monetary values  
- Applied **K-Means clustering** to group customers into segments  

### Predictive Modeling
- Built a **Random Forest model** to predict customer churn  

### Customer Lifetime Value (CLV)
- Calculated CLV for each customer segment  

---

## Key Insights

### Customer Segments
- Identified key segments: **Champions**, **Loyal Customers**, **Potential Loyalists**, **At Risk**
- High-value segment (e.g., **551 Segment**) contributes significantly to revenue  

### Churn Prediction
- The **Random Forest model** achieved perfect accuracy (**1.00**) in predicting churn  
- **Recency** and **Frequency** are the most important predictors  

### Customer Lifetime Value (CLV)
- The **551 Segment** has the highest CLV (**$1,765,910**), making it the most valuable customer group  

### Actionable Recommendations
- Proposed targeted marketing strategies for each segment to improve engagement and retention  

---

## Installation

To run this project, install the required Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly
