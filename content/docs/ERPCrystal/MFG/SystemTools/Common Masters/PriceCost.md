---
title: "Price/Cost"
date: 2022-03-29
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 7
# tags: 
# - ERPCore 
# - SystemToolModule
# - Price/Cost   

---

## Introduction

Maintain details of price, cost, transfer price of various items over party, brand and currency.


#### Mandatory Fields

<!-- |Mandatory Fields|  
  |:------| 
  | Customer / Supplier <br> - Select from Party Master
  | Item Shortname <br> - Select from Inventory Master
  | Brand Name <br> - Select from Brand Master
  | Select Currency <br> - Select from Currency Master
  | Load Factor <br> `Validations` - Currency / Load Factor should be between 1.0000 - 999.9999 <br> - For INR Currency, Load Factor must be 1.0000
  | Price <br> `Validations` - Please set Floor Price in Inventory Master, for this item. <br> - Price : Range 0 - 9999999.9999 <br> - Sale Price can not be less than Floor Price <br> Error code A - Invalid Sale Price
  | Updated On
  | Use this for BOM at standard cost <br> - Yes / No -->

  |Mandatory Fields|  
  |:------| 
  | Customer / Supplier <br> - Select from Party Master
  | Item Shortname <br> - Select from Inventory Master
  | Brand Name <br> - Select from Brand Master
  | Select Currency <br> - Select from Currency Master
  | Load Factor <br> `Validations` <br> - Currency / Load Factor should be between 1.0000 - 999.9999 <br> - For INR Currency, Load Factor must be 1.0000
  | Price <br> `Validations` <br>- If the ceiling price and the floor price are not set in the Ceiling/Floor price master then **Please set Floor Price in Ceiling / Floor Price Master, for this item.** validation will be shown. <br> - Price : Range 0 - 9999999.9999 <br> - Sale Price can not be less than Floor Price. <br> - **Sorry! you have no access rights to view both Sale / Cost prices.** In order to view/create/modify sales price and cost price admin user needs to grant access right to the user.
  | Updated On
  | Use this for BOM at standard cost <br> - Yes / No <br>- In BOM if you wish to use price/cost master rate as a standard rate you may set this parameter as yes.


#### Optional Fields

|Optional Fields| 
  |:------|
  | Cost <br> `Validations` <br> - Cost : Range 0 - 99999999.9999 <br> - Please set Ceiling Price in Inventory Master, for this item <br> - **This is a BPA item, you can not enter cost here.** For BPA (Bulk Price Agreement) item cost may not be updated in Price Master.
  | Credit Days
  | Non standard Item Name
  | CST Percentage <br> `Validation` - CST Percentage : Range 0 - 999.99
  | MRP  
  

####  Features

<!-- |Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete 
  | **Authorize Special Sale Price** <br> Special Sale Price <br> `Validation` - Price must be greater than zero.
  | **Bulk Edit Price Records** <br> Customer / Vendor <br> - Select from Party Master <br> Select File <br> `Validation` - Uploaded CSV file name should be UpdatePrice
  | **Create Multiple** <br> Select File <br> `Validation` - Uploaded CSV file name should be PriceMst <br> Download Model <br> Upload   
  | **Error codes for Import Master Data** <br> - Error code A - Invalid Itemid <br> - Error code B - Invalid Partyid <br> - Error code C - Invalid BrandId <br> - Error code D - Sale Price should be 0 <br> - Error Code E - Cost Price should be 0 <br> - Error Code F - Sale Price less than Floor Price Or Floor Price is 0 <br> - Error Code G - Cost Price more than Ceiling Price Or Ceiling Price is 0 <br> Error code H - Both Sale / Cost Prices are 0    -->

  |Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete 
  |Export to Excel
  | **Bulk Edit Price Records** <br> Customer / Vendor <br> - Select from Party Master <br> Select File <br>- In order to update price/cost for multiple items you can use this and edit through XL interface<br> `Validation` - Uploaded CSV file name should be UpdatePrice
  | **Create Multiple** <br> Select File  <br> Download Model <br> Upload <br> `Validation` - Uploaded CSV file name should be PriceMst.