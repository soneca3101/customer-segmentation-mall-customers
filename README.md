# Customer Segmentation with KMeans - Mall Customers Dataset

## Project Overview

This project applies exploratory data analysis and unsupervised machine learning to segment mall customers based on demographic and behavioral characteristics.

The goal is to help a retail marketing team better understand customer profiles and design targeted marketing strategies.

Dataset: Mall Customers Dataset from Kaggle.

## Business Problem

Retail companies often run generic marketing campaigns for all customers, which can reduce campaign efficiency and increase costs.

Customer segmentation helps identify groups of customers with similar behavior, allowing the business to create more personalized and effective marketing actions.

## Business Questions

- What are the main customer profiles in the dataset?
- How do income and spending score relate to each other?
- Can we identify high-value and high-potential customer groups?
- What marketing actions should be recommended for each segment?

## Dataset Description

The dataset contains customer-level information from a mall, including:

- CustomerID
- Gender
- Age
- Annual Income
- Spending Score

The `Spending Score` represents a behavioral score assigned to customers based on their spending patterns.

## Methodology

The project follows these steps:

1. Data loading and initial inspection
2. Data cleaning and column standardization
3. Exploratory Data Analysis
4. Feature selection for clustering
5. Feature scaling using StandardScaler
6. Elbow Method to choose the number of clusters
7. KMeans clustering
8. Cluster profiling
9. Business interpretation
10. Marketing recommendations

## Machine Learning Approach

KMeans was used as the clustering algorithm because it is simple, interpretable, and effective for identifying customer groups based on numerical features.

The main features used for clustering were:

- Annual Income
- Spending Score

The data was scaled before modeling because KMeans is distance-based and can be affected by variables with different scales.

## Key Insights

The clustering analysis identified distinct customer segments, such as:

- High income and high spending customers
- High income and low spending customers
- Low income and high spending customers
- Low income and low spending customers
- Average income and average spending customers

These segments provide actionable insights for marketing strategy.

## Business Impact

This segmentation can help the marketing team:

- Improve campaign personalization
- Increase customer engagement
- Identify premium customers
- Activate high-income customers with low spending
- Design better loyalty programs
- Optimize promotional investments

## Marketing Recommendations

### Premium Customers

Customers with high income and high spending score.

Recommended actions:

- VIP loyalty program
- Exclusive offers
- Early access to new products
- Personalized premium campaigns

### High Income / Low Spending Customers

Customers with high purchasing power but low spending behavior.

Recommended actions:

- Reactivation campaigns
- Premium bundles
- Personalized offers
- Customer surveys to understand barriers

### Low Income / High Spending Customers

Customers with lower income but high spending score.

Recommended actions:

- Cashback
- Discounts
- Loyalty points
- Seasonal promotions

### Low Income / Low Spending Customers

Customers with low income and low spending score.

Recommended actions:

- Price-sensitive campaigns
- Entry-level product offers
- Awareness campaigns

### Average Customers

Customers with moderate income and moderate spending behavior.

Recommended actions:

- Cross-sell campaigns
- Standard loyalty program
- Product recommendations

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Repository Structure

```text
customer-segmentation-mall-customers/
│
├── data/
│   └── Mall_Customers.csv
│
├── notebooks/
│   └── customer_segmentation_kmeans.ipynb
│
├── images/
│   └── cluster_plot.png
│
├── README.md
└── requirements.txt
