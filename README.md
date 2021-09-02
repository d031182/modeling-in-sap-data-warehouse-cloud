# Modeling in SAP Data Warehouse Cloud
## Description

This repository aims to onboard new users into Modeling in SAP Data Warehouse Cloud in the most practical manner. For that you will build a real working data model, which will embrace specific features and functions. During the journey there will be additional tips and explanations on various modeling concepts.

## Overview

The exercises are meant to be built in this particular order starting from basic concepts, while the more advance aspects are following later. 
Please be aware, when creating this tutorial features might be updated or replaced in SAP Data Warehouse Cloud. 
Nonetheless, I hope it still give you a solid understanding on the fundamental concepts in modeling. 

And now enjoy the tutorial ;) 


## Requirements
Before you can start with the exercises, please make sure to get a running SAP Data Warehouse Cloud tenant with the latest updates.
For that you can apply for a **30-Days free Trial Tenant** under the following link:
- https://www.sap.com/products/data-warehouse-cloud/trial.html
- https://saphanajourney.com/data-warehouse-cloud/trial/

[![DWC_Free_Trial](/images/FreeDWCTrial.png)](https://saphanajourney.com/data-warehouse-cloud/trial/)

## Exercises

Provide the exercise content here directly in README.md using [markdown](https://guides.github.com/features/mastering-markdown/) and linking to the specific exercise pages, below is an example.

### SAP Data Warehouse Fundamentals
- [Exercise 1 - SAP Data Warehouse Cloud Fundamentals]
    - [Exercise 1.1 - Repository Explorer]
    - [Exercise 1.2 - Space Management]
    - [Exercise 1.2 - Modeling Entities]
    - [Exercise 1.3 - Lineage]

### Data Layer
- [Exercise Overview](exercises/overview/)

- [Exercise 1 - Upload CSV files](exercises/ex1/)
 
- [Exercise 3 - Sales Orders](exercises/ex3/)  
    - [Exercise 3.1 - Create Business Partners View](exercises/ex3#create-business-partners-view)
        - Dimension
        - ID + Text Semantic
        - Join Node  
        - Level Based Hierarchy 
        - Geo Spatial
    - [Exercise 3.2 - Create Product Texts View](exercises/ex3#product-texts-view)
    - [Exercise 3.3 - Create Products View](exercises/ex3#products-view)
        - Text Association   
    - [Exercise 3.4 - Generate Time Tables and Views](exercises/ex3#generate-time-tables-and-views)
    - [Exercise 3.5 - Create Sales Orders View](exercises/ex3/sales-orders-view.md)
        - Analytical Dataset
        - Projection Node
        - Filter Node
        - Union Node
        - Associations
    - [Exercise 3.6 - Create Entity Relationship Model (ERM)](exercises/ex3#entity-relationship-model)
        - Associations
        - Text Associations
        - Hierarchy Associations
    - [Exercise 3.7 - Create Story in SAP Analytics Cloud](exercises/ex3#create-story-in-sap-analytics-cloud)
    - 
- [Exercise 4 - Internal Orders](exercises/ex4/)
    - [Exercise 4.1 - Create Employee View](exercises/ex4#create-employee-view)
        - Internal Hierarchy  
    - [Exercise 4.2 - Create Vendor Product Category Hierarchy View](exercises/ex4#create-vendor-product-category-hierarchy-view)
        - External Hierarchy  
    - [Exercise 4.3 - Create Vendor Products View](exercises/ex4#create-vendor-products-view)
        - Hierarchy Association  
    - [Exercise 4.4 - Create Internal Orders View](exercises/ex4#create-internal-orders-view)
        - Calculation Node
        - Currency Conversion
        - Input Parameters
        - Aggregation Node
- [Exercise 5 - Create Entity Relationship Model](exercises/ex1/)
    - [Exercise 1.1 - Exercise 1 Sub Exercise 1 Description](exercises/ex1#exercise-11-sub-exercise-1-description)
    - [Exercise 1.2 - Exercise 1 Sub Exercise 2 Description](exercises/ex1#exercise-12-sub-exercise-2-description)
- [Exercise 6 - Create a Story in SAP Analytics Cloud](exercises/ex1/)
    - [Exercise 1.1 - Exercise 1 Sub Exercise 1 Description](exercises/ex1#exercise-11-sub-exercise-1-description)
    - [Exercise 1.2 - Exercise 1 Sub Exercise 2 Description](exercises/ex1#exercise-12-sub-exercise-2-description)



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


**OR** Link to the PDF document stored in your github repo for example...

Start the exercises [here](exercises/myPDFDoc.pdf).
    
**OR** Link to the Tutorial Navigator for example...

Start the exercises [here](https://developers.sap.com/tutorials/abap-environment-trial-onboarding.html).

## Links
- SAP Data Warehouse Cloud in SAP Roadmaps: https://roadmaps.sap.com/board?PRODUCT=73555000100800002141&range=FIRST-CURRENT
- SAP Data Warehouse Cloud What's New?

## License
Copyright (c) 2020 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
