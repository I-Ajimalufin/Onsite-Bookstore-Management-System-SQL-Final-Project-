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
  Screenshots: 
  <img width="1920" height="1080" alt="Screenshot (410)" src="https://github.com/user-attachments/assets/c5dbac6b-df20-44c2-80c8-325f8adfe7b2" />
  <img width="1920" height="1080" alt="Screenshot (411)" src="https://github.com/user-attachments/assets/83b4f344-9684-4619-a035-b139bb6d1114" />
  <img width="1920" height="1080" alt="Screenshot (412)" src="https://github.com/user-attachments/assets/657c4ee5-895c-4cf1-bb05-f17b9b7472ad" />
  <img width="1920" height="1080" alt="Screenshot (413)" src="https://github.com/user-attachments/assets/871b1ede-cdd0-4db3-817b-26154ddad87f" />
  <img width="1920" height="1080" alt="Screenshot (414)" src="https://github.com/user-attachments/assets/d0793238-1409-4950-8d9d-33a46573d259" />
  <img width="1920" height="1080" alt="Screenshot (415)" src="https://github.com/user-attachments/assets/28d94f1b-601c-4042-85a4-5f934db1e411" />
  <img width="1920" height="1080" alt="Screenshot (416)" src="https://github.com/user-attachments/assets/6c653b04-b3b5-4d5c-bc15-de7df8a20905" />
  <img width="1920" height="1080" alt="Screenshot (417)" src="https://github.com/user-attachments/assets/d95376b0-3651-47fb-8d9b-4621672b4334" />
  <img width="1920" height="1080" alt="Screenshot (418)" src="https://github.com/user-attachments/assets/4b6a25fe-79ac-430e-a505-4677c1e54628" />
  <img width="1920" height="1080" alt="Screenshot (419)" src="https://github.com/user-attachments/assets/877df124-4c50-41a0-97f5-2236371933f0" />
  <img width="1920" height="1080" alt="Screenshot (428)" src="https://github.com/user-attachments/assets/5541c699-af61-40ce-bc6c-63a305fb3ab2" />
  <img width="1920" height="1080" alt="Screenshot (429)" src="https://github.com/user-attachments/assets/19f75815-028c-4509-9568-d23339fe7066" />
  <img width="1920" height="1080" alt="Screenshot (430)" src="https://github.com/user-attachments/assets/8a10fd4b-a99c-4a6c-aee1-5d5c5e38d4d5" />
  <img width="1920" height="1080" alt="Screenshot (431)" src="https://github.com/user-attachments/assets/8f77ad0a-310b-4d2c-a8de-96fd1cec7aa7" />
  <img width="1920" height="1080" alt="Screenshot (432)" src="https://github.com/user-attachments/assets/3271b65c-ab04-4421-9927-1e8f479f9279" />
  <img width="1920" height="1080" alt="Screenshot (433)" src="https://github.com/user-attachments/assets/e5b3f055-e921-4c42-8a46-dbe9c0b634c7" />
  <img width="1920" height="1080" alt="Screenshot (434)" src="https://github.com/user-attachments/assets/c005fd4e-b0ea-4835-bebc-5767e63b900b" />
  <img width="1920" height="1080" alt="Screenshot (435)" src="https://github.com/user-attachments/assets/4e31c9b2-d447-49b4-9501-bed3d792e6ce" />
  <img width="1920" height="1080" alt="Screenshot (436)" src="https://github.com/user-attachments/assets/27cc61f1-635f-4044-8564-c1aecf787609" />
  <img width="1920" height="1080" alt="Screenshot (437)" src="https://github.com/user-attachments/assets/b041ce15-3290-45f2-b55a-f3d88c509938" />
  <img width="1920" height="1080" alt="Screenshot (438)" src="https://github.com/user-attachments/assets/1a237338-f033-491d-9c1f-e9f8efa6c6c1" />
  <img width="1920" height="1080" alt="Screenshot (439)" src="https://github.com/user-attachments/assets/5006aa8f-4230-4490-a09d-694b26ea7066" />
  <img width="1920" height="1080" alt="Screenshot (440)" src="https://github.com/user-attachments/assets/c875a9fb-5227-49ab-981a-b5b8e1f1e55e" />
  <img width="1920" height="1080" alt="Screenshot (441)" src="https://github.com/user-attachments/assets/c8c6b96a-72eb-4aaf-ac72-2ee7ece0e75b" />
  <img width="1920" height="1080" alt="Screenshot (442)" src="https://github.com/user-attachments/assets/7ee7cd98-9c84-4a05-88a7-80653c8c40ea" />
  <img width="1920" height="1080" alt="Screenshot (444)" src="https://github.com/user-attachments/assets/8d16f67e-a58e-476b-8e57-bfdf005bb94d" />

