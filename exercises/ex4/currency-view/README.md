# Create Currency Views

Date: 2021-09-22

As of today, SAP Analytics Cloud must not access any table directly in SAP Data Warehouse Cloud due to security boundaries.
That applies also for the currency conversion relevant tables such as **TUCRR (Rates)**, **TCURX (Precisions)**, **TCURV (Configurations)**, **TCURF (Prefactors)**.

As a intermediate workaround you have to wrap the tables as views and declare them in the usage of the Currency Conversion function, e.g.

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

**Please note that this will change in the upcomming releases**. There it is planned that Currency Conversion can be configured centrally per space. 
