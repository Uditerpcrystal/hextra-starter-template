---
title: "Transfer Price Master"
date: 2022-01-13
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 5
# tags: 
# - ERPCore 
# - SalesModule
# - TransferPriceMaster

---

## Introduction

This feature helps to maintain transfer prices for various items.

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Item <br> - Select from Inventory master.
  | Transfer Price <br> `Validation` - Range between 1 - 999999.9999 
  | Recommended Sales Price (RSP) <br> `Validation` - Range 1 - 999999.9999
  | No Regret Price (NRP) <br> `Validation` - Range between 1 - 999999.9999
  | Apply From Date <br> - Pre Selected as current date.

#### Optional Fields

|Optional Fields|   
  |:------|
  | Notes

#### Features

|Features|  
  |:------|
  | Create New 
  | Modify
  | Delete
  | Import Transfer Price <br> - Option to create multiple Transfer Price records from XL template. <br> `Valdation` <br> - Uploaded File must be with csv extension and file name must be ImportTransferPrice.

<!-- #### Import Transfer Price - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Apply From Date
  | Select File 

#### Import Transfer Price - Features

|Features|  
  |:------|
  | Upload <br>  `Validation` - Uploaded file name should be ImportTransferPrice <br> - Save the file in Csv format
  | Download Model 
   -->
