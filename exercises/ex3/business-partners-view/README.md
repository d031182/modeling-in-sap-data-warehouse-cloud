
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
5. Drag and drop the table <b><i>CSV_Addresses</i></b> into the canvas and drop it directly on the CSV_BusinessPartners Node.
6. Select from the context menu <b>Join</b>
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_03.png)

7. A new <b>Join Node</b> and a <b>Projection Node</b> will created
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_04.png)

8. Select the <b>Join Node</b> and map the column <b>CSV_BusinessPartners.ADDRESSID</b> with the column <b>CSV_Addresses.ADDRESSID</b>
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_16.png)

9. Furthermore, you can adjust the **<i>Join Type</i>**. Following Join Types are currently supported:
    - Inner Join
    - Left Join
    - Right Join
    - Full Outer Join 
    - Cross Join
      <br><br>![](/exercises/ex3/images/create_business_partner_dimension_18.png)

10. You can also set the join cardinality:
    - Exactly One (1)
    - One (0..1)
    - Many (*)
  
    The cardinality information is utilized in SAP HANA Cloud to optimize the query execution and for that also the overall performance.
    <br><br>![](/exercises/ex3/images/create_business_partner_dimension_17.png)

### Projection Node
With the projection node, you can exclude or restore columns from your model. Hence, they won't be available nor consumpable on the client side, such as SAP Analytics Cloud. 

11. Select the **Projection Node** and exclude the **FAXNUMBER** from the Node. 
 <br><br>![](/exercises/ex3/images/create_business_partner_dimension_19.png)

  
### Id and Text
11. Select the <i>Output Node</i> and navigate to the <i>Attributes</i> section and click on <b>Edit Attriutes</b> button:
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_05.png)
12. Adjust the following attribute properties:
    - <b>COMPANYNAME</b>: set the semantic type to <b>TEXT</b>
    - <b>PARTNERID</b>: set the label to <b>COMPANYNAME</b>
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_06.png)

### Level Based Hierarchy
13. Select the *Output Node* and open the **Hierarchy** Dialog
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_07.png)
14. Add a new **Level Based Hierarchy**  
  <br>![](/exercises/ex3/images/create_business_partner_dimension_08.png)
  
15. Adjust the Hierarchy as following: 
   - Business Name: <b>Hierarchy</b>
   - Technical Name: <b>Hierarchy</b>
   - Levels: 
      - **REGION**
      - **COUNTRY**
      - **CITY**
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_09.png)
### Data Preview
16. Select the *Output Node* and click on **Data Preview** from the context menu.
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_10.png)
  
### Geo Spatial
17. Select the *Projection Node* and add a new **Calculation Node** from the context menu
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_11.png)
18. vrrfr  
  <br>![](/exercises/ex3/images/create_business_partner_dimension_12.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_13.png)
  <br>![](/exercises/ex3/images/create_business_partner_dimension_14.png)
### Deployment
15. Click on <b>Deploy</b> button to deploy the view
  <br><br>![](/exercises/ex3/images/create_business_partner_dimension_15.png)
