![dashboard](https://github.com/user-attachments/assets/5b40f0e1-37f3-4dd2-8cf3-7994700e28a1)

## 📚 Bookstore Sales Dashboard – Power BI Project
### 🔍 Overview
This Power BI project analyzes the performance of a fictional bookstore using customer, order, and book datasets. The dashboard provides insights into sales trends, customer behavior, top-selling books, and monthly performance to support data-driven decision-making.
________________________________________
### 📁 Datasets Used
File Name -	      Description

Books.csv -	Book ID, Title, Author, Genre, Price

Customers.csv -	Customer ID, Name, City, Join Date

Orders.csv -	Order ID, Customer ID, Book ID, Order Date
________________________________________
### 📊 Dashboard Highlights
•	Total Sales, Total Orders, Total Customers

•	Monthly Sales Trend (line chart from January to December)

•	Top 5 Best-Selling Books (bar chart)

•	Sales by Genre and Author

•	Customer Acquisition Trend

•	Repeat vs New Customers

• KPI Cards for:

o	Total Sales

o	Total Orders

o	Average Order Value (AOV)

o	Sales Last 30 Days

________________________________________
### 🧠 DAX Measures Used
Measure	DAX Logic

Total Sales :-	Total Sales = SUMX(Orders, Orders[Quantity] * RELATED(Books[Price]))

Total Orders :-	COUNTROWS(Orders)

Total Customers :-	DISTINCTCOUNT(Customers[Customer_ID])

Sales Last 30 Days :-	DATESINPERIOD()

Repeat Customers :-	Customer_IDs with COUNTROWS > 1

New Customers :-	Customer_IDs with COUNTROWS = 1

Full list of DAX measures is included in the project file.
________________________________________
### 🔗 Model Relationships
•	Orders[Customer_ID] → Customers[Customer_ID]

•	Orders[Book_ID] → Books[Book_ID]

•	Orders[Order_Date] → Date[Date] (Date table created with CALENDAR())
________________________________________
### 🛠 Tools & Skills Used
•	Power BI

o	Power Query for data cleaning

o	Data model design

o	DAX for calculated columns and measures

•	Excel (initial data inspection)

•	SQL (optional pre-processing)
________________________________________
### 🧾 How to Use
1.	Open the .pbix file in Power BI Desktop.
2.	Refresh the data if required.
3.	Use filters and slicers to explore performance by:
o	Month

o	City

o	Genre

o	Quarter
________________________________________
### 📌 Project Use Cases
•	Monitor bookstore performance

•	Understand customer purchase behavior

•	Identify high-performing genres/authors

•	Optimize inventory based on top-selling books

•	Track growth in new vs. repeat customers
________________________________________
### 📬 Contact
Built by a data analyst exploring customer behavior and retail analytics using Power BI.

https://www.linkedin.com/in/nikhil-kumar-3982a9348/


💬 Always happy to connect with fellow data enthusiasts and professionals!
