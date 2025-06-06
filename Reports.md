# 📊 Nike Shoe Sales Database – Analytical Reports

This file contains analytical reports developed for the Nike Shoe Sales Database. Each report answers a key business question using multi-table joins and aggregation logic. Visualizations can be added to complement these insights.

---

## 🧾 Report 1: Top-Spending Customers

**Purpose**: Identify the highest-value customers based on total amount spent and number of orders.

**Query Logic**:
- Join Customer, Order, Order_Info, and Product.
- Count orders and sum revenue (price × quantity).
- Group by customer.

**Insight**: Helps understand your most loyal and profitable customers.

---

## 🧾 Report 2: Best-Selling Product Categories

**Purpose**: Show which categories bring in the most revenue and sales volume.

**Query Logic**:
- Join Product and Order_Info.
- Group by product category.
- Sum quantity and revenue.

**Insight**: Guides inventory and marketing focus by top-performing categories.

---

## 🧾 Report 3: Revenue by Supplier

**Purpose**: Analyze supplier performance by total sales revenue of their products.

**Query Logic**:
- Join Supplier, Product, and Order_Info.
- Group by supplier name.
- Aggregate sales revenue (price × quantity).

**Insight**: Helps assess supplier impact and negotiate better deals.

---

## 🧾 Report 4: Current Stock Levels

**Purpose**: Show quantity on hand for each product and whether it's in stock.

**Query Logic**:
- Join Product and Inventory.
- Sum available quantities.
- Return “Not in Stock” for items with no inventory.

**Insight**: Critical for supply chain, restocking, and avoiding out-of-stock issues.

---

## 🧾 Report 5: Full Customer Order History

**Purpose**: Provide a CRM-friendly view of each customer's complete purchase history.

**Query Logic**:
- Join Customer, Order, Order_Info, and Product.
- Display customer name, product, order date, quantity, and total spent.

**Insight**: Useful for customer service, personalization, and loyalty campaigns.

---
