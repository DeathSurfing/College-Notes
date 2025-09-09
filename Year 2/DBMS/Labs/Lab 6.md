___

You are managing a database for a retail store that sells various products. The database needs to keep track of products, categories, and orders. You are tasked with setting up the database tables with appropriate constraints to ensure data integrity.

## TASKS:

**Instructions**:

1. Insert the following categories into the Categories table:

o **Electronics**

o **Clothing**

o **Furniture**

2. Insert the following products into the Products table:

o **ProductName**: "Laptop", **Price**: 1200.00, **StockQuantity**: 50,

**Category**: Electronicso **ProductName7**: "T-Shirt", **Price**: 20.00, **StockQuantity**: 150,

**Category**: Clothing

3. Attempt to insert another product with the name "Laptop" into the

Products table.

4. 5. Insert an order for 3 units of "Laptop" into the Orders table.

Insert an order for 2 units of "T-Shirt" into the Orders table without

specifying the OrderDate.

6. 7. **Insert a new category** called "Books" into the Categories table.

**Insert a new product** into the Products table with the following details:

o **ProductName**: "Desk Chair"

o **Price**: 85.00

o **StockQuantity**: 30

o **Category**: Furniture

8. 9. **Insert a new product** called "Smartphone" into the Products table.

**Attempt to insert another product** with the same name "Smartphone" to observe the

UNIQUE constraint.

10. **Insert a new order** for 5 units of "Smartphone" into the Orders table.

11. **Try to insert an order** with a negative quantity (-3) to observe the CHECK constraint.

12. **Insert a new order** for 3 units of "Bookshelf" without specifying the OrderDate and

observe how the DEFAULT constraint sets the OrderDate.

13. **Insert a new order** for 1 unit of "Bookshelf" and specify a different OrderDate (e.g.,

'2024-09-01').

14. **Attempt to insert a new product** with a CategoryID that does not exist in the

Categories table to observe the FOREIGN KEY constraint.

15. **Insert a new order** for a product that does not exist in the Products table to see what

happens.

16. **Insert a new product** called "Gaming Laptop" with the following details:

• **Price**: 1500.00

• **StockQuantity**: -5 (This should fail due to the CHECK constraint)

• **Category**: Electronics

17. **Insert a new order** for 10 units of "Gaming Laptop" and leave the OrderDate

unspecified to use the DEFAULT constraint.](<# Retail Store Database Management Tasks

You are managing a database for a retail store that sells various products. The database needs to keep track of products, categories, and orders. You are tasked with setting up the database tables with appropriate constraints to ensure data integrity.

## Tasks

### Instructions:

1. **Insert the following categories into the Categories table:**
   - Electronics
   - Clothing
   - Furniture

2. **Insert the following products into the Products table:**
   - **ProductName**: "Laptop", **Price**: 1200.00, **StockQuantity**: 50, **Category**: Electronics
   - **ProductName**: "T-Shirt", **Price**: 20.00, **StockQuantity**: 150, **Category**: Clothing

3. **Attempt to insert another product** with the name "Laptop" into the Products table.

4. **Insert an order** for 3 units of "Laptop" into the Orders table.

5. **Insert an order** for 2 units of "T-Shirt" into the Orders table without specifying the OrderDate.

6. **Insert a new category** called "Books" into the Categories table.

7. **Insert a new product** into the Products table with the following details:
   - **ProductName**: "Desk Chair"
   - **Price**: 85.00
   - **StockQuantity**: 30
   - **Category**: Furniture

8. **Insert a new product** called "Smartphone" into the Products table.

9. **Attempt to insert another product** with the same name "Smartphone" to observe the UNIQUE constraint.

10. **Insert a new order** for 5 units of "Smartphone" into the Orders table.

11. **Try to insert an order** with a negative quantity (-3) to observe the CHECK constraint.

12. **Insert a new order** for 3 units of "Bookshelf" without specifying the OrderDate and observe how the DEFAULT constraint sets the OrderDate.

13. **Insert a new order** for 1 unit of "Bookshelf" and specify a different OrderDate (e.g., '2024-09-01').

14. **Attempt to insert a new product** with a CategoryID that does not exist in the Categories table to observe the FOREIGN KEY constraint.

15. **Insert a new order** for a product that does not exist in the Products table to see what happens.

16. **Insert a new product** called "Gaming Laptop" with the following details:
    - **Price**: 1500.00
    - **StockQuantity**: -5 (This should fail due to the CHECK constraint)
    - **Category**: Electronics

17. **Insert a new order** for 10 units of "Gaming Laptop" and leave the OrderDate unspecified to use the DEFAULT constraint.>)](<# MySQL Retail Store Database Tasks

## Database Schema Setup

First, create the database and tables with appropriate constraints:

```sql
-- Create the retail store database
CREATE DATABASE retail_store;
USE retail_store;

-- Create Categories table
CREATE TABLE Categories (
    CategoryID INT AUTO_INCREMENT PRIMARY KEY,
    CategoryName VARCHAR(100) NOT NULL UNIQUE
);

-- Create Products table
CREATE TABLE Products (
    ProductID INT AUTO_INCREMENT PRIMARY KEY,
    ProductName VARCHAR(255) NOT NULL UNIQUE,
    Price DECIMAL(10, 2) NOT NULL CHECK (Price > 0),
    StockQuantity INT NOT NULL CHECK (StockQuantity >= 0),
    CategoryID INT,
    FOREIGN KEY (CategoryID) REFERENCES Categories(CategoryID)
);

-- Create Orders table
CREATE TABLE Orders (
    OrderID INT AUTO_INCREMENT PRIMARY KEY,
    ProductID INT,
    Quantity INT NOT NULL CHECK (Quantity > 0),
    OrderDate DATE DEFAULT (CURRENT_DATE),
    FOREIGN KEY (ProductID) REFERENCES Products(ProductID)
);
```

## Task Solutions

### Task 1: Insert Categories

```sql
INSERT INTO Categories (CategoryName) VALUES 
    ('Electronics'),
    ('Clothing'),
    ('Furniture');

-- Verify categories were inserted
SELECT * FROM Categories;
```
![[Screenshot 2025-09-04 at 11.31.18 AM.png]]
### Task 2: Insert Products

```sql
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Laptop', 1200.00, 50, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics')),
    ('T-Shirt', 20.00, 150, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Clothing'));

-- Verify products were inserted
SELECT p.*, c.CategoryName 
FROM Products p 
JOIN Categories c ON p.CategoryID = c.CategoryID;
```
![[Screenshot 2025-09-04 at 11.31.36 AM.png]]
### Task 3: Attempt Duplicate Product Insert

```sql
-- This should fail due to UNIQUE constraint
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Laptop', 1500.00, 25, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics'));
-- Expected Error: Duplicate entry 'Laptop' for key 'ProductName'
```
![[Screenshot 2025-09-04 at 11.31.59 AM.png]]
### Task 4: Insert Order for Laptop

```sql
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Laptop'), 3);
```
![[Screenshot 2025-09-04 at 11.32.14 AM.png]]
### Task 5: Insert Order for T-Shirt (No OrderDate)

```sql
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'T-Shirt'), 2);

-- Verify orders were inserted (notice DEFAULT OrderDate)
SELECT o.*, p.ProductName 
FROM Orders o 
JOIN Products p ON o.ProductID = p.ProductID;
```
![[Screenshot 2025-09-04 at 11.32.32 AM.png]]
### Task 6: Insert Books Category

```sql
INSERT INTO Categories (CategoryName) VALUES ('Books');
```
![[Screenshot 2025-09-04 at 11.32.47 AM.png]]
### Task 7: Insert Desk Chair Product

```sql
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Desk Chair', 85.00, 30, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Furniture'));
```
![[Screenshot 2025-09-04 at 11.33.10 AM.png]]
### Task 8: Insert Smartphone Product

```sql
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Smartphone', 800.00, 75, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics'));
```
![[Screenshot 2025-09-04 at 11.32.47 AM.png]]
### Task 9: Attempt Duplicate Smartphone Insert

```sql
-- This should fail due to UNIQUE constraint
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Smartphone', 900.00, 50, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics'));
-- Expected Error: Duplicate entry 'Smartphone' for key 'ProductName'
```
![[Screenshot 2025-09-04 at 11.34.02 AM.png]]
### Task 10: Insert Order for Smartphone

```sql
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Smartphone'), 5);
```
![[Screenshot 2025-09-04 at 11.34.15 AM.png]]
### Task 11: Attempt Negative Quantity Order

```sql
-- This should fail due to CHECK constraint
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Laptop'), -3);
-- Expected Error: Check constraint 'orders_chk_1' is violated.
```
![[Screenshot 2025-09-04 at 11.34.25 AM.png]]
### Task 12: Insert Bookshelf and Order (Default OrderDate)

```sql
-- First, add a "Bookshelf" product
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Bookshelf', 150.00, 20, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Furniture'));

-- Insert order for 3 units of "Bookshelf" without specifying OrderDate
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Bookshelf'), 3);
```
![[Screenshot 2025-09-04 at 11.34.40 AM.png]]
### Task 13: Insert Order with Specific OrderDate

```sql
INSERT INTO Orders (ProductID, Quantity, OrderDate) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Bookshelf'), 1, '2024-09-01');
```
![[Screenshot 2025-09-04 at 11.35.12 AM.png]]
### Task 14: Attempt Insert with Invalid CategoryID

```sql
-- This should fail due to FOREIGN KEY constraint
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Mystery Item', 99.99, 10, 999);
-- Expected Error: Cannot add or update a child row: a foreign key constraint fails
```
![[Screenshot 2025-09-04 at 11.35.23 AM.png]]
### Task 15: Attempt Order for Non-existent Product

```sql
-- This should fail due to FOREIGN KEY constraint
INSERT INTO Orders (ProductID, Quantity) VALUES 
    (999, 2);
-- Expected Error: Cannot add or update a child row: a foreign key constraint fails
```
![[Screenshot 2025-09-04 at 11.35.33 AM.png]]
### Task 16: Attempt Gaming Laptop with Negative Stock

```sql
-- This should fail due to CHECK constraint
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Gaming Laptop', 1500.00, -5, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics'));
-- Expected Error: Check constraint 'products_chk_2' is violated.
```
![[Screenshot 2025-09-04 at 11.35.46 AM.png]]
### Task 17: Insert Gaming Laptop and Order

```sql
-- Insert Gaming Laptop with correct stock quantity
INSERT INTO Products (ProductName, Price, StockQuantity, CategoryID) VALUES 
    ('Gaming Laptop', 1500.00, 25, (SELECT CategoryID FROM Categories WHERE CategoryName = 'Electronics'));

-- Insert order for 10 units of "Gaming Laptop" without OrderDate
INSERT INTO Orders (ProductID, Quantity) VALUES 
    ((SELECT ProductID FROM Products WHERE ProductName = 'Gaming Laptop'), 10);
![[Screenshot 2025-09-04 at 11.35.58 AM.png]]```

## Final Verification Queries

```sql
-- View all categories
SELECT * FROM Categories;

-- View all products with their categories
SELECT p.ProductID, p.ProductName, p.Price, p.StockQuantity, c.CategoryName 
FROM Products p 
JOIN Categories c ON p.CategoryID = c.CategoryID;

-- View all orders with product names
SELECT o.OrderID, p.ProductName, o.Quantity, o.OrderDate 
FROM Orders o 
JOIN Products p ON o.ProductID = p.ProductID 
ORDER BY o.OrderID;
```
![[Screenshot 2025-09-04 at 11.36.08 AM.png]]
## Summary of Expected Constraint Violations

The following tasks should produce constraint violation errors:

- **Task 3**: UNIQUE constraint violation (duplicate "Laptop")
- **Task 9**: UNIQUE constraint violation (duplicate "Smartphone") 
- **Task 11**: CHECK constraint violation (negative quantity)
- **Task 14**: FOREIGN KEY constraint violation (invalid CategoryID)
- **Task 15**: FOREIGN KEY constraint violation (invalid ProductID)
- **Task 16**: CHECK constraint violation (negative StockQuantity)
