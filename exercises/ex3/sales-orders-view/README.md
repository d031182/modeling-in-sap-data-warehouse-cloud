# Create <i>Sales Orders</i> View

### Analytical Dataset
1. Navigate to the Repository Explorer
2. Click on **Create - Graphical View** button to create a new view
  <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)
3. Click on **Details** button and configure the following properties:
  - Business Name: **V_SALES_ORDERS**
  - Technical Name: **V_SALES_ORDERS**
  - Semantic Usage: **Analytical Dataset**
  - Expose for Consumption: **ON**
    <br><br>![](/exercises/ex3/images/create_sales_orders_ads_01.png)

### Join Node
3. Drag and drop the table **CSV_SalesOrderItems** into the canvas
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_02.png)
4. Drag and drop the table **CSV_SalesOrders** into the canvas and drop it on the *CSV_SalesOrderItems**
5. Create a new **Join Node** from the context menu 
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_03.png)
7. Map the column **CSV_SalesOrderItems.SALESORDERID** with the column **CSV_SalesOrders.SALESORDERID**
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_04.png)

### Filter Node
7. Select the *Projection Node* and add a new **Filter Node**
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_05.png)

8. Adjust the filter as the following:
    - Name: **Filter 1**
    - Expression: **SALESORG in ('EMEA', 'AMER')**
      <br><br>![](/exercises/ex3/images/create_sales_orders_ads_06.png)

### Data Preview 
9. Select the *Filter Node* and click on **Data Preview** from the context menu. Please check if the preview is showing the correct data for the defined filter.  
      <br><br>![](/exercises/ex3/images/create_sales_orders_ads_07.png) 
 
### Association
10. Select the *Output Node* and add a new **Association** from the *Association Section*. 
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_08.png)
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_09.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_10.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_11.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_12.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_13.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_14.png)


14. In the *Output Node* change the following attributes to **Measure**:
  - **GROSSAMOUNT**
  - **NETAMOUNT**
  - **TAXAMOUNT**
  - **QUANTITY**
    <br><br>![](/exercises/ex3/images/create_sales_orders_ads_15.png)
    <br><br>![](/exercises/ex3/images/create_sales_orders_ads_16.png)
  
15. Click on **Deploy** button to deploy the view. Please check the **Status** after successful deployment.
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_17.png)


