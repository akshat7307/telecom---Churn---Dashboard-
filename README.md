# Telecom Customer Churn Analysis

Project Objective

The objective of this project is to analyze customer churn in a telecom company and understand the factors that may be related to customers leaving the company.

In this project, I worked on the complete data analytics process — starting from data cleaning using Python, storing and querying the data using SQL Server, and finally creating an interactive dashboard in Tableau.

---

Project Structure

Telecom-Customer-Churn/
│
├── data/                  # Raw dataset
├── python/                # Python files/notebooks for data cleaning
├── sql/                   # SQL queries and database scripts
├── tableau/               # Tableau dashboard/workbook
├── README.md              # Project documentation
└── requirements.txt       # Python libraries used

---

Problem Statement

Customer churn is an important problem for telecom companies because losing existing customers can affect revenue and business growth.

The main purpose of this project is to answer questions such as:

- How many customers have churned?
- What is the overall churn rate?
- Which contract types have higher churn?
- Does internet service type affect customer churn?
- Which payment methods are commonly used by customers?
- How does customer tenure relate to churn?
- Which customer groups have higher churn rates?
- What are the differences between customers who stayed and customers who churned?

---

What I Did in This Project

1. Data Cleaning Using Python

I used Python and Pandas to prepare the raw telecom customer data for analysis.

The main steps included:

- Loading the raw dataset
- Checking the structure and data types
- Handling missing and incorrect values
- Removing unnecessary columns
- Cleaning and standardizing the data
- Converting columns into the required data types
- Preparing the final dataset for SQL Server

---

2. Data Storage and Analysis Using SQL Server

After cleaning the data, I stored the prepared data in SQL Server.

I used SQL to:

- Create database tables
- Load the cleaned data
- Query customer information
- Calculate important business metrics
- Group customers based on different categories
- Analyze churn across different customer segments

---

3. Dashboard Creation Using Tableau

The final dataset was connected to Tableau to create an interactive dashboard.

The dashboard was used to analyze:

- Total customers
- Churned customers
- Churn rate
- Customer tenure
- Contract type
- Internet service
- Payment method
- Monthly charges
- Customer segments

The dashboard helps in understanding the major patterns in customer churn in a visual and easier way.

---

Skills and Tools Used

Python

- Pandas
- Jupyter Notebook
- Data Cleaning
- Data Transformation
- Exploratory Data Analysis

SQL Server

- SQL
- Data Storage
- Data Cleaning/Validation
- Aggregation
- Filtering
- Grouping
- Business Queries

Tableau

- Data Connection
- Data Visualization
- Interactive Dashboard
- Charts and KPIs
- Filters and Segmentation

---

Project Outcome

This project helped me understand how different tools can be connected to build a complete data analytics workflow.

The overall workflow was:

Raw Data
   ↓
Python
(Data Cleaning & Transformation)
   ↓
SQL Server
(Data Storage & Analysis)
   ↓
Tableau
(Data Visualization)
   ↓
Business Insights

Instead of analyzing the raw dataset directly, I created a process where the data was cleaned first, stored in a database, analyzed using SQL, and then presented through a Tableau dashboard.

---

Final Insights

Some of the important observations from the analysis include:

- Customer churn is not equally distributed across all customer groups.
- Contract type shows a noticeable difference in customer churn.
- Customers with shorter-term contracts show different churn behavior compared with customers having longer-term contracts.
- Internet service type is also associated with differences in churn rates.
- Customer tenure can be useful for understanding customer retention.
- Monthly charges and payment methods provide additional information when comparing customers who churned with customers who stayed.

These insights can help a telecom company identify customer segments that may require more attention and improve customer retention strategies.

---

Conclusion

The analysis shows that customer churn is influenced by several customer and service-related factors rather than one single factor.

Customers with month-to-month contracts showed higher churn compared with customers on longer-term contracts. Churn also varied across internet service types, customer tenure, and payment methods. This suggests that customers with shorter commitments and certain service profiles may require more attention from the company.

Overall, the analysis can help the telecom company identify customer segments with higher churn and focus its retention efforts on those groups. The dashboard makes these patterns easier to monitor and compare, which can support better customer retention decisions.



---

Dashboard

Tableau dashboard screenshots will be added here.

<!-- Dashboard images will be added later -->


