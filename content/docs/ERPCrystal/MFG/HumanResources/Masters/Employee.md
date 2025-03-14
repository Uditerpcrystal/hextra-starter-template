---
title: "Employee"
date: 2022-03-15
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 3
# tags: 
# - ERPCore 
# - HumanResourcesOverview
# - Employee  

---

## Introduction

Maintains master data of employees.


#### Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Type of Employee <br> - Pre selected as Own (Own, Contract-Surwase, NEEM etc.)
  | Title <br> - Pre selected as Mr (Mr, Ms, Dr etc)
  | Gender <br> - Pre selected as Male (Male, Female) <br> `Validation`  <br>- Wrong gender selected.
  | First Name
  | Last Name
  | Date of Birth <br> - Pre selected as current date `Validation` <br> - Employee must have completed 18 years as on the date of joining
  | Contact No
  | Email
  | Date of Joining <br> - Pre selected as current date
  | Department <br> - Select from Department master.
  | Cost Center <br> - Pre selected as NA (Options as per Cost Center Master)
  | Designation
  | Grade <br> - Select from Grade master.
  | Category <br> - Staff (office/factory), worker
  | Pay Basis <br> - Daily rate, Hybrid, Monthly Rate etc.
  | Select Shift <br> - Pre selected (Select shift for general, over time.)
  | Mode Of Pay <br> - Pre selected as Cash (Cash, Cheque, ECS etc.)
  | PAN No
  | Time Record System No <br> `Validation`<br>- Time Record System No is duplicate
  | PF Applicable? <br> - Pre selected as No (Yes / No)
  | ESIC Applicable? <br> - Pre selected as No (Yes / No)
  | Professional Tax Applicable? <br> - Pre selected as No (Yes / No)
  | Eligible for Bonus? <br> - Pre selected as No (Yes / No)
  | Eligible for Exgratia? <br> - Pre selected as No (Yes / No)
  | Labor Welfare Fund Applicable? <br> - Pre selected as No (Yes / No)
  | Is Director? <br> - Pre selected as No (Yes / No)
  | Eligible for Domestic Incentive? <br> - Yes / No
  | Eligible for Export Incentive? <br> - Yes / No


#### Optional Fields

|Optional Fields| 
  |:------|
  | Bank Name
  | Branch Name
  | Bank A/c No
  | IFSC Code
  | UAN No <BE> `Validation` <br> - Please enter a valid UAN no. <br> - UAN No needs to be 12 digits.
  | EPF No
  | ESI No
  | Date of Leaving <br> `Validations`  <br> - Date of leaving must be between Current Pay month  and Next Pay Month <br> - Date of leaving must be after to date of joining.


#### Features

|Features|   
  |:------|
  | Create New
  | Modify <br> `callout` <br>- If employee has already left, this option will be disabled.  
  | Delete <br>`callout` <br> - If the master record is live, you may not delete it. <br> - If employee has already left, this option will be disabled.  
  | Export To Excel
  | Employee Type <br> - To create employee type master record.
  | Import Employee Master


#### Employee Type - Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Type Code <br> - Auto generated by System
  | Type Name  


#### Employee Type - Features

|Features|   
  |:------|
  | Create New
  | Modify  
  | Delete  <br>`callout` <br>  - If the record is owned by System, this option will be disabled.
    