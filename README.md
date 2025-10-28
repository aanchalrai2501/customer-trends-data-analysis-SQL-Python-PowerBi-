Customer Shopping Behavior Analysis This project analyzes customer shopping behavior using a dataset of 3,900 purchases. The goal is to uncover trends in customer spending, segment customers, and identify key drivers of purchasing decisions. The insights from this analysis are used to provide actionable recommendations for marketing, product, and sales strategies.

Business Problem A retail company wants to better understand its customers' shopping habits to improve sales and customer loyalty. The company has noticed changes in purchasing patterns and wants to understand the factors driving these changes, such as discounts, reviews, and payment methods. The main business question is: "How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?".

Dataset The dataset contains 3,900 rows and 18 columns of customer transaction data. The key features include:

Customer demographics: Age, Gender, Location, and Subscription Status.

Purchase details: Item Purchased, Category, Purchase Amount, Season, Size, and Color.

Shopping behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, and Shipping Type.

Analysis and Findings The analysis was conducted using Python for data cleaning and feature engineering, SQL for querying and business insights, and Power BI for visualization.

🐍 Python: Data Preparation The initial data preparation was done using a Jupyter Notebook (Customer_Shopping_Behavior_Analysis.ipynb). The key steps included:

Loading the dataset using pandas.

Handling missing values in the Review Rating column by imputing the median rating for each product category.

Standardizing column names to snake_case for consistency.

Feature engineering to create an age_group column and a purchase_frequency_days column.

Checking for data consistency and removing redundant columns like promo_code_used.

Loading the cleaned data into a PostgreSQL database for SQL analysis.

💾 SQL: Answering Business Questions A series of SQL queries (customer_behavior_sql_queries.sql) were run to extract key business insights. Here are some of the questions addressed:

Revenue by Gender: Female customers generate slightly higher total revenue than male customers.

High-Spending Discount Users: A segment of customers who use discounts but still spend more than the average purchase amount was identified.

Top-Rated Products: The top 5 products with the highest average review ratings are Gloves, Sandals, Boots, Hat, and Skirt.

Shipping Type Comparison: Customers who opt for Express shipping spend slightly more on average than those who choose Standard shipping.

Subscribers vs. Non-Subscribers: Non-subscribers have a higher total revenue, but subscribers have a higher average spend.

📊 Power BI: Visualization An interactive dashboard (customer_behavior_dashboard.pbix) was created in Power BI to visualize the findings and allow for easy exploration of the data. The dashboard includes visualizations for:

Key metrics such as the total number of customers, average purchase amount, and average review rating.

Customer demographics and subscription status.

Revenue and sales by category and age group.

Business Recommendations Based on the analysis, the following recommendations are proposed:

Boost Subscriptions: Launch marketing campaigns to highlight the exclusive benefits for subscribers.

Customer Loyalty Programs: Implement a loyalty program to reward repeat customers and increase retention.

Review Discount Policy: Analyze the impact of discounts on profit margins and adjust the discount strategy to balance sales growth with profitability.

Product Positioning: Promote top-rated and best-selling products in marketing campaigns to attract new customers.

Targeted Marketing: Focus marketing efforts on high-revenue customer segments, such as certain age groups and express-shipping users.

How to Use Clone the repository:

Bash

git clone https://github.com/aanchalrai2501/customer-trends-data-analysis-sql-python-powerbi-.git Install the required libraries:

Bash

pip install pandas sqlalchemy psycopg2-binary Set up the database:

Make sure you have PostgreSQL installed and running.

Create a new database named customer_behavior.

Update the database connection details in the Customer_Shopping_Behavior_Analysis.ipynb notebook.

Run the Jupyter Notebook:

Open and run the Customer_Shopping_Behavior_Analysis.ipynb notebook to perform the data cleaning, feature engineering, and load the data into the PostgreSQL database.

Run the SQL queries:

Use a SQL client of your choice to connect to the customer_behavior database.

Run the queries in the customer_behavior_sql_queries.sql file to perform the analysis.

View the dashboard:

Open the customer_behavior_dashboard.pbix file in Power BI Desktop to view the interactive dashboard.

Tools Used Python: For data cleaning, feature engineering, and data loading.

Pandas: For data manipulation and analysis.

SQLAlchemy: For connecting to and interacting with the PostgreSQL database.

PostgreSQL: For data storage and SQL-based analysis.

Power BI: For creating the interactive dashboard and visualizing the data.

License This project is licensed under the MIT License. See the LICENSE file for details.
