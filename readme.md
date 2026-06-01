# Customer Transaction Analysis Using Matplotlib and Seaborn

## Project Overview

This project focuses on analyzing customer transaction data using Python's data visualization libraries, **Matplotlib** and **Seaborn**. The objective is to uncover customer spending patterns, identify relationships between transaction variables, analyze transaction trends over time, and detect unusual purchasing behavior through visual analytics.

The analysis was performed on a customer transaction dataset containing information such as customer age, income, purchase amount, number of items purchased, product category, and transaction date.

---

## Dataset Description

The dataset contains the following attributes:

| Column Name      | Description                         |
| ---------------- | ----------------------------------- |
| Transaction_ID   | Unique transaction identifier       |
| Customer_ID      | Unique customer identifier          |
| Age              | Customer age                        |
| Income           | Customer annual income              |
| Purchase_Amount  | Amount spent during the transaction |
| Items_Purchased  | Number of items purchased           |
| Category         | Product category                    |
| Transaction_Date | Date of transaction                 |

---

## Objectives

The project aims to:

* Visualize the distribution of transaction amounts.
* Analyze correlations between customer-related variables.
* Examine transaction trends over time.
* Detect and analyze outliers in purchase behavior.
* Compare purchase patterns across different product categories.

---

## Tools and Libraries Used

* Python
* Pandas
* Matplotlib
* Seaborn
* NumPy

---

## Visualizations Performed

### 1. Distribution of Transaction Amounts

A histogram with a Kernel Density Estimation (KDE) curve was created to understand customer spending behavior.

#### Findings

* Most transactions fall between ₹200 and ₹1200.
* The distribution is positively skewed (right-skewed).
* A small number of transactions exceed ₹5000.
* The maximum transaction amount exceeds ₹10000.

#### Interpretation

The majority of customers make low to medium-value purchases, while a small number of customers contribute significantly through large transactions.

---

### 2. Correlation Heatmap

A correlation matrix was generated using Age, Income, Purchase Amount, and Items Purchased.

#### Findings

| Variable Pair                     | Correlation |
| --------------------------------- | ----------- |
| Income & Purchase Amount          | 0.45        |
| Age & Purchase Amount             | 0.00082     |
| Age & Income                      | 0.000024    |
| Items Purchased & Purchase Amount | -0.0085     |

#### Interpretation

* Income has a moderate positive relationship with Purchase Amount.
* Age has almost no impact on spending behavior.
* Number of items purchased shows negligible correlation with transaction value.

The analysis suggests that customer income is the strongest factor influencing spending.

---

### 3. Transaction Trend Analysis

A time-series visualization was created to examine the number of transactions occurring each day.

#### Findings

* Daily transactions fluctuate between approximately 40 and 73 transactions.
* No major upward or downward trend is visible throughout the year.
* Several short-term spikes occur during specific periods.

#### Interpretation

Customer activity remains stable throughout the year, indicating consistent engagement and purchasing behavior.

---

### 4. Moving Average Trend Analysis

A 7-day moving average was applied to smooth daily fluctuations and reveal underlying patterns.

#### Findings

* The moving average remains relatively stable between 52 and 58 transactions per day.
* No significant long-term growth or decline is observed.

#### Interpretation

The business maintains a steady transaction volume over time, suggesting stable customer demand.

---

### 5. Outlier Detection

A boxplot and the Interquartile Range (IQR) method were used to identify unusual transaction values.

#### Findings

* A total of 239 outliers were detected.
* Several transactions exceed ₹5000.
* Extreme values reach over ₹10000.

#### Interpretation

These outliers may represent:

* Premium customers
* Bulk purchases
* Corporate orders
* Special promotional purchases

Such transactions are important and should be analyzed rather than immediately removed.

---

### 6. Category-Wise Purchase Analysis

A boxplot was created to compare purchase amounts across different product categories.

#### Findings

* Median purchase amounts are relatively similar across categories.
* All categories contain high-value outliers.
* The Sports category exhibits the highest transaction values.

#### Interpretation

Customer spending patterns are generally consistent across product categories, although some categories attract occasional high-spending customers.

---

## Key Insights

1. Customer income is the most influential factor affecting purchase amount.
2. Most transactions are low to medium in value, with a few exceptionally large purchases.
3. Daily transaction volume remains stable throughout the year.
4. High-value customers contribute significantly to overall revenue.
5. Significant outliers exist and may represent valuable customer segments.
6. Spending patterns are broadly similar across product categories.

---

## Conclusion

The analysis reveals that customer spending behavior is largely influenced by income rather than age. The purchase amount distribution is highly right-skewed, indicating that while most customers make moderate purchases, a small number of high-value transactions contribute substantially to total revenue.

Transaction activity remains stable throughout the year, and the presence of 239 outliers highlights the importance of premium or bulk-purchasing customers. These insights can help businesses better understand customer behavior, identify valuable customer segments, and make data-driven decisions for marketing and sales strategies.

---

## Future Improvements

* Customer segmentation using clustering techniques.
* Sales forecasting using time-series models.
* Category-wise customer behavior analysis.
* Predictive modeling for purchase amount estimation.
* Dashboard creation using Power BI or Tableau.

---

## Author

Varun Sinha

B.Tech Computer Science and Engineering

SRM Institute of Science and Technology
