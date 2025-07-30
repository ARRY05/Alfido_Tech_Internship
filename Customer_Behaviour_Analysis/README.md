Customer Behavior E-commerce Analysis

Overview

This repository contains a customer behavior analysis project focused on e-commerce transaction data. The workflow combines, cleans, and explores two datasets to uncover insights into purchasing patterns, product preferences, payment types, and demographic trends. All analysis is completed in Python using Pandas, Seaborn, and Matplotlib.

Contents

- ecommerce_customer_data_large.csv – Main e-commerce customer transaction dataset.
- ecommerce_customer_data_custom_ratios.csv – Supplementary dataset including custom ratio metrics.
- Customer_Behaviour_Analysis.ipynb – The main notebook for data cleaning, merging, and visualization.
- README.md – This file.

Steps Performed

1. Data Loading and Merging
- Loaded both CSV files and merged them using `pd.concat`.

2. Data Cleaning & Preprocessing
- Converted the `Purchase Date` column to datetime format.
- Filled missing values in the `Returns` column with 0.
- Dropped an irrelevant or redundant column: `Customer Age`.
- Created new features:
  - Month: Extracted from `Purchase Date`.
  - DayOfWeek: Extracted day name from purchases.
  - Age Group: Binned age values into logical buckets.

3. Exploratory Data Analysis & Visualization

- Product Category Distribution:
  Countplot shows which product categories are most frequently purchased.

- Payment Methods: 
  Visualized the distribution of payment types with a countplot.

- Monthly Purchase Volume:
  Line plot to reveal purchasing trends across months.

- Average Purchase Amount by Age Group: 
  Bar plot to show how average spend fluctuates by age bracket.

Example Visualizations

- Countplot of Product Categories
- Countplot of Payment Methods
- Monthly Purchases Volume (line chart)
- Average Purchase Amount by Age Group (bar chart)

Technologies Used

- Python 3.7+
- Pandas for data handling
- Seaborn & Matplotlib for visualization
- (Optionally) Jupyter Notebook for interactive exploration

License

This project is intended for educational and exploratory purposes. Please review your organization's policies before using real customer data in a public repository.

Contact

For questions or feedback, please open an issue or reach out.
