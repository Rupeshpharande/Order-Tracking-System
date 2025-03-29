# Order Tracking System

## Project Overview  
The **Order Tracking System** is a Java-based application that leverages JDBC for database connectivity and MySQL for data management. This system efficiently handles different user roles—**Admin, Supplier, and Customer**—each with specific functionalities. It provides a comprehensive solution for managing orders, products, and user interactions, including **real-time order tracking, product management, and role-based access control**.

## Features  

### Admin  
- Full access to manage **customers, suppliers, products, and orders**.  

### Supplier  
- Add and delete products.  
- Change order statuses.  
- View total orders.  

### Customer  
- Purchase products.  
- Check order details.  
- View previous orders.  

## Database  

### Database Management System  
- **MySQL**  

### Triggers Implemented  
- **Order Count Update**:  
  - Automatically increments the total order count when a customer buys a product.  
  - Decrements the total order count when a product is deleted.  

## Technologies  

- **Programming Language**: Java  
- **Database Connectivity**: JDBC (Java Database Connectivity)  
- **Database**: MySQL  

## Usage  

- **Admin**: Log in with admin credentials to manage all aspects of the system.  
- **Supplier**: Log in to add or remove products, manage order statuses, and view total orders.  
- **Customer**: Log in to purchase products, view current and past order details.  

## Database Schema  

### Customer  
Stores customer information:  
- **id** (Primary Key)  
- **name**  
- **phone_number**  
- **address**  
- **total_orders**  

### OrderDetails  
Stores order details:  
- **order_id** (Primary Key)  
- **customer_id** (Foreign Key referencing Customer)  
- **product_id** (Foreign Key referencing Product)  
- **delivery_date**  
- **order_status**  

### Product  
Stores product details:  
- **product_id** (Primary Key)  
- **name**  
- **price**  
- **supplier_id** (Foreign Key referencing Supplier)  

### Supplier  
Stores supplier details:  
- **supplier_id** (Primary Key)  
- **name**  
- **contact_info**  

---

This system ensures efficient **order management, product tracking, and user role-based functionalities**, making it a **reliable and scalable solution** for order tracking needs.
