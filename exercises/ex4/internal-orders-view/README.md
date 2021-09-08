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

5. Click on the <b>Hierarchy</b> button 
  <br><br>![](/exercises/ex4/images/create_employee_dimension_04.png)
6. Add a new <b>Parent Child Hieararchy</b> (aka Internal Hierarchy)
  <br><br>![](/exercises/ex4/images/create_employee_dimension_05.png)
7. Adjust the following properties:
    - Business Name: <b>Employee Hierarchy</b>
    - Technical Name: <b>EMP_HIER</b>
    - Parent Column: <b>MANAGERID</b>
    - Child Column: <b>EMPLOYEEID</b>
  <br><br>![](/exercises/ex4/images/create_employee_dimension_06.png)
8. Select the Output Node in the canvas and click on <b>Data Preview</b> from the context menu
    <br><br>![](/exercises/ex4/images/create_employee_dimension_10.png)
9. Click on <b><i>deploy</i></b> button to deploy the view
  <br><br>![](/exercises/ex4/images/create_employee_dimension_08.png)







## Create Associations
<br>![](/exercises/ex4/images/create_internal_orders_ads_05.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_06.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_07.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_08.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_09.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_10.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_11.png)

## Create Calculated Measures - Currency Conversion
<br>![](/exercises/ex4/images/create_internal_orders_ads_12.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_13.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_14.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_13.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_15.png)

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

## Set Measures

<br>![](/exercises/ex4/images/create_internal_orders_ads_17.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_18.png)

## Deploy
<br>![](/exercises/ex4/images/create_internal_orders_ads_29.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_30.png)
