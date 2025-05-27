# 📚 Online Book Store - SQL Project

## 📝 Project Summary

This project simulates an **Online Book Store Booking System** where customers can browse and order books online. It includes three main datasets represented as CSV files:

- **books.csv** — Contains book details like `book_id`, `title`, `author`, `genre`, `price`, and available stock.
- **customer.csv** — Contains customer data including `user_id`, `name`, `email`, and registration date.
- **order.csv** — Contains order records that link books and customers through `book_id` and `user_id`, along with order date and status.

The project structure ensures relational integrity by using **common columns with identical names and data types** across tables. This design supports effective JOIN operations, allowing for insightful queries such as total sales by book, order statuses, and customer activity.

This project offers hands-on practice in SQL fundamentals including table creation, data insertion, querying with joins, filtering, aggregation, and data analysis — ideal for learners and professionals polishing their SQL skills.

---

## 🗃️ Tables and Structure

### 1. `books.csv`
- `book_id` (INT) — Primary key
- `title` (VARCHAR)
- `author` (VARCHAR)
- `genre` (VARCHAR)
- `price` (DECIMAL)
- `stock_quantity` (INT)

### 2. `customer.csv`
- `user_id` (INT) — Primary key
- `name` (VARCHAR)
- `email` (VARCHAR)
- `registration_date` (DATE)

### 3. `order.csv`
- `order_id` (INT) — Primary key
- `book_id` (INT) — Foreign key referencing `books.book_id`
- `user_id` (INT) — Foreign key referencing `customer.user_id`
- `order_date` (DATE)
- `status` (VARCHAR) — e.g., Confirmed, Cancelled

---

## 🔗 Common Columns for JOINs

To ensure data consistency and enable relational queries, these tables share key columns:

- `book_id` connects `books.csv` and `order.csv`
- `user_id` connects `customer.csv` and `order.csv`

These common columns are of the same data type and column name, which facilitates efficient JOIN operations to combine data across tables for reports and analysis.

---

## 💡 Sample Queries and Use Cases

- List all orders made by a specific user.
- Calculate total sales revenue per book.
- Identify books currently out of stock.
- Retrieve customers who have never placed an order.
- Analyze the status of all bookings (confirmed, cancelled).

---

## 🚀 Getting Started

1. Import the CSV files into your preferred SQL database.
2. Create tables using the structure above, and load the CSV data.
3. Write SQL queries to practice joins, filters, aggregations, and subqueries.
4. Explore reporting use cases with the dataset.

---

Feel free to reach out if you want me to provide **SQL scripts**, **sample queries**, or help with anything else!

