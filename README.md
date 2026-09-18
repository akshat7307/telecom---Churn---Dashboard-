# telecom---Churn---Dashboard-



# Customer Churn Analytics — Python, SQL Server & Tableau

I built this project to get practical experience with the complete data analytics workflow instead of working with Python, SQL, and Tableau as separate tools.

I started with a raw telecom customer dataset and worked through the process of cleaning and transforming the data in Python, organizing it in SQL Server, analyzing it with SQL, and finally building an interactive Tableau dashboard to present the findings.

The main focus of the project is customer churn — understanding how customer behavior, contracts, services, tenure, and billing are related to customers leaving the company.

---

Why I Built This Project
I wanted to build something where I could use the skills I had been learning together rather than creating a project around just one tool.
Instead of simply cleaning a dataset in Python or writing a few SQL queries, I wanted to understand what happens when a dataset goes through a complete analytics workflow.
I chose customer churn because it gives a good opportunity to look at different parts of a customer's journey — how long they stay, what services they use, what type of contract they have, how much they pay, and whether they eventually leave.
This also gave me the opportunity to think about the analysis from a business perspective rather than only focusing on the technical side.

Business Problem
For a telecom company, losing customers can directly affect recurring revenue. But knowing the number of customers who churned is only the starting point.
The more useful questions are:
Which types of customers are leaving?
Does contract type have any relationship with churn?
Does customer tenure differ between churned and retained customers?
Are certain services associated with different churn patterns?
How do monthly charges differ across customer groups?
Are there particular customer segments that deserve more attention?
I used these questions to guide the analysis instead of creating visualizations without a specific purpose.
What I Did
Data Preparation with Python
I started by loading the raw dataset into Python using Pandas.
Before doing any analysis, I went through the dataset to understand its structure and check whether the data was actually ready to use.
This included:
Checking the columns and data types
Looking for missing values
Checking inconsistent or invalid values
Converting columns into appropriate data types
Cleaning the data
Preparing the data for analysis
Creating fact and dimension tables
The main notebook is:
python/notebooks/Telecom-customer-churn.ipynb
I also used Python to connect the processed data to SQL Server and load the required tables.
Data Modeling
After cleaning the data, I separated the information into fact and dimension tables using a basic star-schema structure.
I did this because keeping everything in one large table makes the data harder to manage as the analysis becomes more complex.
The structured model also makes it easier to perform analysis in SQL and connect the data to Tableau.
SQL Server and SQL Analysis
I used SQL Server as the database layer for the project.
Once the data was loaded, I used SQL to answer the business questions I had identified earlier.
The analysis included areas such as:
Total customers
Churned customers
Churn rate
Churn by contract type
Churn by internet service
Customer tenure
Monthly charges
Total charges
Payment methods
Customer segments
Customer value
The SQL work is available in the sql/ folder.
I tried to keep the queries focused on actual business questions rather than writing queries simply to demonstrate SQL functions.
Tableau Dashboard
After completing the SQL analysis, I used Tableau to turn the results into an interactive dashboard.
The idea was to make the analysis easier to explore rather than presenting a collection of unrelated charts.
The dashboard covers:
Overall customer and churn KPIs
Churn by contract type
Churn by internet service
Customer tenure
Payment methods
Customer demographics
Monthly charges
Total charges
Customer segments
The Tableau workbook and dashboard screenshots are available in the tableau/ folder.
Key Visuals
I selected the visuals based on the type of question I was trying to answer.
KPI Cards
I used KPI cards for metrics such as total customers, churned customers, churn rate, average monthly charges, and average tenure.
These give a quick overview before moving into the detailed analysis.
Churn by Contract Type
I used a bar chart because the main purpose here is to compare churn across different contract categories.
This makes differences between month-to-month, one-year, and two-year contracts easy to see.
Churn by Internet Service
I used a category comparison to understand whether churn patterns differ between different internet service types.
Tenure Analysis
I included tenure analysis because customer lifetime is an important part of understanding retention.
It helps show how customer behavior differs between newer and longer-term customers.
Payment Method Analysis
I included payment methods to understand how they are distributed across customers and whether different payment groups show different churn patterns.
Monthly and Total Charges
I used charge-related visuals to understand customer billing and identify differences in customer value across segments.
Business Insights
The analysis helped me identify several patterns in the customer data, including:
Churn patterns differ across contract types.
Churn also varies across internet service categories.
Customer tenure shows noticeable differences between customer groups.
Billing levels vary across different customer segments.
Payment method usage is not evenly distributed across the customer base.
Customers who churned and customers who stayed show different characteristics across several dimensions.
These findings provide areas that a business could investigate further when thinking about customer retention.
I have treated these as relationships and patterns in the data, not as proof that one particular factor directly causes customers to churn.
Business Impact
The main value of the dashboard is that it brings different customer attributes together in one place.
Instead of looking at churn as a single percentage, a business analyst can use the dashboard to investigate which customer groups have different churn patterns and then decide where further investigation may be useful.
For example, if a particular customer segment shows a relatively high churn rate, the business could investigate that segment further and test targeted retention strategies.
The analysis can support areas such as:
Customer retention
Customer segmentation
Retention campaign planning
Contract strategy
Service-level analysis
Customer-value analysis
The dashboard itself does not claim to reduce churn because no real business intervention was performed as part of this project.
End-to-End Workflow
The complete workflow I followed was:
Raw Dataset
     ↓
Python
     ↓
Data Cleaning
     ↓
Data Transformation
     ↓
Data Modeling
     ↓
SQL Server
     ↓
SQL Analysis
     ↓
Tableau
     ↓
Interactive Dashboard
     ↓
Business Insights
This was the main reason for building the project: to understand how these different stages connect in a practical analytics workflow.
Tech Stack
Technology
How I Used It
Python
Data cleaning and transformation
Pandas
Data manipulation
Jupyter Notebook
Data preparation and exploration
SQL Server
Data storage and modeling
SQL
Business analysis
SQLAlchemy / pyodbc
Connecting Python with SQL Server
Tableau
Dashboard and visualization
GitHub
Version control and documentation
Data Source
The project uses the Telco Customer Churn Dataset.
The dataset contains information about telecom customers, including:
Customer demographics
Contract type
Internet service
Payment method
Tenure
Monthly charges
Total charges
Churn status
The dataset was originally provided through IBM's sample datasets and is publicly available for educational and analytical purposes.


