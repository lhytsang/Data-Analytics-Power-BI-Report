# Data-Analytics-Power-BI-Report


## Importing the Data
> This project was done on a Linux system so the processes used for some parts may differ.

For this task, there are four tables that we need to import:
- **Orders**: contains each order's details, including the order and shipping dates, the customer, store, product IDs and the quantity of each product ordered. Each order in the table is made up of an order of a single product type.
- **Products**: contains information about each product sold by the company, including the product code, name, category, cost price, sale price, and weight.
- **Stores**: contains information about each store, including the store code, store type, country, region, and address.
- **Customers**: contains information about the customers, including their full name, email, address, telephone and join date.

The **Orders** table was imported using Azure SQL Database credentials. The column *Card Number* was deleted to ensure data privacy and the 'Split Column' function was used to distinguish 
both *Order Date* and *Shipping Date* into corresponding columns of its dates and times. Rows with null or missing elements in the *Order Date* column were also deleted. 

The **Products** table was in the form of a .csv file, which was uploaded onto Google Drive before being imported into Power BI from the web. The 'Remove Duplcates' feature was used on the *product_code* column to ensure that there are no duplicates of the same product. 

Next, the **Stores** table was imported using Blob Storage and the columns *id*, *id2* and *id3* were removed.

The **Customers** table was in a folder file which was imported using 'Combine and Transform' function. A new column *Full Name* was created using the 'Column from Examples' feature to merge *First Name* and *Last Name* columns and the *First Name* and *Last Name* columns were then deleted.

For every table, the columns were renamed to align with Power BI naming conventions as well as for maintaining consistency. For example, *product_code* was changed into *Product Code*.
