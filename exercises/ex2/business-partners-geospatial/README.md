
# Apply Geo Spatial on _Business Partners_ View
In this exercise we will apply Geo Spatial configuration on the view _**V_BUSINESS_PARTNERS**_. 

1. Navigate to the Repository Explorer
2. Search and open the view _**V_BUSINESS_PARTNERS**_
  <br><br>![](../images/create_business_partner_geospatial_01.png)

3. Click on **Details** button and configure the following properties:
    - Business Name: <b>V_BUSINESS_PARTNERS</b>
    - Technical Name: <b>V_BUSINESS_PARTNERS</b>
    - Semantic Usage: <b>Dimension</b>
    - Expose for Consumption: <b>ON</b>
   <br><br>![](../images/create_business_partner_dimension_01.png)
   

### Join Node
4. Drag and drop the table <b><i>CSV_BusinessPartners</i></b> into the canvas
  <br><br>![](../images/create_business_partner_dimension_02.png) 
5. Drag and drop the table <b><i>CSV_Addresses</i></b> into the canvas and drop it directly on the CSV_BusinessPartners Node.
6. Select from the context menu <b>Join</b>
  <br><br>![](../images/create_business_partner_dimension_03.png)

7. A new <b>Join Node</b> and a <b>Projection Node</b> will created


8. Select the <b>Join Node</b> and map the column <b>CSV_BusinessPartners.ADDRESSID</b> with the column <b>CSV_Addresses.ADDRESSID</b>
  <br><br>![](../images/create_business_partner_dimension_04.png)

9. Furthermore, you can adjust the **<i>Join Type</i>**. Following Join Types are currently supported:
    - Inner Join
    - Left Join
    - Right Join
    - Full Outer Join 
    - Cross Join
      <br><br>![](../images/create_business_partner_dimension_18.png)

10. You can also set the join cardinality:
    - Exactly One (1)
    - One (0..1)
    - Many (*)
  
    The cardinality information is utilized in SAP HANA Cloud to optimize the query execution and for that also the overall performance.
    <br><br>![](../images/create_business_partner_dimension_17.png)

### Projection Node
With the projection node, you can exclude or restore columns from your model. Hence, they won't be available nor consumpable on the client side, such as SAP Analytics Cloud. 

11. Select the *Projection Node* and **exclude** the **FAXNUMBER** from the Node. 
 <br><br>![](../images/create_business_partner_dimension_19.png)

  
### Id and Text
>**Id and Text**: Master Data usually consists an identifier (e.g. Cost Center Id) and a textual description (Cost Center Name). Depending on the reporting requirement, users might want to display one or the other (or both) in the story. This particular semantic and relation between an Id and Text can be modelled in SAP Data Warehouse Cloud.

11. Select the <i>Output Node</i> and navigate to the <i>Attributes</i> section and click on <b>Edit Attriutes</b> button:
  <br><br>![](../images/create_business_partner_dimension_05.png)
12. Adjust the following attribute properties:
    - <b>COMPANYNAME</b>: set the semantic type to <b>TEXT</b>
    - <b>PARTNERID</b>: set the label to <b>COMPANYNAME</b>
  <br><br>![](../images/create_business_partner_dimension_06.png)

### Level Based Hierarchy
13. Select the *Output Node* and open the **Hierarchy** Dialog
  <br><br>![](../images/create_business_partner_dimension_07.png)
14. Add a new **Level Based Hierarchy**  
  <br>![](../images/create_business_partner_dimension_08.png)
  
15. Adjust the Hierarchy as following: 
   - Business Name: <b>Hierarchy</b>
   - Technical Name: <b>Hierarchy</b>
   - Levels: 
      - **REGION**
      - **COUNTRY**
      - **CITY**
  <br><br>![](../images/create_business_partner_dimension_09.png)
### Data Preview
16. Select the *Output Node* and click on **Data Preview** from the context menu.
  <br><br>![](../images/create_business_partner_dimension_10.png)
  
### Geo Spatial
17. Select the *Projection Node* and add a new **Calculation Node** from the context menu
  <br><br>![](../images/create_business_partner_dimension_11.png)
18. Add a new **Geo-Coordinates Column**.
  <br><br>![](../images/create_business_partner_dimension_12.png)
19. Adjust the Calculated Column as following:
    - Business Name: **LOCATION**
    - Technical Name: **LOCATION**
    - Data Type: **hana.ST_GEOMETRY
    - Spatial Reference Identifier: **4326**
    - Latitude: **LATITUDE**
    - Longitude: **LONGITUDE** 
  <br><br>![](../images/create_business_partner_dimension_13.png)

### Deployment
15. Click on <b>Deploy</b> button to deploy the view
  <br><br>![](../images/create_business_partner_dimension_15.png)
