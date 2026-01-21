# Bakery Sales Analysis & Association Rule Mining

### Problem Statement
In the competitive retail bakery environment, understanding customer purchasing behavior and optimizing product offerings are essential for sustainable growth. Despite having access to transaction data, many small-to-medium bakeries struggle to derive actionable insights from their sales records.

The core challenges addressed in this project are:

1. **Undiscovered Product Associations:** The bakery lacks a data-driven understanding of which products are frequently purchased together. Without identifying these "Market Baskets", the business cannot effectively design product bundles or cross-selling strategies.

2. **Inefficient Inventory & Staffing:** Sales fluctuate significantly across different times of the day (Morning, Afternoon, Evening) and seasons. Without a precise analysis of these trends and a reliable forecasting model, the bakery risks either overstocking (leading to waste) or understocking during peak hours (resulting in lost revenue).

3. **Lack of Customer Personalization:** The bakery treats its customer base as a monolith. By not segmenting customers based on their specific purchasing habits, the business misses the opportunity to create targeted marketing campaigns and loyalty rewards that cater to different high-value groups.

### Objective: 
The goal of this project is to leverage Association Rule Mining (Apriori Algorithm) and Time Series Forecasting to transform raw transaction data into strategic business intelligence. This will enable the bakery to optimize its menu, improve operational efficiency through demand prediction, and enhance the customer experience through data-backed promotions.

<img src="bakery.png" alt="Picture" width="300"/>

### Project Overview
This project provides a comprehensive analysis of bakery transaction data to uncover customer purchasing patterns and business performance trends. By leveraging data science techniques such as Association Rule Mining and Time Series Forecasting, the study identifies key product relationships (e.g., "The Coffee Effect") and predicts future sales to optimize inventory and marketing strategies.

### Key Features

1. **Exploratory Data Analysis (EDA):** Visualization of daily, weekly, and monthly sales patterns to identify peak business periods.
2. **Time-Based Segmentation:** Analysis of sales across different dayparts: Morning, Afternoon, Evening, and Night.
3. **Association Rule Mining (Market Basket Analysis):** Implementation of the Apriori Algorithm to identify frequent itemsets and product bundles (e.g., Coffee with Pastries or Medialunas).
4. **Network Visualization:** Interactive network graphs using NetworkX to visualize the strength of connections between different bakery items.
5. **Sales Forecasting:** Time series forecasting using the Prophet tool to predict demand fluctuations.
6. **Customer Segmentation:** Clustering customers based on purchasing behavior using K-Means Clustering.

### Dataset Summary
The analysis is performed on a dataset containing over 20,500 transactions.

**Transactions:** 20,507 rows

**Columns:** Date, Time, Transaction ID, Item

**Unique Items:** 94 different products

**Top Sellers:** Coffee (5,471 sales), Bread (3,325 sales), and Tea (1,435 sales).

### Tech Stack
**Languages:** Python 3.10

**Data Manipulation:** pandas, numpy

**Visualization:** matplotlib, seaborn, networkx

**Machine Learning:** mlxtend (Apriori & Association Rules), scikit-learn (K-Means)

**Forecasting:** Prophet

### Methodology
**Data Cleaning:** Handling missing values and formatting date/time objects.

**Market Basket Analysis:**

One-hot encoding transactions using TransactionEncoder.

Generating frequent itemsets with a defined minimum support.

Extracting rules based on metrics like Support, Confidence, and Lift.

Visualization: Mapping rules into a network graph where nodes represent items and edges represent the strength of association.

### Strategic Recommendations
Based on the data, the project suggests:

1. Custom Bundling: Creating "Coffee & Pastry" combos to increase the average transaction value.

2. Seasonal Promotions: Adjusting inventory and staffing based on identified peak hours and seasonal trends.

3. Targeted Marketing: Leveraging customer segments for personalized loyalty rewards.

### How to Run
1. Clone the repository.

2. Ensure you have the required libraries installed:

```Bash

pip install pandas numpy matplotlib seaborn mlxtend networkx prophet scikit-learn
```

3. Open bakery-sales-analysis.ipynb in Jupyter Notebook or Kaggle.

