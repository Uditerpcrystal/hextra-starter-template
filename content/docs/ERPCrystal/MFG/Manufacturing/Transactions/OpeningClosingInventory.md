---
title: "Opening / Closing Inventory"
date: 2022-02-17
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
# - ManufacturingModule
# - Opening/ClosingInventory

---

## Introduction

Maintain Opening / Closing inventories of good and rejected raw materials and finished goods.

#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Unit <br> - Select from GST units
  | Inventory Type <br> - Book, Excise, Store, Physical
  | Item State <br> - Good, Rejected


#### Features

|Features|   
  |:------|
  | OK
  | Upload Stock
  | Export to Excel

#### Inventory Item - Mandatory Fields

<!-- |Mandatory Fields|  
  |:------|
  | Division <br> - Select from Division Master
  | Item <br> - Select from Inventory Master <br> - Error code A - Invalid item id <br> - Error code D - Duplicate item id
  | Stage <br> - RM, FG Loose, FG Packed, WIP 10% <br> - Error code  B - Invalid stage
  | Brand <br> - Select from Brand Master <br> - Error code C - Invalid brand
  | Store Location <br> - Select from Store Master -->

  |Mandatory Fields|  
  |:------|
  | Division <br> - Select from Division Master.
  | Item <br> - Select from Inventory Master.
  | Stage <br> - RM, FG Loose, FG Packed, WIP 20%, WIP 40%, WIP 60%, WIP 80%.
  | Brand <br> - Select from Brand Master.
  | Store Location <br> - Select from Store Master.
  | Opg Qty
  | Opg Rate
  | Clg Qty
  | Clg Rate    



<!-- #### Inventory Item - Optional Fields

|Optional Fields| 
  |:------|
  | Opg Qty
  | Opg Rate
  | Clg Qty
  | Clg Rate  -->


#### Inventory Item - Features

|Features|   
  |:------|
  | Create New 
  | Modify
  | Delete
  | Export To Excel <br> - To download inventory report.


#### Upload Stock - Mandatory Fields  

|Mandatory Fields|  
  |:------|
  | Unit <br> - Select from GST units
  | Year <br> - Select year from year combo box.
  | Inventory Type <br> - Physical, Store
  | Item State <br> - Good, Rejected
  | Select File

#### Upload Stock  - Features

|Features|   
  |:------|
  | Download Model
  | Upload 
