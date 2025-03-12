---
title: "Ceiling/Floor Price"
date: 2022-12-10
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 7 

---


## Introduction

To maintain the ceiling price and the floor price of all items, this master was created, where you will get to see the ceiling price and floor price of all the items that you have created.

#### Mandatory Fields
|Mandatory Fields|  
|:------| 
|Type. <br> - It can be either Ceiling price or Floor price. <br> - By default it will be Floor price.
|Item Shortname <br> - Select item for Inventory Master. <br> - A search box is available to search for a specific item.<br> `Validation` - Item needs to be selected.
|Currency <br>- Pre Selected as INR (Options as per Currency Master)
|Price  <br> `Validation` <br> - Price should be between 0.01 to 99999999.9999 <br>- If the record is already created with the same item and currency then <b>"For this item, currency record already exists."</b> validation will be shown. <br> - Floor Price must be more than Ceiling Price. <br> - Ceiling Price must be less than Floor Price.

####  Features

|Features|   
|:------|
|Create
|Modify
|Export to Excel
|Import Ceiling/Floor Price