## Email
#### Hey,

#### The board is asking to see how volume looked in Q2. I got some data (attached), but didn’t have a chance to pull anything together and was  hoping you could take a stab at it.

#### I think they just want to see Q2 2021 volume by region and wanted to know if everything was looking good. I think this file has what you need.
#### I don’t remember all the region codes – I know NAM ends in 1, EMEA ends in 3 and APAC and LATAM are 2 and 4, but I don’t remember which is . I do know LATAM has the lowest volume so just go ahead and assign that to which ever comes out lowest.

#### I appreciate your help!

## About Dataset
#### The dataset includes:
##### Cl ID, Geo ID, Date, Vol

## This repository contains:
1. Data wrangling 
2. Dashboard for volume by regions using power bi

## 1. Data wrangling
##### Before data cleaning
![untidy](https://github.com/Marwaaah/ExcelProject/assets/68570897/9e06883e-a760-45ad-9e59-1e9285f347cc)
##### After data cleaning
![tidy](https://github.com/Marwaaah/ExcelProject/assets/68570897/0b59134d-c15e-495c-b07b-9d1affd631a3)

### Data Cleaning Process
###### 1. rename sheet2 to Volume Data
######    rename sheet1 to Geo Data
###### 2. Fill Missing values in Cl ID column by using find & select excel tool
###### 3. change Volume column data type from general to number
###### 4. Extract Geo ID from Geo Data to Volume Data using VLOOKUP Function
###### The formula =VLOOKUP([@CLID],Table6,2,FALSE)
###### 5. Create Geo Name column by using information in the email
###### 6. Create Quarters column by using ROUNDUP Function
###### The formula ="Q" & ROUNDUP(MONTH(B:B)/3,0)&" " & YEAR(B:B)

![final](https://github.com/Marwaaah/ExcelProject/assets/68570897/65970320-2afd-40ed-b241-a238be989b84)
##### 7. Create Final sheet using pivot table and pivot charts

## 2. Dashboard to see Q2 2021 volume by region and  if everything was looking good using power bi
![dashboardd_page-0001](https://github.com/Marwaaah/ExcelProject/assets/68570897/dc99143d-6fc5-4e82-a7b9-398c9f4fc332)

