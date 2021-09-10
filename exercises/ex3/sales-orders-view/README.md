# Create <i>Sales Orders</i> View
1. Navigate to the Repository Explorer
2. Click on Create - Graphical View Button to create a new view
  <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)

3. Drag and drop the table **CSV_SalesOrderItems** into the canvas
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_01.png)
  
4. Drag and drop the table **CSV_SalesOrders** into the canvas and drop it on the *CSV_SalesOrderItems**
5. Create a new **Join Node** from the context menu 
6. Map the column **CSV_SalesOrderItems.SALESORDERID** with the column **CSV_SalesOrders.SALESORDERID**
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_02.png)

7. Select the *Projection Node* and add a new **Filter Node**
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_04.png)

8. Adjust the filter as the following:
    - Name: **Filter 1**
    - Expression: **SALESORG in ('EMEA', 'AMER')**
      <br><br>![](/exercises/ex3/images/create_sales_orders_ads_05.png)
  

### Association

  <br>![](/exercises/ex3/images/create_sales_orders_ads_08.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_09.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_10.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_11.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_12.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_13.png)
  
  <br>![](/exercises/ex3/images/create_sales_orders_ads_06.png)
  <br>![](/exercises/ex3/images/create_sales_orders_ads_07.png)
12. Click on **Deploy** button to deploy the view
  <br><br>![](/exercises/ex3/images/create_sales_orders_ads_14.png)

