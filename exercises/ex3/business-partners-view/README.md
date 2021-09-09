
# Create <i>Business Partners</i> View

1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
  <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)

3. Drag and drop the table <b><i>CSV_BusinessPartners</i></b> into the canvas
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_01.png)
  
4. Select the Output Node in the canvas and configure the following properties:
    - Business Name: <b>V_BUSINESS_PARTNERS</b>
    - Technical Name: <b>V_BUSINESS_PARTNERS</b>
    - Semantic Usage: <b>Dimension</b>
    - Expose for Consumption: <b>ON</b>
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_02.png)

### Join Node
5. Drag and drop the table <b><i>CSV_Addresses</i></b> into the canvas 
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_03.png)

6. Create <i>Join Node</i> between CSV_BusinessPartners and CSV_Addresses
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_04.png)

### Id and Text
7. Select the <i>Output Node</i> and navigate to the <i>Attributes</i> section and click on <b>Edit Attriutes</b> button:
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_05.png)
8. Adjust the following attribute properties:
    - <b>COMPANYNAME</b>: set the semantic type to <b>TEXT</b>
    - <b>PARTNERID</b>: set the label to <b>COMPANYNAME</b>
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_06.png)

### Level Based Hierarchy
9. dwdw
  <br>![](/exercises/ex3/images/create_business_partner_dimension_07.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_08.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_09.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_10.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_11.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_12.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_13.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_14.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_15.png)
