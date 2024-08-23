# Data-Analytics-Power-BI-Report


## Importing the Data
This project was done on a Linux system so the 

Four tables in total needed to import, each in various conditions in multiple locations
- Orders: 
- Products:
- Stores:
- Customers:  

 Orders table was imported from Azure SQL Database credentials. deleted column [Card Number], used 'Split Column' function to distinguish 
[Order Date] and [Shipping Date] into columns of the dates and times, deleted columns that, removed any rows with null or missing elements in the [Order Date] column, renaming columns


Products table - dowloaded file, imported file from web, used 'Remove Duplcates' feature on [product_code] column, renaming columns

Stores table - accessed using Blob Storage, rename columns, removed [id], [id2] and [id3] columns

Customer table - imported folder then 'Combine and Transform', created new column using the 'Column from Examples' feature to merge [First Name] and [Last Name] columns, rename columns, deleted [First Name] and [Last Name] columns
