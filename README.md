Data Cleaning with PySpark – Orders Dataset
Overview
This project shows how to clean and transform an e‑commerce orders dataset using PySpark. The raw data is stored in Parquet format, and the script converts it into an analytics‑ready dataset by standardizing columns, creating new features, and filtering records.​

What this project does

Main steps in the script:
Read orders_data.parquet using a Spark session.​
Create a new column time_of_day from the order_date timestamp (morning, afternoon, evening; night orders are filtered out).
Cast order_date to DateType for easier date‑level analysis.​
Convert product and category values to lowercase and filter out products containing "tv".​
Parse purchase_address to extract a new purchase_state column.
Compute the number of distinct states as a simple data‑profiling check.
Write the cleaned output to orders_data_clean.parquet in overwrite mode.​

Tech stack
Python
Apache Spark (PySpark)
Parquet file format
