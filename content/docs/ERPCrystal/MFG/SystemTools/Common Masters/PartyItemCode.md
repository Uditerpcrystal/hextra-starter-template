---
title: "Party Item Code"
date: 2022-03-30
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 8
# tags: 
# - ERPCore 
# - SystemToolModule
# - PartyItemCodes 

---

## Introduction

Maintains the item code details of customers and vendors to be printed on invoices and purchase indents.


#### Mandatory Fields

<!-- |Mandatory Fields|  
  |:------| 
  | Customer / Supplier <br> - Select from Party Master <br> - Error code A - Wrong Party Id  <br> - Error code E - Duplicate Party, Item, Brand <br> `Validation` - A record with this Party / Item / Brand already exists.
  | Item <br> - Select from Item Master <br> - Error code B - Wrong Item Id <br> - Error code E - Duplicate Party, Item, Brand
  | Brand Name <br> - Select from Brand Master <br> - Error code C - Wrong Brand Id <br> - Error code E - Duplicate Party, Item, Brand
  | Party Item Code <br> `Validation` - Party Item Code needs to be 20 characters. <br> - Error code D - Wrong Party Item Code -->

  |Mandatory Fields|  
  |:------| 
  | Customer / Supplier <br> - Pre Selected (Options as per Party Master) <br> `Validation` - A record with this Party / Item / Brand already exists.
  | Item <br> - Pre Selected (Options as per Item Master)
  | Brand Name <br> - Pre Selected (Options as per Brand Master)
  | Party Item Code <br> `Validation` - Party Item Code needs to be 20 characters.


#### Optional Fields

|Optional Fields| 
  |:------|
  | Party Erp Code <br> `Validation` - Party Erp Code needs to be 20 characters.


####  Features

|Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete 
  | Export To Excel
  | Import <br> - Select File <br> `Validation` <br> - Uploaded CSV file name should be ImportPartyItemCode
  | Upload   