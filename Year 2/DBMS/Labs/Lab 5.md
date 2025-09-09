___
## Introduction:

Retail stores require efficient management of product inventories, categories, and customer orders to ensure smooth operation and accurate tracking. In this experiment, we designed a **Retail Store Database** consisting of three tables: `Categories`, `Products`, and `Orders`. The `Categories` table stores product categories, the `Products` table stores detailed product information including price and stock, and the `Orders` table records customer orders. Appropriate constraints (primary keys, foreign keys, NOT NULL, UNIQUE, CHECK) were applied to maintain data integrity and consistency throughout the database.

## Observations:

- The **Categories table** enforced unique category names and auto-incremented IDs.
    
- The **Products table** linked products to categories with `CategoryID` as a foreign key, ensuring that a product cannot exist without a valid category.
    
- The **Orders table** linked orders to products, ensuring orders reference valid products.
    
- The **Price and Stock fields** used CHECK constraints to prevent negative values.
    
- Data insertion was successful for categories, products, and orders without errors.
    
- Sample records were inserted and correctly linked, confirming relational integrity.
    

---

# Scenario
You are managing a database for a retail store that sell various products. The database needs to keep track of products, categories and orders. you are tasked with setting up the database tables with appropriate constraints to ensure data integrity


| CategoryID     | CateogryName | CategoryID  | CategoryName |
| -------------- | ------------ | ----------- | ------------ |
| Auto increment | Not NULL     | Primary Key | Unique       |


### Step 1:
#### Create Categories Table
```mysql
CREATE TABLE Categories (
    CategoryID INT AUTO_INCREMENT PRIMARY KEY,
    CategoryName VARCHAR(100) NOT NULL UNIQUE
);
```



#### Create Products Table
```mysql
CREATE TABLE Products (
    ProductID INT AUTO_INCREMENT PRIMARY KEY,
    ProductName VARCHAR(100) NOT NULL,
    Price DECIMAL(10, 2) NOT NULL CHECK (Price >= 0),
    Stock INT DEFAULT 0 CHECK (Stock >= 0),
    CategoryID INT NOT NULL,
    FOREIGN KEY (CategoryID) REFERENCES Categories(CategoryID)
);
```

#### Create Orders Table
```mysql
CREATE TABLE Orders (
    OrderID INT AUTO_INCREMENT PRIMARY KEY,
    OrderDate DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP,
    ProductID INT NOT NULL,
    Quantity INT NOT NULL CHECK (Quantity > 0),
    FOREIGN KEY (ProductID) REFERENCES Products(ProductID)
);
```

#### Seed values
```mysql
INSERT INTO Categories (CategoryName) VALUES
('Electronics'),
('Groceries'),
('Clothing'),
('Books'),
('Furniture');

INSERT INTO Products (ProductName, Price, Stock, CategoryID) VALUES
('Smartphone', 699.99, 50, 1),
('Laptop', 1099.00, 30, 1),
('Bananas', 0.59, 200, 2),
('T-shirt', 15.99, 100, 3),
('Novel: The Alchemist', 9.99, 80, 4),
('Office Chair', 89.99, 40, 5);

INSERT INTO Orders (ProductID, Quantity) VALUES
(1, 2),    -- 2 Smartphones
(3, 10),   -- 10 Bananas
(4, 3),    -- 3 T-shirts
(2, 1),    -- 1 Laptop
(6, 2);    -- 2 Office Chairs
```
![[Screenshot 2025-07-31 at 3.18.18 PM.png]]![[Screenshot 2025-07-31 at 3.18.25 PM.png]]![[Screenshot 2025-07-31 at 3.18.33 PM.png]]
## Conclusion:

In this experiment, we successfully created a Retail Store Database schema with proper relational table design and constraints. The database correctly handled products, categories, and orders with enforced data integrity via foreign keys, default values, and CHECK constraints. We inserted sample data into each table and verified successful relationships through consistent query results. This structure provides a strong foundation for more advanced retail data management and reporting.