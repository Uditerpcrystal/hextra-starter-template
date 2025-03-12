---
title: "FEMA Compliance"
date: 2022-03-07
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 12
# tags: 
# - ERPCore 
# - SupplyChainModule
# - FEMACompliance

---

## Introduction 



#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Party Name <br> - Select from Party Master
  | Pro-Forma Invoice No
  | Pro-Forma Invoice Date <br> - Pre selected as current date <br> `Validation` <br> - Future dates are not allowed
  | Select Currency <br> - Select from Currency Master
  | Pro-Forma Invoice Amount <br> `Validation`  <br>- Pro-Forma invoice amount can only be between 1-9999999.99
  | **Only for Update ORM** <br> ORM No <br> ORM Date <br> - Pre selected as current date <br> - Future dates are not allowed <br> `Validation`  <br>- ORM date must be after Pro-Forma invoice date   <br> Debit Advice No
  | **Only for Update Invoice** <br> Commercial Invoice No <br> Commercial Invoice Date  <br> - Pre selected as current date <br> `Validation`  <br>- Invoice date must be after ORM date. <br> - Future dates are not allowed <br> Commercial Invoice Amount <br> `Validation` <br> - Commercial invoice amount can only be between 1-9999999.99 <br> BOE No <br> BOE Date  <br> - Pre selected as current date  <br> `Validations` <br>  - BOE date must be after ORM date. <br> - Future dates are not allowed <br>- AWB No
  | **Update Submission Date** <br> Submission Date  <br> `Validations` <br> - Submission date must be after invoice date <br> - Future dates are not allowed

  
#### Optional Fields

|Optional Fields|  
  |:------|
  | Notes


#### Features

|Features| 
  |:------|
  | Create New 
  | Delete
  | Update Pro-Forma <br> - To update Pro-Forma invoice details.
  | Update ORM <br> - To update ORM details.
  | Update Invoice <br> - To update commercial invoice details
  | Update Submission Date <br> - To update the submission date.
  | FEMA Report <br> - To Download the FEMA Report with specific date range.
