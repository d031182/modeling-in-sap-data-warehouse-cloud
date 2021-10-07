# Create Internal Orders View

1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
  <br><br>![](/exercises/ex1/images/create_in_repository_explorer.png)<br><br>
3. Drag and drop the table <b><i>CSV_VendorProductCategoryHierarchy</i></b> into the canvas
  <br><br>![](../images/create_internal_orders_ads_01a.png)
4. Select the Output Node in the canvas and configure the following properties:
    - Business Name: <b>V_INTERNAL_ORDERS</b>
    - Technical Name: <b>V_INTERNAL_ORDERS</b>
    - Semantic Usage: <b>Analytical Dataset</b>
    - Expose for Consumption: <b>ON</b>
    <br><br>![](../images/create_internal_orders_ads_02.png)

5. Select the <i>Output Node</i> and change the following columns into measures:<b>
  - NETAMOUNT
  - GROSSAMOUNT
  - TAXAMOUNT
  - QUANTITY</b>
  <br><br>![](../images/create_internal_orders_ads_02a.png)

6. Click on the **CSV_InternalOrders Node** and add a **Projection Node** from the context menu.
  <br><br>![](../images/create_internal_orders_ads_03.png)
  
7. Select the column **CREATEDAT** from the **Projection Node** and click on **Change Name**.
  <br><br>![](../images/create_internal_orders_ads_04.png)

8. Change the name of the column to **CREATE_DATE**.
  <br><br>![](../images/create_internal_orders_ads_04a.png)

### Create Associations
5. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br><br>![](../images/create_internal_orders_association_01.png)
6. Find a select the view <b>V_VENDOR_PRODUCTS</b>
<br><br>![](../images/create_internal_orders_association_02.png)

7. Map the column <b>V_INTERNAL_ORDERS.PRODUCTID</b> with the column <b>V_VENDOR_PRODUCTS.PRODUCTID</b>
<br><br>![](../images/create_internal_orders_association_03.png)

8. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br><br>![](../images/create_internal_orders_ads_05.png)

9. Find a select the view <b>V_EMPLOYEES</b>
<br><br>![](../images/create_internal_orders_ads_08.png)

10. Map the column <b>V_INTERNAL_ORDERS.EMPLOYEEID</b> with the column <b>V_EMPLOYEES.EMPLOYEEID</b>
<br><br>![](../images/create_internal_orders_ads_09.png)

11. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br><br>![](../images/create_internal_orders_ads_05.png)

12. Find a select the view <b>SAP.TIME.VIEW_DIMENSION_DAY (Time Dimension-Day)</b>
<br><br>![](../images/create_internal_orders_ads_10.png)

13. Map the column <b>V_INTERNAL_ORDERS.CREATEDAT</b> with the column <b>SAP.TIME.VIEW_DIMENSION_DAY.DATE_SQL</b>
<br><br>![](../images/create_internal_orders_ads_11.png)


### Deploy
15. Click on <b><i>deploy</i></b> button to deploy the view
<br><br>![](/exercises/ex4/images/create_internal_orders_ads_29.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_30.png)
