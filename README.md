# Product-sales-
//..Combining the tables to get product sales data. 
Hey there 👋
contains 3 tables:-
1.Order table
2.Product table
3.Customer 
...............here we go 🙏🤝
Preferrrable steps used:-
1.Cleaning of bad data.
2.Combining of data from  two tables using:-
   a.VLOOKUP
   b.INDEX and MATCH 
   c. XLOOKUP
Performed two tasks to complete these steps.



--------------- Task1: Cleaning the bad data:---------------

For orders table:

	- Eliminated duplicate 'order_id' to prevent double-counting in data analysis.

	- Converted the data type of 'product_id' from number to Text.

	- To address data entry issues, replaced the incorrect entries in the 'qty' field that end with "Q" and appended the corrected values as necessary.

	- Substituted any empty values in the 'qty' column with the text 'Not Available'.



For the products table:

	- Removed all the extra leading and trailing spaces in product_name using TRIM function).

	- splited the 'price (in Rs)' column at the '₹' symbol and extracted the numerical values. 

	  Renamed the columns completing this task.



For the customer table:

	- Converted all customer names to lowercase.

	- Copied all customer name values, then paste them permanently using 'Paste Special' -> 'Values'.





--------------- Task2: Merging Data---------------



Note: Ensure that the cell type is  'General'

1. Used the VLOOKUP() function to retrieve all the customer names that correspond to their respective 'customer_id' listed in the orders table.

2. Used the INDEX-MATCH() function to retrieve all the product names that correspond to their respective 'product_id' listed in the orders table.

3. Used XLOOKUP() to obtain the corresponding 'price (in Rs)' of the products listed in the orders table.

4. Created a new column named "total_price" in the orders table that calculates the product of 'qty' and 'price (in INR)'.
   

