# 👟 Nike Shoe Sales Database Project

This project is a relational database model simulating the end-to-end process of Nike shoe sales, from product sourcing to customer delivery. The database was created using **DBeaver**, a graphical database management tool, and includes all key business entities like suppliers, inventory, customers, orders, and shipments.

---

## 📌 Project Objective

The main goal of this project is to design and build a database that helps manage and track:
- Product inventory across warehouses
- Supplier-product relationships
- Customer orders and payment flows
- Shipment and delivery status

It reflects a real-world retail database structure used by e-commerce and logistics-driven companies like Nike.

---

## 🧱 Database Structure

The project contains 9 core tables, each serving a specific purpose in the sales pipeline:

### 1. **Warehouse**
Stores information about each warehouse where products are stocked.
- Key fields: Warehouse ID, Name, Location, Capacity

### 2. **Inventory**
Tracks available quantity of each product at each warehouse.
- Key fields: Inventory ID, Product ID, Warehouse ID, Stock Quantity

### 3. **Products**
Represents Nike shoe models with details like name, color, size, and price.
- Key fields: Product ID, Name, Category, Price, Supplier ID

### 4. **Supplier**
Contains data about companies or manufacturers supplying products.
- Key fields: Supplier ID, Name, Contact Info, Country

### 5. **Order Info**
Provides metadata about each order like order date and current status.
- Key fields: OrderInfo ID, Customer ID, Order Date, Status

### 6. **Orders**
Links specific products to specific orders.
- Key fields: Order ID, OrderInfo ID, Product ID, Quantity

### 7. **Customers**
Contains customer profiles for placing and tracking orders.
- Key fields: Customer ID, Name, Email, Address, Phone Number

### 8. **Payments**
Tracks financial transactions related to each order.
- Key fields: Payment ID, OrderInfo ID, Payment Method, Amount, Payment Date

### 9. **Shipment**
Handles delivery information and shipping status.
- Key fields: Shipment ID, OrderInfo ID, Carrier, Shipping Date, Delivery Status

---

## 🔄 How It Works (Workflow)

1. **Suppliers** deliver **Products** to **Warehouses**, where they are tracked in **Inventory**.
2. **Customers** place **Orders**, which are tied to multiple **Products** via **Order Info**.
3. Once an order is confirmed, a **Payment** is processed.
4. The order is prepared for **Shipment** and delivered to the customer.

---

## 🛠 How to Recreate the Project in DBeaver

If someone wants to recreate this project, they can follow these steps:

1. **Install DBeaver**  
   Download and install from [https://dbeaver.io/](https://dbeaver.io/)

2. **Connect to a Local Database**  
   (MySQL, PostgreSQL, SQLite, etc. — choose one during setup)

3. **Manually Create Tables**  
   Use DBeaver's **ER Diagram view** or SQL Editor to manually create the 9 tables listed above.

4. **Define Relationships**  
   Add foreign key constraints (e.g., Orders → Products, Payments → OrderInfo, etc.) via the UI.

5. **Populate Sample Data**  
   Add dummy data using DBeaver's spreadsheet-like data editor to simulate transactions.

6. **Visualize ERD**  
   Use DBeaver's **ERD tool** to generate a visual entity-relationship diagram automatically.

---

## 💡 Features

- Designed with a normalized schema to avoid redundancy
- End-to-end data flow from supply to delivery
- Ideal for SQL practice, analytics projects, or inventory simulations
- Platform-independent — can be recreated on any SQL-based system

---

## 🔮 Possible Extensions

- Add user roles (admin, customer, supplier)
- Integrate with analytics platforms (Tableau, Power BI)
- Add triggers for inventory depletion or auto restocking
- Build a simple front-end for order placement and tracking

---

## 📌 Final Note

This project was created manually using **DBeaver** without code or automation. It's ideal for learners or developers who want to understand the logic and structure of a real-world sales database through hands-on modeling.

---

## 🙋‍♂️ Author

**Your Name**  
📧 your.email@example.com  
📍 Based in [City, Country]  

---

