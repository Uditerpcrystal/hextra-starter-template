---
title: "Make To Availability"
date: 2022-01-12
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 10
# tags: 
# - ERPCore 
# - SalesModule
# - MakeToAvailability

---

## Introduction

Helps to keep record for plan qty for the items.
<!-- Helps to plan MTA (Make To Availability) quantity. -->
<!-- Helps to keep record for plan qty for an items. -->
#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Item Id <br> - Auto fetched from uploaded excel 
  | MTA Month <br> - Auto fetched from uploaded excel
  | Item Name <br> - Auto fetched from System
  | Original Quantity <br> - Auto fetched from uploaded excel <br> `Validations` 
  | Additional Quantity <br> - Enter desired quantity <br> `Validation` <br> - Additional Quantity can not be zero.<br> - Revised Qty may not be lower than MTA Qty in orders. (Sum of Original Qty and Addition Qty must be greater then sum of Sales Orders Qty for selected item.)
  | Reason to Modify <br>  `Validation` - Notes maybe upto 200 characters and minimum of 15 characters.
 
  

#### Import MTA - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | MTA Month <br> - By default current month with the last date
  | Select File <br> - Save the file in Csv extension <br> `Validation` <br> - Uploaded file name should be ImportMTA. <br> -  Re-uploading is not allowed for first three months
  
#### Features

|Features|  
  |:------
  | Import MTA <br> - To Plan MTA 
  | Download Model <br> - To set/plan MTA in specific format
  