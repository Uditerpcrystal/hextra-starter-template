---
title: "Leave Details"
date: 2022-03-14
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 9
# tags: 
# - ERPCore 
# - HumanResourcesOverview
# - LeaveDetails

---

## Introduction

Maintain leave records of employees.

#### Mandatory Fields

|Mandatory Fields|  
  |:------|   
  | Paydate <br> - Select from pay dates list.
  | Employee name <br> - Select from Employee Master <br> `Validation` <br>- Leave credit has already given for this employee
  | Leave Type <br> - Pre selected as Used (Used, Credited, Without Pay.) <br> `Validation` <br>- As leave balance is 0, select leave type as [Without Pay]
  | Date From <br> `Validations` <br>- From date must be between 01-Feb-22 and 28-Feb-22 <br> - From date may not be a holiday <br> `Validations` <br>- **From / To dates are overlapping with an earlier leave record.** If Leave record is allrady created for the Empolyee in that pay month 
  | Date To <br> `Validations` - To date cannot be before From date <br> - To date may not be a holiday <br> - **From / To dates are overlapping with an earlier leave record.** If Leave record is ready created for the Empolyee in that pay month  <br> - To date must be between Current Pay month's Start date and End date
  | No. of Days <br> `Validations` <br>- No. of days should not be more than the gap between To Date and From date <br> - No. of Days should not be less than the gap between To date and From date <br> - Days cannot be more than leave balance <br> - No. of Days should be greater than zero  
  | Reason For Leave


#### Features

|Features|   
  |:------|
  | Create New
  | Delete
  | Email
  | Export To Excel