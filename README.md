# Modeling in SAP Data Warehouse Cloud
## Description

This repository aims to onboard new users into Modeling in SAP Data Warehouse Cloud in the most practical manner. For that you will build a real working data model, which will embrace specific features and functions. During the journey there will be additional tips and explanations on various modeling concepts.

## Overview

<b>"Learning by Doing"</b> is the main principle of this tutorial. Discover and understand the features and modeling concepts by putting your hands on the SAP Data Warehouse Cloud application and build a fully functioning data model yourself. 

The exercises are meant to be built in this particular order starting from basic concepts and diving step by step into deeper advanced features while processing with the exercises. The exercises are also based on each other. Hence, they prerequisite each other.



In general, you should be aware that SAP Data Warehouse is constantly delivering and updating features. That means, that some of the described features might be outdated and look differently than from your latest version (for that please also check regularly the "What's New" and the SAP Roadmaps in the links section). Nonetheless, I hope it still give you a solid understanding and insights into the fundamental modeling principles of SAP Data Warehouse Cloud.. 

And now enjoy the tutorial ;) 


## Requirements
Before you can start with the exercises, please make sure to get a running SAP Data Warehouse Cloud tenant with the latest updates.
For that you can apply for a **30-Days free Trial Tenant** under the following link:
- https://www.sap.com/products/data-warehouse-cloud/trial.html
- https://saphanajourney.com/data-warehouse-cloud/trial/

[![DWC_Free_Trial](/images/FreeDWCTrial.png)](https://saphanajourney.com/data-warehouse-cloud/trial/)


### SAP Data Warehouse Fundamentals
- [Exercise 1 - SAP Data Warehouse Cloud Fundamentals](exercises/ex1)
     - [Exercise 1.1 - Repository Explorer] - <b><i>under construction !!!</i></b>
     - [Exercise 1.2 - Data Source Browser] - <b><i>under construction !!!</i></b>
     - [Exercise 1.3 - Space Management] - <b><i>under construction !!!</i></b>
     - [Exercise 1.4 - Time Tables and Views Configurator](exercises/ex1/time-tables-views)
     - [Exercise 1.5 - Currency Conversion Configurator] - <b><i>under construction !!!</i></b>
     - [Exercise 1.6 - Fiscal Calendar Configurator] - <b><i>under construction !!!</i></b>
     - [Exercise 1.7 - Modeling Entities] - <b><i>under construction !!!</i></b>
     - [Exercise 1.8 - Data Lineage] - <b><i>under construction !!!</i></b>
     - [Exercise 1.9 - Versioning] - <b><i>under construction !!!</i></b>
     - [Exercise 1.10 - Change Management] - <b><i>under construction !!!</i></b>

### Data Layer
- [Exercise 2 - Upload Sample Data](exercises/ex2/)
     - [Exercise 2.1 - Upload BIKE SALES Sample Data](exercises/ex2/upload-bike-sales)
        - Upload CSV Files 
     - [Exercise 2.2 - Upload Currency Conversion Sample Data (TCUR*)](exercises/ex2/upload-tcur)
        - Data Wrangling    
        
- [Exercise 3 - Sales Orders](exercises/ex3/)  
    - [Exercise 3.1 - Create Business Partners View](exercises/ex3/business-partners-view)
        - Dimension View
        - ID + Text Semantic
        - Join Node  
        - Level Based Hierarchy 
        - Geo Spatial
    - [Exercise 3.2 - Create Product Texts View](exercises/ex3/product-texts-view)
        - Text View 
    - [Exercise 3.3 - Create Products View](exercises/ex3#products-view)
        - Text Association   
    - [Exercise 3.4 - Generate Time Tables and Views](exercises/ex1/time-tables-views)
    - [Exercise 3.5 - Create Sales Orders View](exercises/ex3/sales-orders-view)
        - Analytical Dataset View
        - Projection Node
        - Filter Node
        - Associations
    - [Exercise 3.7 - Create Story in SAP Analytics Cloud](exercises/ex3/create-story-in-sap-analytics-cloud)
    - 
- [Exercise 4 - Internal Orders](exercises/ex4/)
    - [Exercise 4.1 - Create Employee View](exercises/ex4/employees-view)
        - Internal Hierarchy  
    - [Exercise 4.2 - Create Vendor Product Category Hierarchy View](exercises/ex4/vendor-product-category-hierarchy-view)
        - Hierarchy View (External Hierarchy)
    - [Exercise 4.3 - Create Vendor Products View](exercises/ex4/vendor-products-view)
        - Hierarchy Association  
    - [Exercise 4.4 - Create Currency Rates View (TCURR)](exercises/ex4/tcurr-currency-view)
        - Union Node 
    - [Exercise 4.5 - Create Currency Prefactors View (TCURF)](exercises/ex4/tcurf-currency-view)
    - [Exercise 4.6 - Create Currency Configurations View (TCURV)](exercises/ex4/tcurv-currency-view)
    - [Exercise 4.7 - Create Currency Precisions View (TCURX)](exercises/ex4/tcurx-currency-view)
    - [Exercise 4.8 - Create Internal Orders View](exercises/ex4/internal-orders-view)
        - Calculation Node with Currency Conversion 
        - Input Parameters 
        - Aggregation Node 
    - [Exercise 4.9 - Create Story in SAP Analytics Cloud](exercises/ex3/create-story-in-sap-analytics-cloud)

 
 - [Exercise 5 - Extended Internal Orders] - <b><i>under construction !!!</i></b>
    - Exercise 4.5 - Create Extended Internal Orders View - <b><i>under construction !!!</i></b>
        - Change Management    
    - Exercise 4.5 - Create Cost Center View - <b><i>under construction !!!</i></b>
        - Compound Keys - <b><i>under construction !!!</i></b>
    - Exercise 4.6 - Create Cost Center Hierarchy View - <b><i>under construction !!!</i></b>
        - Time Dependency
            
- [Exercise 6 - Create Entity Relationship Model (ERM)] - <b><i>under construction !!!</i></b>
   - Associations
   - Text Associations
   - Hierarchy Associations
   
### Business Layer
- [Exercise 7 - Sales Pipeline]
    - [Exercise 7.1 - Create Business Entity]
    - [Exercise 7.2 - Create Consumption Model]
    - [Exercise 7.3 - Create a Cube / Query]
- [Exercise 7 - Sales Quota]
    - [Exercise 7.1 - Create Business Entity]
    - [Exercise 7.2 - Create Consumption Model]
    - [Exercise 7.3 - Create a Cube / Query]
- [Exercise 3 - Second Exercise Description]
    - [Exercise 2.1 - Exercise 2 Sub Exercise 1 Description](exercises/ex2#exercise-21-sub-exercise-1-description)
    - [Exercise 2.2 - Exercise 2 Sub Exercise 2 Description](exercises/ex2#exercise-22-sub-exercise-2-description)


## Links
- SAP Data Warehouse Cloud in [SAP Roadmaps](https://roadmaps.sap.com/board?PRODUCT=73555000100800002141&range=FIRST-CURRENT)
- Latest and greatest features of SAP Data Warehouse Cloud are presented regularly in [What's New](https://jam4.sapjam.com/blogs/show/JytsjzYpI9LproZNYpdkhG)

## License
Copyright (c) 2020 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
