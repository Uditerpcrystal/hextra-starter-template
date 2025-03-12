---
title: "Daily Production Monitor"
date: 2022-02-17
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 6
# tags: 
# - ERPCore 
# - ManufacturingModule
# - DailyProductionMonitor

---

## Introduction

Helps to set daily production targets shop-floor wise and monitor actual product performance.

#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Plan  <br> - First Floor, Second Floor Etc. <br> `Validation` - Plan must be Selected for production monitor

#### Features

|Features| 
  |:------|
  | Set Target <br> - To set daily production target
  | **Production Monitor** <br> - To set today's target <br> Select Plan  <br> `Validation` - Plan must be selected for production monitor <br> Production <br> - Scan or enter itemid <br> `Validation` - This item is not available in today's target. <br> *Featurs* : OK, Refresh
  | **Set Daily Workers** <br> - To create daily production workers <br> Select Plan  <br> - First Floor, Second Floor, Third Floor Etc. <br> No. of Workers <br> `Validation` - Workers cannot be 0 and less then zero <br> *Featurs* : Modify

#### Set Target - Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Plan  <br> - First Floor, Second Floor, Third Floor Etc.
  | Select Item  <br> - Select from Item Master <br> `Validation` - There is no production plan for this Item. <br> - This item is already available in today's target
  | Start Date / Time
  | End Date / Time <br> `Validation` - From / to date must be same.<br>To Date cannot be before From Date
  | Target Qty <br> `Validation` - Target qty can not be 0 <br>- Target qty cannot exceed remaining linked plan qty {{< callout type="info" >}} For Example <br> If the linked plan quantity is set as 1000 and we have already achieved target quantity of 600 then for the 2nd time we can take target quantity only upto 400 i.e. 1000 - 600 = 400{{< /callout >}}
  | Is This Against Linked Plan? <br> - Yes / No    

#### Set Target - Optional Fields

|Optional Fields| 
  |:------|
  | Notes

#### Set Target - Features

|Features|   
  |:------|
  | Create New 
  | Delete <br> - If target is live, this option will be disabled.     

#### Production Monitor - Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Plan  <br> `Validation` - Plan must be selected for production monitor
  | Production <br> - Scan or enter itemid <br> `Validation` - This item is not available in today's target.  -->
#### Production Monitor - Features

|Features|   
  |:------|
  | OK
  | Refresh

#### Set Daily Workers - Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Plan  <br> - First Floor, Second Floor, Third Floor Etc.
  | Date <br>  `Validation` - Record for this floor plan and date is already available
  | No. of Workers <br> `Validation` - Workers cannot be 0 and less then zero

#### Set Daily Workers - Features

|Features|   
  |:------|
  | Modify  
