
DATA ANALYTICS INTERNSHIP REPORT
MINOR PROJECT
DATA ANALYTICS INTERNSHIP PROJECT
REPORT On E-Commerce Sales Performance Analysis

Submitted by
Name :Konjeti Venkata Sai Manidhar
Branch : Data Science

Submitted in partial fulfillment of the requirements for the completion of Data Analytics Internship.
ACKNOWLEDGEMENT
I express my sincere gratitude to my faculty members and the institution for providing me with the opportunity to complete this Data Analytics Internship project.

I would like to thank my faculty guide and mentors for their valuable guidance, encouragement, and support throughout the completion of this project.

This internship has provided me with practical knowledge of Data Analytics tools and techniques such as Advanced Excel, Oracle SQL Plus, and Tableau. The knowledge gained during this project helped me understand the process of data analysis, database management, and business visualization.

I also express my gratitude to everyone who directly or indirectly contributed to the successful completion of this project.
ABSTRACT
Data Analytics plays a significant role in modern businesses by converting raw information into meaningful insights that support effective decision-making. The E-Commerce Sales Performance Analysis project focuses on analyzing sales performance, customer purchasing behavior, product trends, and regional business performance.

This project demonstrates the complete data analytics process using Advanced Excel for data organization and cleaning, Oracle SQL Plus for database management and analytical queries, and Tableau for creating interactive visual dashboards.

Different SQL operations such as data retrieval, aggregation, grouping, ordering, and conditional statements are used to analyze sales information. The analytical results are represented through visual charts and dashboards to make business insights easier to understand.

The project helps organizations identify sales patterns, understand customer preferences, improve decision-making, and develop better business strategies.
TABLE OF CONTENTS
1. Introduction
2. Problem Statement
3. Objectives
4. Scope of the Project
5. Tools and Technologies Used
6. System Workflow
7. Database Design and Table Creation
8. Data Insertion and SQL Implementation
9. SQL Queries with Outputs
10. Tableau Dashboard Design
11. Results and Findings
12. Conclusion
13. Future Scope
14. References
1. INTRODUCTION
Data Analytics is the process of collecting, organizing, analyzing, and interpreting information to discover useful patterns and support better decision-making. In the modern business environment, organizations generate large amounts of information from various activities such as sales transactions, customer interactions, and market trends.

E-commerce businesses rely on data analytics to understand customer preferences, monitor sales performance, identify successful products, and improve overall business strategies. By converting business information into meaningful insights, companies can make accurate decisions and increase their growth.

The  E-Commerce Sales Performance Analysis  project focuses on understanding different aspects of sales performance through analytical techniques. It demonstrates the complete analytics workflow from data preparation and database management to querying and visual representation of results.

This project uses Advanced Excel for organizing and preparing information, Oracle SQL Plus for database operations and analytical queries, and Tableau for creating interactive dashboards. These tools help transform business information into easy-to-understand reports and visual insights.
2. PROBLEM STATEMENT
E-commerce organizations handle large amounts of sales information, making it difficult to manually identify important trends and business patterns. Without proper analytical techniques, businesses may face challenges in understanding customer behavior, product performance, and regional sales contributions.

The main problem addressed in this project is the need to convert raw business information into meaningful insights that can help management make better decisions regarding sales strategies, customer satisfaction, and business growth.
3. OBJECTIVES
The major objectives of this project are :
	To understand the process of e-commerce sales performance analysis.
	To organize and prepare business information using Advanced Excel.
	To perform data analysis and calculations using Oracle SQL Plus.
	To apply SQL queries for extracting meaningful business insights.
	To create interactive dashboards and visual reports using Tableau.
	To analyze sales trends, product performance, and customer purchasing behavior.
	To improve business decision-making through analytical reports.
4. SCOPE OF THE PROJECT
The scope of this project involves analyzing different factors that influence the performance of an e-commerce business. It includes studying sales trends, customer preferences, product performance, and regional comparisons.

The techniques used in this project can help organizations improve inventory planning, marketing strategies, customer relationship management, and overall business efficiency.

The concepts used in this project can also be expanded in the future by integrating real-time analytics, machine learning techniques, and advanced business intelligence solutions.
 5. TOOLS AND TECHNOLOGIES USED
5.1 Advanced Excel
Advanced Excel is used for organizing information, performing basic cleaning operations, applying formulas, and creating Pivot Tables for summary analysis.
 5.2 Oracle SQL Plus
Oracle SQL Plus is used for creating and managing database tables, inserting records, and executing SQL queries such as SELECT, GROUP BY, ORDER BY, and CASE statements to perform analytical operations.
5.3 Tableau
Tableau is a powerful data visualization tool used to create interactive charts, graphs, and dashboards. It helps in presenting complex analytical results in a simple and understandable format.
6. SYSTEM WORKFLOW
The complete workflow of the E-Commerce Sales Performance Analysis project is represented below :
      Data Collection
             |
             ↓
    Data Cleaning (Excel)
             |
             ↓
   Database Storage (Oracle SQL)
             |
             ↓
       SQL Analysis
             |
             ↓
  Data Visualization (Tableau)
             |
             ↓
      Business Insights

The above workflow explains how business information moves through different stages, starting from collection and preparation to analysis and final decision-making.
7. DATABASE DESIGN AND TABLE CREATION
One table is used in this project :
1. Ecommerce_Sales
7.1 Ecommerce_Sales Table Structure
Column Name	Description
Order_ID	Unique Order ID
Order_Date	Date of Order
Ship_Date	Date of Shipment
Ship_Mode	Shipping Mode
Customer_ID	Customer ID
Customer_Name	Customer Name
Segment	Customer Segment
Country	Country
City	City
State	State
Postal_Code	Postal_Code
Region	Sales Region
Product_ID	Product ID
Category	Product Category
Sub_Category	Product Sub-Category
Product_Name	Product Name
Sales	Sales Amount
Quantity	Quantity Sold
Discount	Discount
Profit	Profit
7.2 Oracle SQL Table Creation
CREATE TABLE Ecommerce_Sales(
Row_ID NUMBER,
Order_ID VARCHAR2(30),
Order_Date DATE,
Ship_Date DATE,
Ship_Mode VARCHAR2(30),
Customer_ID VARCHAR2(20),
Customer_Name VARCHAR2(100),
Segment VARCHAR2(30),
Country VARCHAR2(50),
City VARCHAR2(50),
State VARCHAR2(50),
Postal_Code NUMBER,
Region VARCHAR2(30),
Product_ID VARCHAR2(30),
Category VARCHAR2(30),
Sub_Category VARCHAR2(50),
Product_Name VARCHAR2(150),
Sales NUMBER(10,2),
Quantity NUMBER,
Discount NUMBER(5,2),
Profit NUMBER(10,2)
);
7.3 Dataset Description
Dataset Source : Sample Superstore Dataset (Kaggle)
Item	Value
Records	9,994
Columns	21
Format	CSV
Domain	Retail Sales
Important Fields :
	Order ID 
	Order Date 
	Customer Name 
	Product Name 
	Category 
	Sales 
	Profit 
	Region
8.Data Import and Preprocessing
The Sample Superstore dataset was downloaded from Kaggle in CSV format. The dataset contains 9,994 records and 21 columns related to customer orders, product information, sales, profit, shipping details, and regional data.
Before importing the dataset into Oracle SQL Plus, the data was cleaned and preprocessed using Microsoft Excel. After the cleaning process, the dataset was imported into the Oracle SQL database for performing SQL analysis and generating business insights.
8.1 Dataset Import Process
The cleaned Sample Superstore dataset was imported into Oracle SQL Plus for data analysis. Since the dataset already contained all the required records, manual SQL INSERT statements were not required.
The imported dataset was stored in the Ecommerce_Sales table and used for executing SQL queries.
8.2 Excel Data Cleaning Process
Before importing the dataset into Oracle SQL Plus, data cleaning and preprocessing were performed using Microsoft Excel.
The following activities were carried out:
	Removed duplicate records.
	Checked and handled missing values.
	Standardized date formats.
	Verified data consistency.
	Formatted numerical columns such as Sales, Profit, Discount, and Quantity.
	Created Pivot Tables for summary analysis. 
The cleaned dataset was then imported into Oracle SQL Plus for SQL analysis and Tableau dashboard development.
8.3 Original Dataset Screenshot
Figure 8.3 : Original Sample Superstore Dataset (CSV) before data cleaning and preprocessing.
 
8.4 Cleaned Dataset Screenshot
Figure 8.4 : Cleaned Sample Superstore Dataset after preprocessing in Microsoft Excel.
 
8.5 Pivot Table Analysis
Figure 8.5 : Pivot Table showing Total Sales by Product Category.
 
A Pivot Table was created in Microsoft Excel to summarize the total sales across different product categories. The analysis shows that Technology generated the highest sales (836,154.03), followed by Furniture (741,999.80) and Office Supplies (719,047.03). The overall sales recorded in the dataset were 2,297,200.86. This analysis helps in identifying the best-performing product categories and supports business decision-making.
9. SQL IMPLEMENTATION WITH OUTPUT
9.1 Total Sales by Category
Query :
SELECT
    Category,
    SUM(Sales) AS Total_Sales
FROM Ecommerce_Sales
GROUP BY Category
ORDER BY Total_Sales DESC;
Output :
 
9.2 Region-wise Sales Analysis
Query :
SELECT
    Region,
    SUM(Sales) AS Total_Sales
FROM Ecommerce_Sales
GROUP BY Region
ORDER BY Total_Sales DESC;
Output :
 
9.3 Top 10 Customers by Sales
Query :
SELECT *
FROM (
    SELECT
        Customer_Name,
        SUM(Sales) AS Total_Sales
    FROM Ecommerce_Sales
    GROUP BY Customer_Name
    ORDER BY Total_Sales DESC
)
WHERE ROWNUM <= 10;
Output :
 
9.4 Monthly Sales Analysis
Query :
SELECT
    TO_CHAR(Order_Date,'MON') AS Month,
    SUM(Sales) AS Monthly_Sales
FROM Ecommerce_Sales
GROUP BY TO_CHAR(Order_Date,'MON')
ORDER BY TO_CHAR(Order_Date,'MON');
Output :
 
9.5 Profit Analysis by Category
Query :
SELECT
    Category,
    SUM(Profit) AS Total_Profit
FROM Ecommerce_Sales
GROUP BY Category
ORDER BY Total_Profit DESC;
Output :
 
9.6 Top 10 Products by Sales
Query :
SELECT *
FROM (
    SELECT
        Product_Name,
        SUM(Sales) AS Total_Sales
    FROM Ecommerce_Sales
    GROUP BY Product_Name
    ORDER BY Total_Sales DESC
)
WHERE ROWNUM <= 10;
Output :
 
9.7 Discount Analysis
Query :
SELECT
    Discount,
    COUNT(*) AS Number_of_Orders,
    SUM(Sales) AS Total_Sales
FROM Ecommerce_Sales
GROUP BY Discount
ORDER BY Discount;
Output :

 
10. TABLEAU DASHBOARD DESIGN
The Tableau dashboard is designed to provide a visual representation of sales performance.
The dashboard contains :
	Bar Chart for sales comparison across regions.
	Line Chart for monthly sales trends.
	Pie Chart for category-wise sales distribution.
	Product performance chart.
	Filters for region, product category, and sales period.
	 
The dashboard helps management understand business performance quickly and make effective decisions.
11. RESULTS AND FINDINGS
After analyzing the sales information, the following findings were obtained :
	Technology category generated the highest sales revenue.
	Office Supplies maintained consistent sales across regions.
	Sales varied across different geographical regions.
	Discounts influenced the overall profitability of products.
	The Tableau dashboard provided better visualization of sales performance and business trends.
12. CONCLUSION
The E-Commerce Sales Performance Analysis project successfully demonstrates the use of Data Analytics techniques to understand business performance.
Advanced Excel was used for data preparation, Oracle SQL Plus was used for database operations and analysis, and Tableau was used for creating interactive dashboards.
The project helps in identifying sales trends, customer behavior, and profitable business areas, supporting better decision-making.
13. FUTURE SCOPE
Future enhancements of this project include :
	Integrating real-time sales monitoring systems.
	Applying machine learning models for sales 		prediction.
	Developing advanced interactive dashboards.
	Using artificial intelligence for automated business recommendations.
14. REFERENCES
	Oracle SQL Documentation.
	Microsoft Excel Documentation.
	Tableau Desktop Documentation
	Data Analytics and Business Intelligence learning materials.
	Sample Superstore Dataset (Kaggle)
