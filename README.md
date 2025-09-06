# Onsite-Bookstore-Management-System-SQL-Final-Project-
A complete relational database project for a physical bookstore that manages inventory, authors &amp; categories, customers, and sales/transactions—from schema design to sample data and analytical queries.
# 🧭 Project Overview
Scenario: Local walk‑in bookstore; cash/PoS purchases.
Goals:
  Manage book inventory
  Track authors & categories
  Maintain customer records
  Record sales & line items, report KPIs
  Deliverables:
  Schema (bookstore)
  6 normalized tables with PK/FK/constraints
  ≥ 40 authors, 10 categories, 40 books, 40 customers
  ≥ 40 sales with sale items
  Query suite for reporting & insights
# 🗂️ Repository Structure
# bookstore-sql/
  ├─ /sql/
  │ ├─ 01_create_schema.sql
  │ ├─ 02_create_tables.sql
  │ ├─ 03_constraints_indexes.sql
  │ ├─ 04_seed_authors_categories.sql
  │ ├─ 05_seed_books.sql
  │ ├─ 06_seed_customers.sql
  │ ├─ 07_seed_sales_and_items.sql
  │ └─ 08_reporting_queries.sql
 # 🧱 Logical Model (Tables)
  authors: author_id (PK), author_name, country
  categories: category_id (PK), category_name (UNIQUE, NOT NULL)
  books: book_id (PK), book_name, author_id, category, price, stock
  customers: customer_id (PK), customer_name, email, sex,country
  sales: sale_id (PK) NOT NULL, customer_id, book_id, book_name, customer_name, quantity, price, total_amount, sale_date
  transactions: transaction_id (PK) NOT NULL, author_id (FK), book_id (FK), customer_id (FK), sales_id, category_id, customer_name, payment_method, payment_status, transaction_date
  # SQL PROJECT FILE
  Screenshots: <img width="1920" height="1080" alt="Screenshot (436)" src="https://github.com/user-attachments/assets/dd8edaef-cec1-4738-bb75-edbaecf8d083" />
