# Customer Churn Analysis - Lloyd's Bank
### Comprehensive data processing and predictive analytics for customer retention
🎯 Project Overview
This project analyzes customer churn patterns for Lloyd's Bank using advanced data processing and machine learning techniques. The analysis encompasses both data preprocessing methodologies and exploratory data analysis findings. The study processed five separate datasets containing customer demographics, transaction history, service interactions, online activity, and churn status to create a unified analytical framework. The analysis examined 1,000 customer records across 20 engineered features to identify key factors contributing to customer attrition, revealing critical insights for strategic decision-making.
### Key Findings
* Service Quality is the primary churn driver (100% unresolved issues for churned vs. 50% for retained customers)
* Financial Behavior patterns serve as strong predictive indicators
* Digital Engagement metrics provide early warning signals


 # Data Processing and Preprocessing
The data cleaning and preprocessing pipeline successfully integrated five separate datasets to create a comprehensive customer profile database suitable for machine learning applications.
#### Original Data Sources
* Customer Demographics: 1,000 entries, 5 columns
* Transaction History: 5,054 entries, 5 columns
* Customer Service Interactions: 1,002 entries, 5 columns
* Online Activity: 1,000 entries, 4 columns
* Churn Status: 1,000 entries
### Data Quality Assessment
* Missing Value Analysis: Zero missing values detected across all datasets
* Data Completeness: 100% non-null counts for all columns
* Imputation Required: None
# Feature Engineering Process
### Transaction-Based Features
Aggregated customer-level transaction metrics from 5,054 individual transactions:

* Total Spent: Sum of all transaction amounts per customer
* Average Transaction: Mean transaction value per customer
* Transaction Count: Number of transactions per customer
* Favorite Category: Most frequently purchased product category

### Service Interaction Metrics
Derived comprehensive service quality indicators:
* Service Interaction Count: Total service contacts per customer
* Unresolved Percentage: Proportion of unresolved service issues
* Interaction Types: Breakdown by complaint, feedback, and inquiry counts
### Digital Engagement Features
Created online behavior indicators:
* Login Frequency: Customer online engagement level
* Service Usage: Online service utilization patterns
### Categorical Variable Encoding
Applied systematic encoding for machine learning compatibility:
* Marital Status: One-hot encoded to binary indicators (Married, Single, Widowed)
* Income Level: Encoded as binary features (Low, Medium)
* Gender: Maintained as categorical variable
* Service Usage: Encoded for online activity patterns
### Data Integration Methodology
Successfully merged all datasets using CustomerID as primary key
# Exploratory Data Analysis and Insights
### Customer Demographics Profile
### Age Distribution Analysis
* Age Range: 18-70 years
* Mean Age: 43.3 years (Standard Deviation: 15.2)
* Distribution: Relatively uniform across age groups
* Churn Correlation: No significant age-based churn differential
* Key Finding: Both churned and retained customers show similar age medians (~42-45 years)
### Gender and Marital Status Distribution
* Gender: Balanced representation across categories
* Marital Status Breakdown:
   * Single: 513 customers (51.3%)
   * Married: 276 customers (27.6%)
   * Other statuses: 211 customers (21.1%)
### Financial Behavior Analysis
### Spending Pattern Insights
* Spending Range: $9.80 - $3,386.04
* Distribution: Right-skewed with most customers spending $500-1,500
* Average Transaction: $248.81 (Standard Deviation: $79.37)
* Key Finding: No significant difference in spending patterns between churned and retained customers
### Service Interaction Analysis
### Service Usage Distribution
* Interaction Patterns: Three distinct peaks at 0, 1, and 2 interactions
* Majority Behavior: Minimal service interactions for most customers
* Service Channels: Mobile App, Website, Online Banking
* Key Finding: Online Banking shows highest usage among retained customers
### Critical Service Quality Findings
Unresolved Issues - Primary Churn Indicator:
* Retained Customers: ~50% unresolved issues
* Churned Customers: ~100% unresolved issues
* Impact: Strongest predictor of churn in the dataset
* Service Resolution Rate: 31.6% average unresolved rate overall
# Predictive Feature Importance Analysis
### Top Churn Predictors (Ranked by Importance)
* Average Transaction (0.16) - Highest predictor
* Total Spent (0.14) - Strong financial indicator
* Login Frequency (0.13) - Digital engagement metric
* Age (0.12) - Demographic factor
* Transaction Count (0.08) - Behavioral pattern
* Service Interaction Count (0.06) - Service engagement
* Unresolved Percentage (0.04) - Service quality metric
#  Conclusion and Next Steps
### Key Insights Summary
The comprehensive analysis reveals that customer churn at Lloyd's Bank is fundamentally a service quality issue rather than a demographic or financial behavior problem. The dramatic difference in unresolved issue rates (50% vs. 100%) between retained and churned customers represents the most significant finding and should drive immediate operational changes.
Financial behavior patterns serve as strong predictive indicators, with average transaction amounts and total spending providing early warning signals. Digital engagement through login frequency emerges as a critical metric for customer health assessment.


