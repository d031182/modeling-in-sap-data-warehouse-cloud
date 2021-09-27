 # Create My Internal Orders View

1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
  <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)<br><br>
3. Drag and drop the view **_V_INTERNAL_ORDERS_** into the canvas, which you have created previously.
  >:mortar_board: **Note**: the properties and semantics from the previous view will be inherited to the new view, such as Measure classification, Attributes Semantics, etc. In the future also Input Parameters, Associations, Text and Hierarchy definitions will be reusable. 
  
  <br><br>![](../images/create_my_internal_orders_ads_02.png)
4. TBD :construction::construction::construction:
  <br><br>![](../images/create_my_internal_orders_ads_03.png)
5. Select the Output Node in the canvas and configure the following properties:
    - Business Name: <b>V_MY_INTERNAL_ORDERS</b>
    - Technical Name: <b>V_MY_INTERNAL_ORDERS</b>
    - Semantic Usage: <b>Analytical Dataset</b>
    - Expose for Consumption: <b>ON</b>
  <br><br>![](../images/create_my_internal_orders_ads_04.png)
  <br><br>![](../images/create_my_internal_orders_ads_05.png)
  
### Data Access Control
6. Navigate to the _Data Access Control_ section and add a new Data Access Control.
  <br><br>![](../images/create_my_internal_orders_ads_07.png)
  
7. Select the Data Access Control **DAC_COMPANYCODE**.
  <br><br>![](../images/create_my_internal_orders_ads_08.png)
  
8. By mapping the Data Access Control **DAC_COMPANYCODE.ALLOWED_VALUE** column to the **V_MY_INTERNAL_ORDERS.COMPANYCODE**, the view will be filtered by the Company Code with the user's allowed values.
  <br><br>![](../images/create_my_internal_orders_ads_09.png)
  <br><br>![](../images/create_my_internal_orders_ads_10.png)
  <br><br>![](../images/create_my_internal_orders_ads_11.png)
  <br><br>![](../images/create_my_internal_orders_ads_12.png)
