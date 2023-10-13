# ETL-pipeline
 Design and implement an ETL (Extract, Transform, Load) pipeline using Python, SQL, and other data engineering technologies.



Designed and implemented an ETL (Extract, Transform, Load) pipeline using Python, SQL, and other data engineering technologies

#Steps for creation of ETL

1)Imported all the important modules
    import pandas as pd
      import sqlite3

2)Extracted the file Updated_sales_data.csv and converted it into a dataframe while making sure 
    If columns such as ('order_id' or 'product name' or 'price' or 'quantity' or 'Order Date') are null skip that row also log the issue
    If Price amount is negative then make it positive and log the issue
    If there is an error in loading the csv file then also return the error and logging the issue
3)Made 3 more columns in the dataframe namely ‘total sales’ by multiplying ‘Price Each’ and ‘Quantity Ordered’ , ‘month_of_purchase’ and ‘year_of_purchase’
4) Made a new Dataframe ‘df’  which aggregated the data for getting the total sales amount of each product for each product in each month .
5) Made a new Dataframe ‘sales_per_month’ indicating the monthly sales of all product.
6) Made a database test.db and made connections

7) Made 3 tables in that database namely ‘csv_table’,  ‘sales_per_month’ and ‘total_amount’ and copied all data from dataframe ‘data’, ‘sales_per_month’ and ‘df’ into it respectively, at the same time handling the issue while loading data into it and logging the issue

8) Writing sql code to get total sales amount for each product in the last quarter (last 3 months)
   
9)Writing sql code to get top 5 products by total sales amount for the entire dataset.

10)Writing sql code to get the monthly average sales for each product over the entire dataset.

