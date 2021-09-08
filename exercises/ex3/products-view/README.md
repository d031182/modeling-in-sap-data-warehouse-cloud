# Create <i>Products</i> View


1. Navigate to the Repository Explorer
2. Click on <b><i>Create - Graphical View</i></b> Button to create a new view
   <br><br>![](/exercises/ex2/images/create_in_repository_explorer.png)
  
3. Drag and drop the table <b><i>CSV_Products</i></b> into the canvas
   <br><br>![](../images/create_products_dimension_01.png)
4. Select the Output Node in the canvas and configure the following properties:
    - Business Name: <b>V_PRODUCTS</b>
    - Technical Name: <b>V_PRODUCTS</b>
    - Semantic Usage: <b>Dimension</b>
    - Expose for Consumption: <b>ON</b>
    <br><br>![](/exercises/ex3/images/create_products_dimension_02.png)

5. Add a new <b>Text Association</b> from the <i>Association</i> section  
  <br><br>![](/exercises/ex3/images/create_products_dimension_04.png)

6. Find and select the view <b>V_PRODUCT_TEXTS</b>
  <br><br>![](/exercises/ex3/images/create_products_dimension_05.png)

7. Map the column <b>V_PRODUCTS.PRODUCTID</b> and column <b>V_PRODUCT_TEXTS.PRODUCTID</b>
  <br>![](/exercises/ex3/images/create_products_dimension_06.png)

8.dd
  <br>![](/exercises/ex3/images/create_products_dimension_07.png)
