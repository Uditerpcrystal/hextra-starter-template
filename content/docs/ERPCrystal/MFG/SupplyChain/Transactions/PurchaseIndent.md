---
title: "Purchase Indent"
date: 2022-01-17
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
# tags: 
# - ERPCore 
# - SupplyChainModule
# - PurchaseIndent

---

## Introduction

Purchase Indents are material requests made by branch or department to head-office or another branch/department within the organization. If purchases are centralized, the Purchase Manager or Merchandiser can make purchase decisions based on indents received or transfer existing stocks from any location to fulfill the demand.
<!-- This feature helps to manage indenting of material by Factory / Office. -->

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Year <br> - Pre selected current fiscal year
  | Indent Date <br> - Pre selected current date <br>`Validation` <br>  - **Date must be between FY Start and FY End** If the selected date is outside Fiscal Year 
  | Indent Type <br> NA - Not Applicable , RM - Raw Material , RD - R&D etc. <br>
  | Indent From <br> - Select GST Unit Name <br>
  | Customer/Supplier/Branch <br> - Select from Party master <br>`Validation`<br> **GST Registration No is not available in Party Master.** If the GST registration no. is not updated in the branch of party master then this validation will be shown
  | Currency <br> Pre selected as INR (Options as per Currency Master)
  | Freight Type <br> - Pre Selected as NIL (Options as per Freight master)
  | Freight,Octroi,Carriage & Packing <br> `Validation` <br>  - Freight amount can only be between 0-999999.99
  | Discount Rate <br> `Validation` <br>  - Discount rate can only be between 0-99.99
  | Discount Amount <br> `Validation` <br>  - Discount can only be between 0-999999.99
  | Cash Discount Rate <br> `Validation` <br>  - Cash Discount rate can only be between 0 - 999.99
  | Form `Validations`<br>- **System Indents are being DONE, User cannot Create Indent.** {{< callout type="info" >}}While importing indent through excel if one tries to create indent through user interface then this validation message will be shown.{{< /callout >}}
  <!-- | Customer/Supplier/Branchs <br> - Select from Party master <br> - Error code A - Wrong party id or branch id -->
<!--   | Indent From <br> - Select GST units <br> - Error code I - Invalid unit code -->
#### Optional Fields

|Optional Fields|   
  |:------|
  | Send To <br> - Select from Party master
  | Mode <br> Road, Rail, Ocean, Courier, Air <br>
  | Quote Reference
  | Quote Date
  | Request No <br>
  | Request Date <br>
  | Notes
  <!-- | Request No <br> - Error code G - Request no is required -->
  <!-- | Request Date <br> - Error code H - Invalid request date -->
  <!-- | Mode <br> Road, Rail, Air etc <br> - Error code O - Invalid mode of transport -->
  

#### Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If lock is applied to the document, this option will be disabled.
  | Delete <br> - If lock is applied to the document, this option will be disabled.
  | Make GRN for entire Indent <br> - To create Goods Received Note (GRN)
  | Import Indent  <br> - To upload/import indent details in the excel file format
  | **Only for Print/Email** <br> - Print Total Qty / Value ? :  Yes / No <br> - Print Indent <br> - Print Stores Copy <br> - Email <br> - Print Indent Excel <br> - Print Stores Copy Excel <br> - Email Excel 


#### Create Goods Received Note - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | GRN Date <br> - Auto fetched by System
  | GRN Type <br> - Purchase, Manufacturing
  | Transporter Name <br> - Select from Transporter Master
  | Store Location <br> - Select from Store Master


#### Import Indent - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Indent Date
  | Select Currency <br> - Pre selected as INR (Options as per Currency Master)
  | Select File <br> `Validation` <br>  - Uploaded file name should be ImportIndent

#### Import Indent - Feature

|Features|  
  |:------|
  | Download Model <br> - To fill the data in specific format

#### Indent Item Create - Manadatory Fields

|Mandatory Fields|   
  |:------|                   
  | Item  <br> - Select from Item / Inventory Master <br> 
  | Brand Name <br> - Pre selected as NA (Options as per Brand Master) <br>
  | Stage <br> - Pre selected as RM (RM,FG LOOSE, FG PACKED, WIP 20% etc. ) <br>
  | Quantity  <br> `Validation` <br>  - Quantity should be between 0.001 - 9999999.999 <br>
  | Rate <br> `Validations` <br>  - Rate is not available in price master for this item, party, brand, currency <br> - Non Standard Price is not enabled for this item group <br> - Rate should be between 0.0001 - 99999999.9999  <br>
  | Form `Validation` <br> - **Lead Time data not available for this Party / Item.** Lead Time data must be created in the Lead Time master for this particular vendor , branch , item and mode.<br> If **Get ReqdBy From Lead Time Master** parameter is On then the system will pickup lead Time and Transit days from the Lead Time Master to calculate Required by date i.e Indent date + Lead time + Transit days.<br>  If **Get ReqdBy From Lead Time Master** parameter is Off then Required by date will be calculated as Indent date + Lead time as per Inventory Master + Transit days provided by user. <br> - **Multiple records exist for party,branch,item and mode in lead time master.** While picking up lead time and transit days based on party , branch , item and mode from the lead time master, if multiple values are found then this validation will be shown.{{< callout type="info" >}}If this error occur please duplicate values.{{< /callout >}}
 | Indent Status <br> - Auto inserted as Ok during the Indent creation
  <!-- | Rate <br> `Validations` - Rate is not available in price master for this item, party, brand, currency <br> - Non Standard Price is not enabled for this item group <br> - Rate should be between 0.0001 - 99999999.9999  <br> - Error code E - Rate is not available in price master for this item and party -->
  <!-- | Quantity  <br> `Validation` - Quantity should be between 0.001 - 9999999.999 <br> - Error code D - Invalid quantity <br> - Error code F - Qty * Rate should not exceed 99.99 cr or rate is 0 -->
  <!-- | Stage <br> - Select from Stage list <br> - Error code N - Invalid stage -->
  <!-- | Item  <br> - Select from Item / Inventory Master <br> - Error code B - Wrong item id -->
  <!-- | Brand Name <br> - Select from Brand Master <br> - Error code C - Wrong brand id -->

#### Indent Item Create - Optional Fields

|Optional Fields|   
  |:------|
  | Lead Time  
  | Transit Days  
  | GST Code <br> - Select from list of Inventory Master <br> `Validation`  <br> - Auto-fetch did not succeed. GST code specified in inventory master may not be valid
  | Currency / Load Factor <br> `Validation` <br>  - Currency / load factor should be between 1.0000 - 999.9999 <br>
  | To Be Received By <br> `Validation` <br>  - To be received by date must be Indent Date + Lead Time + Transit Days or Later.
  | Allow manual rate ? <br> - Yes / No
  | Non Standard Item Name 
  | **Only for Change Follow Up Notes** <br> - Expected On <br> `Validation`  <br> - Expected On date can not be less than required by date
  | Is Non Standard 
  | Non Std Price 
  <!-- | Lead Time <br> - Error code Q - Lead time data not available for this party / branch / item -->
  <!-- | Currency / Load Factor <br> `Validation` - Currency / load factor should be between 1.0000 - 999.9999 <br> - Error code R - Load factor should be between 1.0000 - 999.9999 <br> - Error code S - For INR load factor must be 1 -->
  <!-- | Transit Days <br> - Error code P - Invalid transit days -->
  <!-- | Non Standard Item Name <br> - Error code J - Non standard price is not allowed for this itemid  -->
  <!-- | Is Non Standard <br> - Error code K - Is non standard must be Y / N -->
  <!-- | Non Std Price <br> - Error code L - Non standard price must be specified for non standard item <br> - Error code M - Non standard price must be greater than 0 and less than 9999999.9999 -->

 
#### Indent Item Create - Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If GRN is already made against the indent, this option will be disabled. <br> - If bill is already made against the indent, this option will be disable. <br> - If Import Document is already made against the indent, this option will be disabled.
  | Delete <br> - If GRN is already made against indent, this option will be disabled. <br> - If bill is already made against indent, this option will be disabled. <br> - If bill is already made against the indent, this option will be disabled. <br> - Import Document is already made against the indent, this option will be disabled.
  | Change Follow Up Notes <br> - To Update expected on and follow up note <br> - Update
  | Convert this item to manual rate <br> - Modify other details and manual rate
  | Re-Update rate <br> - Update rate from price master
  | Re-Update GST rate <br> - Update GST rate from inventory master
  | Item Details <br> - To Show list / index of item details of purchase indent


[How to create a Purchase Indent ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/walkthroughpurchaseindent/)