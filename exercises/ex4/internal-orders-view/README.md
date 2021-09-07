# Create Internal Orders View

<br>![](/exercises/ex2/images/create_in_repository_explorer.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_01.png)
<br>![](/exercises/ex4/images/create_internal_orders_ads_02.png)

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
