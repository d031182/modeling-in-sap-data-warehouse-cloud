# Exercise 1 - Upload CSV Files

## Upload CSV Files
In this exercise, we will learn how to bring data into SAP Data Warehouse Cloud, which is pre-requisites for all follow-up exercises. For that we will upload sample data with CSV file format, which you can download from https://github.com/d031182/reference-data-model-samples/tree/main/data/BIKE_SALES .

1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  ![Import CSV File](images/ImportCSVFile_2.png)
3. Select a source file, e.g. SalesOrders.csv, Products.csv, etc. 
4. Click on <b><i>Upload</i></b>
  ![Import CSV File](images/ImportCSVFile_3.png)
5. In this page you will have the options to wrangle and adopt the data to your needs, e.g.:
    - Change Data Types
    - Concatenate different columns into one
    - Replace NULL values with appropriate value of your choice
    - etc.
6. For our exercise it's good enough to click on the <b><i>Deploy</i></b> Button to move on.
  ![Import CSV File](images/ImportCSVFile_4.png)
7. Set the name of the table, which will be created to store the data. In our example please add a prefix <b>CSV_</b> to the CSV filename, e.g. <b><i>CSV_SalesOrders</i></b>.
8. The click again on the <b><i>Deploy</i></b> Button
  ![Import CSV File](images/ImportCSVFile_5.png)
9. Please repeat these steps for all other downloaded CSV files 


## Summary

You've now imported sample data, that is required for all follow up exercises.

Continue to - [Exercise 2 - Exercise 2 Description](../ex2/README.md)

