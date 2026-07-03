# restaurant-ordering-system
# 🍽️ Restaurant Management System (Oracle PL/SQL)

## Project Overview
This project is a Restaurant Management System developed using Oracle SQL and PL/SQL. It demonstrates database design, table relationships, data manipulation, stored procedures, functions, anonymous PL/SQL blocks, and analytical SQL queries.
The system manages customers, staff, menu items, customer orders, order details, and payments while showcasing Oracle database programming concepts.

## Features
- Customer Management
- Staff Management
- Menu Management
- Order Processing
- Payment Management
- Automatic Order Placement using PL/SQL Procedure
- Order Total Calculation using PL/SQL Function
- Sales Analysis using Window Functions
## Database Tables

The project contains the following tables:
Table          Description 

 Customers      Stores customer information 
 Staff          Stores restaurant staff details 
 Menu           Stores food items and pices 
 Orders         Stores customer orders 
 Order Details  Order_Details  Stores ordered menu items 
Payments        Stores payment transactions 

## Technologies Used
 Oracle Database
 Oracle SQL
 PL/SQL
SQL Developer / VS Code Oracle SQL Extension

## Database Relationships

- One Customer can place many Orders.
- One Staff member can manage many Orders.
- One Order can contain many Order Details.
- One Menu item can appear in many Order Details.
- One Order has one Payment.

---

## Main SQL Operations

## Table Creation
The project creates:
 Customers
 Staff
 Menu
 Orders
 Order_Details
 Payments

using Oracle SQL `CREATE TABLE` statements with:

- Primary Keys
- Foreign Keys
- Constraints

---

## Sample Data

The project inserts sample records for:

- Customers
- Staff
- Menu Items
- Payments

using `INSERT INTO` statements.

---

## PL/SQL Features

### Anonymous Block

The anonymous PL/SQL block:

- Checks whether a menu item exists
- Retrieves the menu price
- Creates a new order
- Inserts order details
- Calculates subtotal
- Displays a success message using `DBMS_OUTPUT`

---

### Stored Procedure

##Procedure Name

Place_Order

Purpose:

- Creates a new order
- Retrieves food price
- Calculates subtotal
- Inserts records into Orders and Order_Details
- Automatically generates the next Order ID and Detail ID

Example:

```sql
EXEC Place_Order(1,1,1,2);
```

---

### Function

**Function Name**

```
Calculate_Total
```

Purpose:

Calculates the total amount for a specific order.

Example:

```sql
SELECT Calculate_Total(1)
FROM dual;
```

---

## Analytical SQL Queries

The project demonstrates Oracle Window Functions including:

### Customer Spending Ranking

Uses:

- SUM()
- RANK()

to rank customers based on total payments.

---

### Most Popular Menu Items

Uses:

- SUM()
- DENSE_RANK()

to determine the most ordered food items.

---

### Running Total of Payments

Uses:

- SUM() OVER()

to calculate cumulative sales.

---

### Daily Sales Ranking

Uses:

- GROUP BY
- RANK()

to rank daily sales performance.

---

## Learning Outcomes

This project demonstrates understanding of:

- Oracle SQL
- PL/SQL Programming
- Database Design
- Primary and Foreign Keys
- Stored Procedures
- Functions
- Anonymous Blocks
- Window Functions

## Author

**Name:** Sharell Jotie Manley

## Course: Database Programming (Oracle SQL & PL/SQL)

## Institution: University of Lay Adventists of Kigali (UNILAK)

---

## Conclusion

This project provides a complete demonstration of an Oracle PL/SQL Restaurant Management System. It integrates SQL and PL/SQL programming techniques to manage restaurant operations while applying database relationships, procedural programming, and analytical queries.
