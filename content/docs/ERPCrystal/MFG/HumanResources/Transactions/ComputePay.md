---
title: "Compute Pay"
date: 2022-03-14
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
# - HumanResourcesOverview
# - ComputePay

---

## Introduction

Enables computation of monthly pay, bonus etc.

#### Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Year <br> - - Pre selected as current fiscal year  
  | Pay Date <br> `Validation` <br> - Pay Date cannot be after selected year range.
  | Compute <br> - Pre selected as Pay (Pay, Bonus)
  | Sales Incentive
  | Payroll type 

#### Features

|Feature|   
  |:------|
  | Update Percentage


#### Update Percentage - Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Employee Category <br> - Select Worker ,Staff [Factory] , Staff [Office].
  | Bonus Percentage <br> `Validation` <br> - Bonus Percentage can only be between 0.01-9999.99
  | Ex-gratia Percentage <br> `Validation`<br>  - Ex-gratia Percentage can only be between 0.01-9999.99

[How to create Compute Pay ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/humanresources/transactions/walkthroughcomputepay/)