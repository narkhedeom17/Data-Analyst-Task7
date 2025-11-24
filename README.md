# 🔥 Task 7 – Basic Sales Summary using SQLite & Python

## 📌 Overview
This project demonstrates how to connect Python with an SQLite database, run SQL queries, summarize sales data, and visualize results using a bar chart.  
The task involves creating a tiny sales database named **sales_data.db** and extracting simple sales insights.

---

## 🛠 Tools Used
- Python  
- sqlite3  
- pandas  
- matplotlib  
- Jupyter Notebook / .py file  

---

## 📂 Dataset (Created Inside Python)
A table named **sales** was created with:
- `product`
- `quantity`
- `price`

Sample data was inserted for Shirt, Shoes, and Watch.

---

## 🧠 Steps Performed
### ✔ 1. Connected to SQLite database  
### ✔ 2. Created a sales table  
### ✔ 3. Inserted sample data  
### ✔ 4. Executed SQL query  
### ✔ 5. Loaded results into pandas  
### ✔ 6. Displayed summary  
### ✔ 7. Generated a bar chart  

---

## 📊 SQL Query Used
```sql
SELECT 
    product,
    SUM(quantity) AS total_quantity,
    SUM(quantity * price) AS total_revenue
FROM sales
GROUP BY product;
