---
title: "In/Out Register"
date: 2022-01-19
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight  : 7
# tags: 
# - ERPCore 
# - SupplyChainModule
# - In/OutRegister

---

## Introduction 

This feature helps to record In / Out movements of material and other items by security staff.

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Year <br> - Pre-Selected current fiscal year
  | In / Out <br> - Pre selected as In (In, Out)
  | Document Type <br> - Preselected as NA (NA, Purchase Bill, Job Work)
  | Date <br> - Pre selected as current date and time
  | Unit Name 
  | Customer / Supplier <br> - Select from Party Master **If it is IN and party name is not selected OR It is OUT and Document Type is NA** <br> `Validation` <br>  - Invalid party name 
  | Item Name <br> - Select from Inventory Master.
  | Qty <br> `Validation` <br>  - Qty : Range 0 - 9999999.999
  | Weight <br> `Validation` <br>  - Qty : Range 0 - 99999.999

#### Optional Fields

|Optional Fields|   
  |:------|
  | Non Std Customer/Supplier Name
  | Reference Date
  | Reference No <br> `Validation` <br>  - Invoice details not found <br> - Invoice details already available in In/Out Register <br> - Incorrect Reference No <br> - Job Work Challan Details not found. <br> - **Job Work Details already available in In/Out Register.** This validation will be showed when the chalan number will be keyed in by the user is related to some other in/out number.
  | Non standard Item Name <br> `Validation`  <br> - Either Item name or Non Std. name needs to be filled.
  | No. of Packaging <br> `Validation` <br>  - Incorrect No. of packaging
  | Vehicle No. <br> `Validation` <br>  - Invalid vehicle No
  | Select Remark <br> - Select from Remark Master.
  | Non Standard Remarks
  | `callout` <br> - In case of Sales Invoice / Job Work , Customer/Supplier may not be selected
#### Features   

|Features|   
  |:------|
  | Create New 
  | Modify
  | Delete <br> - If the document is linked to GRN or Sales Return , this option will be disabled.
