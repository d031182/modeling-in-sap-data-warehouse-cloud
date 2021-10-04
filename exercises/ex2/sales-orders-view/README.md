# Create <i>Sales Orders</i> View

### Analytical Dataset
1. Navigate to the Repository Explorer
2. Click on **Create - Graphical View** button to create a new view
  <br><br>![](/exercises/ex1/images/create_in_repository_explorer.png)
3. Click on **Details** button and configure the following properties:
  - Business Name: **V_SALES_ORDERS**
  - Technical Name: **V_SALES_ORDERS**
  - Semantic Usage: **Analytical Dataset**
  - Expose for Consumption: **ON**
    <br><br>![](../images/create_sales_orders_ads_01.png)

### Join Node
3. Drag and drop the table **CSV_SalesOrderItems** into the canvas
  <br><br>![](../images/create_sales_orders_ads_02.png)
4. Drag and drop the table **CSV_SalesOrders** into the canvas and drop it on the *CSV_SalesOrderItems**
5. Create a new **Join Node** from the context menu 
  <br><br>![](../images/create_sales_orders_ads_03.png)
7. Map the column **CSV_SalesOrderItems.SALESORDERID** with the column **CSV_SalesOrders.SALESORDERID**
  <br><br>![](../images/create_sales_orders_ads_04.png)

### Filter Node
8. Select the *Projection Node* and add a new **Filter Node**
  <br><br>![](../images/create_sales_orders_ads_05.png)

9. Adjust the filter as the following:
    - Name: **Filter 1**
    - Expression: **SALESORG in ('EMEA', 'AMER')**
      <br><br>![](../images/create_sales_orders_ads_06.png)
      
10. Select the *Filter Node* and click on **Data Preview** from the context menu. Please check if the preview is showing the correct data for the defined filter.  
      <br><br>![](../images/create_sales_orders_ads_07.png) 
 
### Association
11. Select the *Output Node* and add a new **Association** from the *Association Section*. 
  <br><br>![](../images/create_sales_orders_ads_08.png)
12. Find a select the view **V_PRODUCTS**
  <br><br>![](../images/create_sales_orders_ads_09.png)
13. Map the column **V_SALES_ORDERS.PRODUCTID** with the column **V_PRODUCTS.PRODUCTID**
  <br><br>![](../images/create_sales_orders_ads_10.png)
14. Select the *Output Node* and add a new **Association** from the *Association Section*. 
  <br><br>![](../images/create_sales_orders_ads_08.png)
15. Find a select the view V_BUSINESS_PARTNERS
  <br><br>![](../images/create_sales_orders_ads_11.png)
16. Map the column **V_SALES_ORDERS.PARTNERID** with the column **V_BUSINESS_PARTNERS.PARTNERID**
  <br><br>![](../images/create_sales_orders_ads_12.png)
  
### Asscociating Time Dimension
  >:triangular_flag_on_post: **Note 4th-Oct-2021**: In order to use a time dimension in SAP Analytics Cloud, you must create your dimension by following the procedure at Creating Time Dimensions. Manually-created or other time dimensions may not function correctly.
>
>In addition, attributes in an analytical dataset that are mapped to a time dimension via an association must have technical names that respect the following naming conventions:
*_DATE for Date/Day level
*_CALMONTH for Month level
*_CALQUARTER for Quarter level
*_YEAR for Year level
  >https://help.sap.com/viewer/c8a54ee704e94e15926551293243fd1d/cloud/en-US/5aae0e95361a4a4c964e69c52eada87d.html

16a. Select the _Project Node_ and select the column **CREATDAT** to rename. 
  <br><br>![](../images/create_sales_orders_ads_20.png)
  
16b. Rename the column to **CREAT_DATE**. 
  <br><br>![](../images/create_sales_orders_ads_21.png)
  
17. Select the *Output Node* and add a new **Association** from the *Association Section*. 
  <br><br>![](../images/create_sales_orders_ads_08.png)
18. Find a select the view **SAP.TIME.VIEW_DIMENSION_DAY** (Time Dimension-Day)
  <br><br>![](../images/create_sales_orders_ads_13.png)
19. Map the column **V_SALES_ORDERS.CREATEDAT** with the column **SAP.TIME.VIEW_DIMENSION_DAY.DATE_SQL**
  <br><br>![](../images/create_sales_orders_ads_14.png)
  

### Measures
20. In the *Output Node* change the following attributes to **Measure**:
  - **GROSSAMOUNT**
  - **NETAMOUNT**
  - **TAXAMOUNT**
  - **QUANTITY**
    <br><br>![](../images/create_sales_orders_ads_15.png)
    <br><br>![](../images/create_sales_orders_ads_16.png)
  
21. Click on **Deploy** button to deploy the view. Please check the **Status** after successful deployment.
  <br><br>![](../images/create_sales_orders_ads_17.png)


