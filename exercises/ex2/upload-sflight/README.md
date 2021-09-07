# Upload <i>SFLIGHT</i> CSV Files

## Download the sample dataset:
- Download the sample dataset via the following link: https://github.com/d031182/reference-data-model-samples/tree/main/data/SFLIGHT
- Make sure the following fiiles are available (last update 30th August 2021):
    - TCURR.csv (Currency Rates)
    - TCURF.csv (Currency Prefactors)
    - TCURV.csv (Currency Configurations)
    - TCURX.csv (Currency Precisions)
    - SFLIGHT.csv (Flight Sample Dataset)

       

## Upload file for Currency Rates
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURR.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    KURST | String
    FCURR | String
    TCURR | String
    GDATU | String
    UKURS | Number
    FFACT | Integer
    TFACT | Integer
    
    <br><br>![](../images/create_tcurr_01.png)
    <br><br>![](../images/create_tcurr_02.png)
    
5. Click on Deploy to upload the file and create local table with the Business Name and Technical Name <b><i>CSV_TCURR</i></b>
    <br><br>![](../images/create_tcurr_03.png)

## Upload file for Currency Prefactors
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURF.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    KURST | String
    FCURR | String
    TCURR | String
    GDATU | String
    UKURS | Number
    FFACT | Integer
    TFACT | Integer

    <br><br>![](../../images/create_tcurf_01.png)
    <br><br>![](../../images/create_tcurf_02.png)

## Upload <i>TCURV.csv</i> for Currency Configuration
<br><br>![](../../images/create_tcurv_01.png)
<br><br>![](../../ex2/images/create_tcurv_02.png)
        
        
## Upload <i>TCURX.csv</i> for Currency Precisions
<br><br>![](../../images/create_tcurx_01.png)
<br><br>![](../../images/create_tcurx_02.png)
