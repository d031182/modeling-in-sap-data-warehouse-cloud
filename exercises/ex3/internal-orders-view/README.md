 # Create Internal Orders View

1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
  <br><br>![](../images/internal_orders_view_00.png)<br><br>
3. Drag and drop the table **_CSV_InternalOrders_** into the canvas.
  <br><br>![](../images/internal_orders_view_01.png)

4. Select the Output Node in the canvas and configure the following properties:
  - Business Name: <b>V_INTERNAL_ORDERS</b>
  - Technical Name: <b>V_INTERNAL_ORDERS</b>
  - Semantic Usage: <b>Analytical Dataset</b>
  - Expose for Consumption: <b>ON</b>
  <br><br>![](../images/internal_orders_view_02.png)
5. Select the *Output Node* and change the following columns to **Measure**:
  - **GROSSAMOUNT**
  - **NETAMOUNT**
  - **TAXAMOUNT**
  - **QUANTITY**
  <br><br>![](../images/internal_orders_view_03.png)

6. Select the node _CSV_InternalOrders_ and add a new **Projection Node** from the context menu
  <br><br>![](../images/internal_orders_view_04.png)


7. Select the _Projection Node_ and change the name of the column **CREATEDAT** 
  <br><br>![](../images/internal_orders_view_05.png)
  
8. Set the new name to **CREATE_DATE**
  <br><br>![](../images/internal_orders_view_06.png)

6. Click on the **Deploy** button to deploy the view.
  <br><br>![](../images/internal_orders_view_07.png)
  <br><br>![](../images/internal_orders_view_08.png)


  




  
