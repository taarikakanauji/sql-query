# SQL Query Practice Repository


## Overview

This repository contains a comprehensive set of SQL query exercises and practical examples using a sample sales database. The dataset includes multiple tables representing a typical business scenario with customers, products, sales, returns, and territories.


## Dataset Overview

The database consists of the following tables:

- `calendar_lookup`
- `customer_lookup`
- `product_categories_lookup`
- `product_lookup`
- `product_subcategories_lookup`
- `returns_data`
- `sales_data`
- `territory_lookup`

## Table Descriptions

    
### `calendar_lookup`

Contains date values used for filtering and date-based analysis.

| Column | Description   |
|--------|----------------|
| Date   | Calendar date |

---

### `customer_lookup`

Holds customer demographic and personal data.

| Column         | Description                    |
|----------------|--------------------------------|
| CustomerKey    | Unique customer identifier     |
| Prefix         | Title (Mr./Ms./Mrs.)           |
| FirstName      | Customer's first name          |
| LastName       | Customer's last name           |
| BirthDate      | Date of birth                  |
| MaritalStatus  | Marital status (S/M)           |
| Gender         | Gender (M/F)                   |
| EmailAddress   | Customer's email               |
| AnnualIncome   | Annual income in USD           |
| TotalChildren  | Number of children             |
| EducationLevel | Education level                |
| Occupation     | Occupation type                |
| HomeOwner      | Home ownership status (Y/N)    |

---

### `product_categories_lookup`

Defines top-level product categories.

| Column             | Description                 |
|--------------------|-----------------------------|
| ProductCategoryKey | Unique ID for category      |
| CategoryName       | Category name (e.g., Bikes) |

---

### `product_subcategories_lookup`

Subcategories under each product category.

| Column              | Description                      |
|---------------------|----------------------------------|
| ProductSubcategoryKey | Unique ID for subcategory       |
| SubcategoryName     | Subcategory name (e.g., Road Bikes) |
| ProductCategoryKey  | Foreign key to product category  |

---

### `product_lookup`

Details of individual products including pricing, style, and sizing.

| Column             | Description                      |
|--------------------|----------------------------------|
| ProductKey         | Unique product ID                |
| ProductSubcategoryKey | Link to subcategory            |
| ProductSKU         | Stock Keeping Unit               |
| ProductName        | Product name                     |
| ModelName          | Model name                       |
| ProductDescription | Detailed product description     |
| ProductColor       | Product color                    |
| ProductSize        | Product size                     |
| ProductStyle       | Style (e.g., U = Unisex)         |
| ProductCost        | Cost price                       |
| ProductPrice       | Selling price                    |

---

### `returns_data`

Tracks products returned by customers.

| Column       | Description                |
|--------------|----------------------------|
| ReturnDate   | Date of return             |
| TerritoryKey | Region of return           |
| ProductKey   | Returned product           |
| ReturnQuantity | Quantity returned         |

---

### `sales_data`

Captures daily sales transactions.

| Column         | Description                       |
|----------------|-----------------------------------|
| OrderDate      | Date of the order                 |
| StockDate      | Date the item was stocked         |
| OrderNumber    | Unique order number               |
| ProductKey     | Sold product ID                   |
| CustomerKey    | Customer who placed the order     |
| TerritoryKey   | Region where the sale occurred    |
| OrderLineItem  | Order line item                   |
| OrderQuantity  | Quantity sold                     |

---

### `territory_lookup`

Information about sales territories across the globe.

| Column            | Description           |
|-------------------|-----------------------|
| SalesTerritoryKey | Unique region ID      |
| Region            | Sales region name     |
| Country           | Country               |
| Continent         | Continent             |

---

## Use Cases

This dataset is used for practice:

- SQL Joins (INNER, LEFT, RIGHT)
- Aggregations (SUM, COUNT, AVG)
- Filtering with WHERE, BETWEEN, IN
- Subqueries
- Grouping by time
- Data exploration and data cleaning
- Analytical functions (RANK etc.)


# **Project Resources:**  

### **SQL Query**  
[Insights of Sports Products Tracker Analysis](https://github.com/taarikakanauji/sql-query/blob/main/SQL%20Query.docx)  

### **Dataset Folder**  
[Dataset Files](https://github.com/taarikakanauji/sql-query/tree/main/dataset)  

### **Project README (Setup Guide)**  
[README.md](https://github.com/taarikakanauji/sql-query/blob/main/README.md)  



