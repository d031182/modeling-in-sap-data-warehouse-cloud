# Create Internal Orders View

1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
  <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)<br><br>
3. Drag and drop the table <b><i>CSV_VendorProductCategoryHierarchy</i></b> into the canvas
  <br><br>![](../images/create_internal_orders_ads_01.png)
4. Select the Output Node in the canvas and configure the following properties:
    - Business Name: <b>V_INTERNAL_ORDERS</b>
    - Technical Name: <b>V_INTERNAL_ORDERS</b>
    - Semantic Usage: <b>Analytical Dataset</b>
    - Expose for Consumption: <b>ON</b>
    <br><br>![](../images/create_internal_orders_ads_02.png)

### Create Associations
5. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br>![](../images/create_internal_orders_ads_05.png)
6. Find a select the view <b>V_VENDOR_PRODUCTS</b>
<br>![](../images/create_internal_orders_ads_06.png)

7. Map the column <b>V_INTERNAL_ORDERS.PRODUCTID</b> with the column <b>V_VENDOR_PRODUCTS.PRODUCTID</b>
<br>![](../images/create_internal_orders_ads_07.png)

8. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br>![](/exercises/ex4/images/create_internal_orders_ads_05.png)


9. Find a select the view <b>V_EMPLOYEES</b>
<br>![](../images/create_internal_orders_ads_08.png)

10. Map the column <b>V_INTERNAL_ORDERS.EMPLOYEEID</b> with the column <b>V_EMPLOYEES.EMPLOYEEID</b>
<br>![](../images/create_internal_orders_ads_09.png

11. Select the <i>Output</i> node in the canvas and add a new association from the <i>Associations</i> section: 
<br>![](../images/create_internal_orders_ads_05.png


9. Find a select the view <b>Time Dimension</b>
<br>![](../images/create_internal_orders_ads_10.png)

13. Map the column <b>V_INTERNAL_ORDERS.PRODUCTID</b> with the column <b>V_VENDOR_PRODUCTS.PRODUCTID</b>
<br>![](../images/create_internal_orders_ads_11.png)

### Create Calculated Measures - Currency Conversion
<br>![](../images/create_internal_orders_ads_12.png)
<br>![](../images/create_internal_orders_ads_13.png)
<br>![](../images/create_internal_orders_ads_14.png)
<br>![](../images/create_internal_orders_ads_13.png)
<br>![](../images/create_internal_orders_ads_15.png)

```javascript
CONVERT_CURRENCY(
  "AMOUNT" => "NETAMOUNT", 
  "SOURCE_UNIT" => "CURRENCY", 
  "TARGET_UNIT" => 'EUR', 
  "CONVERSION_TYPE" => 'M', 
  "REFERENCE_DATE" => CURRENT_DATE, 
  "CLIENT" => '002', "SCHEMA" => 'ZST_WORKSHOP', 
  "ERROR_HANDLING" => 'set_to_null', 
  "STEPS" => 'shift,convert,round', 
  "PRECISIONS_TABLE" => 'V_TCURX', 
  "CONFIGURATION_TABLE" => 'V_TCURV', 
  "PREFACTORS_TABLE" => 'V_TCURF', 
  "RATES_TABLE" => 'V_TCURR')
```

<br>![](/exercises/ex4/images/create_internal_orders_ads_16.png)

### Set Measures

<br>![](/exercises/ex4/images/create_internal_orders_ads_17.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_18.png)

### Deploy
9. Click on <b><i>deploy</i></b> button to deploy the view
<br>![](/exercises/ex4/images/create_internal_orders_ads_29.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_30.png)
