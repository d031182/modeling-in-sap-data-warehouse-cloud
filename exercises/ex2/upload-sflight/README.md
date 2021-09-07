# Upload <i>SFLIGHT</i> CSV Files

## Download the sample dataset:
- Download the sample dataset via the following link: https://github.com/d031182/reference-data-model-samples/tree/main/data/SFLIGHT
- Make sure the following fiiles are available (last update 30th August 2021):
    - TCURR.csv (Currency Rates)
    - TCURF.csv (Currency Prefactors)
    - TCURV.csv (Currency Configurations)
    - TCURX.csv (Currency Precisions)
    - SFLIGHT.csv (Flight Sample Dataset)

       

## Upload <i>Currency Rates</i> CSV file
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURR.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    MANDT | String
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

## Upload <i>Currency Prefactors</i> CSV file
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURF.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    MANDT | String
    KURST | String
    TCURR | String
    GDATU | String
    FFACT | Integer
    ABWCT | String
    ABWGA | String

    <br><br>![](../images/create_tcurf_01.png)
    <br><br>![](../images/create_tcurf_02.png)

5. Click on Deploy to upload the file and create local table with the Business Name and Technical Name <b><i>CSV_TCURF</i></b>
    <br><br>![](../images/create_tcurf_04.png)

## Upload <i>Currency Configuration</i> CSV file
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURV.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    MANDT | String
    KURST | String
    XINVR | String
    BWAER | String
    XBWRL | String
    GKUZU | String
    BKUZU | String
    XFIXD | String
    XEURO | String
    
    <br><br>![](../images/create_tcurv_01.png)
    <br><br>![](../images/create_tcurv_02.png)

5. Click on Deploy to upload the file and create local table with the Business Name and Technical Name <b><i>CSV_TCURV</i></b>
    <br><br>![](../images/create_tcurv_03.png)
        
## Upload <i>Currency Precisions</i> CSV file
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>TCURX.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    CURRKEY | String
    CURRDEC | String
        
    <br><br>![](../images/create_tcurx_01.png)

5. Click on Deploy to upload the file and create local table with the Business Name and Technical Name <b><i>CSV_TCURX</i></b>
    <br><br>![](../images/create_tcurx_02.png)
    

## Upload <i>Flight</i> CSV file
1. Navigate to the Data Builder of SAP Data Warehouse Cloud
2. Click on the <b><i>Import CSV File</i></b>
  <br>![Import CSV File](../images/ImportCSVFile_2.png)
3. Select the <i><b>SFLIGHT.csv</b></i> as source file and click on Upload
  <br>![Import CSV File](../images/ImportCSVFile_3.png)
4. Adjust the column data types as the following:

    Column | Data Type
    ---------|---------
    MANDT | String
    CARRID | String
    CONNID | String
    FLDATE | Date
    PRICE | Number
    CURRENCY | String
    PLANETYPE | String
    SEATSMAX | Integer
    SEATSOCC | Integer
    PAYMENTSUM | Number
    SEATSMAX_B | Integer
    SEATSOCC_B | Integer
    SEATSMAX_F | Integer
    SEATSOCC_F | Integer
    
    <br><br>![](../images/create_sflight_01.png)
    <br><br>![](../images/create_sflight_02.png)

5. Click on Deploy to upload the file and create local table with the Business Name and Technical Name <b><i>CSV_SFLIGHT</i></b>
    <br><br>![](../images/create_sflight_03.png)
