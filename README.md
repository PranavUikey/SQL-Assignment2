# SQL-Assignment2
SQL Assignment for aiadventures Students


# About

Our chocolate sales database is organized into four primary tables: `geo`, `people`, `products`, and `sales`. Each table plays a crucial role in capturing and managing the data related to our chocolate sales operations. Below is a detailed description of each table and its purpose:


`Geo` Table

  *Purpose*: The geo table contains geographical information, which helps in identifying the locations where our sales activities are taking place. This includes information about countries and their respective time zones.

  *Key Columns*:
    `geo_id` (Primary Key): A unique identifier for each geographical location.
    `country_name`: The name of the country.
    `time_zone`: The time zone of the country.

`people` Table

  *Purpose*: The people table maintains records of our sales team members. It contains personal and professional details of each salesperson, enabling us to track and manage their performance.
  
  
  *Key Columns*:
    `salesperson` (Primary Key): The name of the salesperson.
    `spid` (Salesperson ID): A unique identifier for each salesperson.
    `team`: The team to which the salesperson belongs.
    `location` (Foreign Key): Links to the geo table to associate salespeople with their respective geographical locations.


`Products` Table
  
  *Purpose*: The products table lists all the different chocolate products we offer. This table is essential for managing inventory and understanding which products are performing well.
  
  *Key Columns*:
  
  `pid` (Primary Key): A unique identifier for each product.
  `product`: The name of the product.
  `category`: The category of the product (e.g., Dark Chocolate, Milk Chocolate, White Chocolate).
  `size`: The size of the product.
  `cost_per_box`: The cost per box of the product.
`Sales` Table

  *Purpose*: The sales table records all transactions made by our salespeople. It connects products, salespeople, and geographical data to provide a comprehensive view of our sales activities.
  
  *Key Columns*:
  `spid` (Foreign Key): References the salespeople table to identify who made the sale.
  `geo_id` (Foreign Key): References the geo table to indicate where the sale took place.
  `pid` (Foreign Key): References the products table to specify which product was sold.
  `sale_date`: The date when the sale occurred.
  `amount`: The total amount of the sale transaction.
  `customers`: The number of customers involved in the sale.
  `boxes`: The number of boxes sold.
  
This database structure allows us to efficiently track and analyze our sales performance across different products, regions, and sales personnel, providing valuable insights that drive our business decisions.

## Business Questions To Answer

1. Print details of `shipments (sales)` where `amount` is > 2,000 and `boxes` are <100.
2. How many `shipments (sales)` did each of the `sales persons` had in the month of `January 2022`?
3. Which product sells more `boxes`? `Milk Bars` or Eclairs?
4. Which product sold more `boxes` in the first 7 days of `February 2022`? `Milk Bars` or `Eclairs`?
5. Which `shipments (sales)` had under `100 customers` & under `100 boxes`? Did any of them occur on `Wednesday`?

6. What are the names of `salespersons` who had at least 1 shipment (sale) in the first 7 days of `January 2022`?
7. Which `salespersons` did not make any `shipments (sale)` in the first 7 days of `January 2022`?
8. How many times have we shipped more than 1000 `boxes` in each `month`?
9. Did we ship at least one box of `After Nines` to `New Zealand` on all the months?
10. `India` or `Australia`? Who buys more chocolate `boxes` on a monthly basis?


## All the best


