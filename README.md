Supply Chain Performance Analysis
Project Overview
This project involves a comprehensive analysis of a supply chain dataset to identify critical factors influencing delivery performance and profitability. The goal is to uncover patterns, pinpoint bottlenecks, and provide actionable insights for optimizing supply chain operations.

Dataset
The analysis is based on the DataCoSupplyChainDataset.csv, which contains detailed information about orders, shipments, customer data, and product details.

Methodology
Data Loading and Initial Exploration: Loaded the dataset using pandas and performed an initial check for dimensions, duplicates, and missing values.
Data Cleaning and Preprocessing:
Dropped irrelevant and redundant columns (e.g., Product Description, Customer Email, Latitude, Longitude).
Removed cancelled orders from the dataset.
Converted date columns (order date (DateOrders), shipping date (DateOrders)) to datetime objects using pandas for time-based analysis.
Feature Engineering:
Calculated Order Processing Time and Delay (in days).
Created Is_Delayed flag.
Extracted order_month, order_day, and order_hour from the order date.
Introduced a Profitability Flag (Profit, Loss, Break-Even) based on Order Profit Per Order.
Exploratory Data Analysis (EDA):
Computed key business KPIs such as total orders, late deliveries, on-time delivery percentage, and overall profit/loss.
Visualized the profitability distribution using matplotlib.
Analyzed delay distribution and profit metrics by delay days to understand the impact of delays on profitability.
Bottleneck Distribution Analysis:
Identified top categories contributing to delivery delays (e.g., Order Region, Customer Segment, Shipping Mode, Department Name) by calculating the delay percentage for each category.
Visualized these distributions using seaborn and matplotlib.
Root Cause Analysis:
Developed a function to identify the top drivers of late delivery within specific regions by analyzing Shipping Mode, Customer Segment, Department Name, Type, and Order Status.
Visualized these drivers to highlight areas for targeted improvements.
Time-Based Analysis:
Examined delay trends over time by analyzing delay percentages across months, days of the week, and hours of the day.
Used matplotlib and seaborn to visualize these temporal patterns, identifying peak periods for delays.
Key Findings
Identified specific regions and shipping modes with higher late delivery rates.
Understood the impact of delays on overall order profitability.
Uncovered temporal patterns in delivery delays, suggesting potential for schedule optimization.
Libraries Used
pandas for data manipulation and analysis.
matplotlib.pyplot for creating static, interactive, and animated visualizations.
numpy for numerical operations.
seaborn for statistical data visualization.
matplotlib.ticker and matplotlib.cm for fine-tuning plot aesthetics.
And here are the 4 points summarizing this project for your resume:

Supply Chain Data Preprocessing & Feature Engineering: Processed a raw supply chain dataset (DataCoSupplyChainDataset.csv) using pandas to clean inconsistencies, handle missing values, and engineer critical features such as Order Processing Time, Delivery Delay, and Profitability Flag for in-depth performance analysis.
Exploratory Data Analysis (EDA) & KPI Development: Conducted extensive EDA using pandas, matplotlib, and seaborn to derive key business performance indicators (KPIs), including total orders, late delivery rates, and profit distribution, providing a foundational understanding of operational efficiency and areas for improvement.
Bottleneck Identification & Root Cause Analysis: Utilized matplotlib and seaborn to visualize and identify critical bottlenecks across various categorical dimensions (e.g., Order Region, Shipping Mode, Customer Segment) and pinpointed top drivers of late deliveries, enabling targeted strategic interventions.
Time-Based Performance Trend Analysis: Performed temporal analysis on delivery delays by month, day of week, and hour using pandas, matplotlib, and seaborn to uncover seasonality and daily patterns, informing optimized scheduling and resource allocation strategies to mitigate future delays.
