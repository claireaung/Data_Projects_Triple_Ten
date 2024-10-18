# Instacart Customer Behavior Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Conclusion](#conclusion)
- [Further Improvements](#further-improvements)

## Project Overview
This project focuses on analyzing the shopping habits of customers on the Instacart grocery delivery platform. The dataset, originally released for a Kaggle competition in 2017, has been modified for this project to include missing and duplicate values. The goal is to clean the data and conduct exploratory data analysis (EDA) to extract meaningful insights into customer behavior. The final analysis will help Instacart in planning strategies for customer engagement.

## Dataset Description
The dataset consists of five tables:
- **instacart_orders.csv**: Details of orders placed by customers.
- **products.csv**: Information about products available on Instacart.
- **order_products.csv**: Data on products within individual orders.
- **aisles.csv**: Information on the aisle location of products.
- **departments.csv**: Data on the department for each product category.

### Data Fields:
1. **instacart_orders.csv**:
    - `order_id`: Unique identifier for each order.
    - `user_id`: Unique identifier for each customer.
    - `order_number`: Number of times the customer placed an order.
    - `order_dow`: Day of the week the order was placed.
    - `order_hour_of_day`: Hour of the day the order was placed.
    - `days_since_prior_order`: Time since the previous order.

2. **products.csv**:
    - `product_id`: Unique identifier for each product.
    - `product_name`: Name of the product.
    - `aisle_id`: Identifier for the aisle.
    - `department_id`: Identifier for the department.

3. **order_products.csv**:
    - `order_id`: Identifier for the order.
    - `product_id`: Identifier for the product.
    - `add_to_cart_order`: Order of item placement in the cart.
    - `reordered`: Whether the item has been reordered (1) or not (0).

4. **aisles.csv**:
    - `aisle_id`: Identifier for the aisle.
    - `aisle`: Name of the aisle.

5. **departments.csv**:
    - `department_id`: Identifier for the department.
    - `department`: Name of the department.

## Project Workflow

### Step 1: Data Exploration
- Load all provided datasets.
- Analyze the general structure of the datasets using `pd.read_csv()`.
- Check for missing values and duplicates.
  
### Step 2: Data Preprocessing
- Verify and fix data types (e.g., convert ID columns to integers).
- Identify and handle missing values by filling or removing them.
- Remove duplicate values and justify the methodology.

### Step 3: Data Analysis
#### [A] Mandatory Analysis:
1. Verify the 'order_hour_of_day' and 'order_dow' fields.
2. Create a plot showing the number of orders placed at each hour of the day.
3. Create a plot showing shopping behavior on different days of the week.
4. Analyze the time customers wait before placing their next order.

#### [B] Comparative Analysis:
1. Compare order distributions on Wednesdays vs. Saturdays using histograms.
2. Visualize the distribution of orders by customers (1 order, 2 orders, etc.).
3. Identify the top 20 most frequently ordered products.

#### [C] Advanced Analysis (Optional):
1. Analyze the distribution of the number of items per order.
2. Identify the top 20 most reordered products.
3. For each product, calculate the proportion of reorders.
4. Identify the top 20 products added first to the cart.

## Results
- Cleaned the dataset by addressing missing and duplicate values.
- Created insightful visualizations to understand customer shopping behavior across different days, hours, and products.
- Identified key products that are frequently reordered and those that are added to the cart first.
  
## Conclusion
Through the analysis, we discovered patterns in shopping behavior, such as peak order hours and frequently purchased products. This information can help Instacart strategize its inventory management and marketing efforts.

## Further Improvements
- Incorporate machine learning models to predict customer behavior based on past shopping data.
- Investigate customer retention strategies by analyzing reorder patterns and customer churn.
