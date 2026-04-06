# ER-Diagram

# Instagram Thrift Store - ER Diagram

## About the Project

This ER diagram is designed for a small Instagram-based thrift and handmade store. The goal was to create a simple and practical database structure to manage products, customers, orders, payments, and delivery.

---

## What I Designed

I created the following main entities:

- **Customer** – stores user details like name, email, phone, and address
- **Order** – stores each order placed by a customer
- **Product** – stores all items (both thrift and handmade)
- **Order_Item** – connects orders and products (since one order can have multiple products)
- **Inventory** – keeps track of how many items are available
- **Payment** – stores payment details for each order
- **Shipping** – stores delivery and tracking information

---

## Key Points

- One customer can place multiple orders
- One order can contain multiple products
- Products and orders have a many-to-many relationship, handled using **Order_Item**
- Thrift items usually have quantity = 1, while handmade items can have more
- Payment and shipping are stored separately to keep things clean

---

## Why This Design

I tried to keep the design simple and realistic. Instead of putting everything in one table, I separated things like payment and shipping so it’s easier to manage and scale later.

---

## Final Thoughts

This design can handle a small business now and can also grow as the store gets bigger. It keeps the data organized and avoids duplication.

---
