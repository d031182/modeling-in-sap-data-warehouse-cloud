# Modeling in SAP Data Warehouse Cloud
## Description

This repository aims to onboard new users into Modeling in SAP Data Warehouse Cloud in the most practical manner. For that you will build a real working data model, which will embrace specific features and functions. During the journey there will be additional tips and explanations on various modeling concepts.

<!-- <div><video controls src="/images/TestVideo.mp4" muted="false"></video></div> -->

## Overview

<img align="right" src="/images/santran.png">
<b>"Learning by Doing"</b> is the main principle of this tutorial. Discover and understand the features and modeling concepts by putting your hands on the SAP Data Warehouse Cloud application and build a fully functioning data model yourself. 

The exercises are meant to be built in this particular order starting from basic concepts and diving step by step into deeper advanced features while progressing with the exercises. The exercises are also based on each other. Hence, they prerequisite each other.

The tutorial comes along with a sample dataset (CSV files), so that only a minimalistic system setup is required, without any complex source system connection and data ingestion processing activities (Off course, it is still highly recommended to get yourself familiar with those features, especially when you run SAP Data Warehouse Cloud in a full enterprise and productive manner). For this tutorial working with the prepared sample datasets serves the purpose.

In general, you should be aware that SAP Data Warehouse constantly updates and delivers new features. That means, that some of the described features might be outdated and look differently than from your latest version (for that please check regularly the "What's New" website and the SAP Roadmaps in the links section below). 

That being said, I hope this tutorial will give you a solid understanding and insights into the fundamental modeling principles of SAP Data Warehouse Cloud on which you can build upon in the future.

And now enjoy the tutorial ;)<br> 




San Tran<br>
Product Manager, SAP

p.s. many thanks to Amogh Kulkarni who provided the sample datasets for the exercises.

## Pre-requisites
Before you can start with the exercises, please make sure to get a running SAP Data Warehouse Cloud tenant with the latest updates.
For that you can apply for a **30-Days free Trial Tenant** under the following link:
- https://www.sap.com/products/data-warehouse-cloud/trial.html
- https://saphanajourney.com/data-warehouse-cloud/trial/

[![DWC_Free_Trial](/images/FreeDWCTrial.png)](https://saphanajourney.com/data-warehouse-cloud/trial/)

## Table of Content
### Get the Sample Data
- [<h2>Exercise 1 - Upload Sample Data</h2>](exercises/ex2/) 
     - [**Exercise 1.1 - Upload BIKE SALES Sample Data**](exercises/ex1/upload-bike-sales)
        - Upload CSV Files 
     - [**Exercise 1.2 - Upload Currency Conversion Sample Data (TCUR)**](exercises/ex1/upload-tcur)
        - Data Wrangling    

### Data Layer       
- [<h2>Exercise 2 - Sales Orders</h2>](exercises/ex2/)  
    - [**Exercise 2.1 - Create Business Partners View**](/exercises/ex2/business-partners-view)
        - Dimension View
        - ID + Text Semantic
        - Join Node  
        - Projection Node
        - Level Based Hierarchy 
        - Data Preview
        - View Deployment
        - [Exercise 2.1.1 - Configure Geospatial Data (Latitude, Longitude)](/exercises/ex2/business-partners-geospatial)
    - [**Exercise 2.2 - Create Products View**](/exercises/ex2/products-view)
        - [Exercise 2.2.1 - Create Product Texts View](/exercises/ex2/product-texts-view)
        - [Exercise 2.2.2 - Add Product Text Association](/exercises/ex2/product-texts-association)
    - [**Exercise 2.3 - Generate Time Tables and Views**](/exercises/ex0/time-tables-views)
    - [**Exercise 2.4 - Create Sales Orders View**](/exercises/ex2/sales-orders-view)
        - Analytical Dataset View
        - Filter Node
        - Associations
        - Measures
        - Replace Table
    - [**Exercise 2.5 - Create Sales Story in SAP Analytics Cloud**](/exercises/ex2/sales-story)
        - ID + Description (Text)
        - Level Based Hierarchy
        - Time Series
        - Variance on Previous and Current Period
        - Range Filter
        - Geo Spatial - Bubble Layer
   

- [<h2>Exercise 3 - Internal Orders</h2>](exercises/ex3/)  
    - [**Exercise 3.1 -Create Employee View**](/exercises/ex3/employees-view)
        - Parent Child Hierarchy (Internal)  
    - [**Exercise 3.2 - Create Vendor Products View**](/exercises/ex3/vendor-products-view)
        - [Exercise 3.2.1 - Create Hierarchy View](/exercises/ex3/vendor-product-category-hierarchy-view)
        - [Exercise 3.2.2 - Create Hierarchy Association](/exercises/ex3/vendor-products-hierarchy-association)
    - [**Exercise 3.3 - Create Internal Orders View**](/exercises/ex3/internal-orders-view)
        - [Exercise 3.3.1 - Wrap Currency Tables as Views](/exercises/ex3/currency-wrapper-view)
        - [Exercise 3.3.2 - Create Calculation Node with Currency Conversion](/exercises/ex3/currency-conversion)
        - [Exercise 3.3.3 - Using Input Parameters](/exercises/ex3/input-parameter) - :construction::construction::construction:
          - Input Parameters - :construction::construction::construction:
          - Union Node - :construction::construction::construction:
          - Story Filters - :construction::construction::construction:
          - Aggregation Node - :construction::construction::construction:
     - [**Exercise 3.4 - Create My Internal Orders View**](/exercises/ex3/my-internal-orders-view)
        - [Exercise 3.4.1 - Create Data Access Control](/exercises/ex3/data-access-control)
          - Data Access Control
        - [Exercise 3.4.2 - Apply Data Access Control](/exercises/ex3/apply-data-access-control)
        - [Exercise 3.4.3 - Maintain Data for a Data Access Control](/exercises/ex3/maintain-dac-data)
          - Table Data Maintenance
     - [**Exercise 3.5 - Create Internal Orders Story in SAP Analytics Cloud**] - :construction::construction::construction:
    
 
 - [Exercise 5 - Extended Internal Orders] - :construction::construction::construction:
    - Exercise 4.5 - Create Extended Internal Orders View - :construction::construction::construction:
        - Change Management    
    - Exercise 4.5 - Create Cost Center View - :construction::construction::construction:
        - Compound Keys - :construction::construction::construction:
    - Exercise 4.6 - Create Cost Center Hierarchy View - :construction::construction::construction:
        - Time Dependency :construction::construction::construction:
    - [Exercise 4.7 - Internal Orders] - :construction::construction::construction:
        - SQL View :construction::construction::construction:
        - Scripted View :construction::construction::construction:
        - Window Functions :construction::construction::construction:
   - Excercise 4.8:  :construction::construction::construction:     
        - Cross Space Sharing :construction::construction::construction:
   - Excercise 4.9 View Persistence :construction::construction::construction:
            
- [Exercise 6 - Create Entity Relationship Model (ERM)] - :construction::construction::construction:
   - Associations
   - Text Associations
   - Hierarchy Associations
  
   
### Business Layer :construction::construction::construction:
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
    - 
### SAP Data Warehouse Fundamentals
- [Repository Explorer] - :construction::construction::construction:
- [Data Source Browser] - :construction::construction::construction:
- [Space Management] - :construction::construction::construction:
- [Time Tables and Views Configurator](exercises/ex0/time-tables-views)
- [Currency Conversion Configurator] - :construction::construction::construction:
- [Fiscal Calendar Configurator] - :construction::construction::construction:
- [Modeling Entities] - :construction::construction::construction:
- [Data Lineage] - :construction::construction::construction:
- [Versioning](exercises/ex1/versioning) - :construction::construction::construction:
- [Change Management](exercises/ex0/change-management) - :construction::construction::construction:
- [View Persistence](exercises/ex0/change-management) - :construction::construction::construction:

## Comments, Issues and Feedbacks
Comments, issues and feedbacks are highly welcome to improve this tutorial grudually. Please file your feedback in the issues site of this repository. I will try to reply as soon as time allows :)
https://github.com/d031182/modeling-in-sap-data-warehouse-cloud/issues

## Links
- SAP Data Warehouse Cloud in [SAP Roadmaps](https://roadmaps.sap.com/board?PRODUCT=73555000100800002141&range=FIRST-CURRENT)
- Latest and greatest features of SAP Data Warehouse Cloud are presented regularly in [What's New](https://jam4.sapjam.com/blogs/show/JytsjzYpI9LproZNYpdkhG)
- SAP Help Site of SAP Data Warehouse Cloud: https://help.sap.com/viewer/product/SAP_DATA_WAREHOUSE_CLOUD/cloud/en-US

## License
Copyright (c) 2020 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
