 Data Analyst Internship — Task 7  
Get Basic Sales Summary from a Tiny SQLite Database using Python
 Objective
This project demonstrates how to connect Python to an SQLite database, run simple SQL queries to get total sales and revenue, and visualize the results using matplotlib.

---
Tools & Technologies
- Python
- SQLite (sqlite3 module)
- pandas
- matplotlib

---
 Dataset
The project uses a small SQLite database file named `sales_data.db` containing a single table:  
`sales(product TEXT, quantity INTEGER, price REAL)`

---
 Steps Performed
1. Created an SQLite database `sales_data.db` and added a simple `sales` table.  
2. Connected to the database using `sqlite3.connect()`.  
3. Executed the SQL query:
   ```sql
   SELECT product, 
          SUM(quantity) AS total_qty, 
          SUM(quantity  price) AS revenue
   FROM sales
   GROUP BY product;# SQLite_Sales_Summary_Analysis
A simple Python-based data analysis project that connects to an SQLite database, retrieves basic sales summaries using SQL, and visualizes the results using Matplotlib.
