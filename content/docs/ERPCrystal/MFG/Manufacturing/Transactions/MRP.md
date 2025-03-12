---
title: "Materials Requirement Plan"
date: 2022-02-16
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 2
# tags: 
# - ERPCore 
# - ManufacturingModule
# - MRP

---

## Introduction

- Helps to generate material consumption, procurement plan and full kit availability. 
- MRP are created based on the Unti Codes. For every unit a different plan ae created.
- It is also based on the production plan created.

#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Unit <br> - Pre selected as Pune (options as per GST Units)
  | Year <br> - Pre selected as current fiscal year (Select from year combo box)
  | Report Type <br> - Pre selected as Production plan (Production Plan, Procurement Plan, Full Kit Plan)
  | Plan Range From <br> - Select from Plan Details list <br> `Validation` - For full kit, plan range from & plan range to must be same
  | Plan Range To <br> - Select from Plan Details list

#### In Process Stock - Mandatory Fields

<!-- |Mandatory Fields|  
  |:------|
  | Item  <br> - Select from Inventory Master <br> - Error code A -  Invalid itemid <br> - Error code D - Duplicate record <br> - Error code E - Inactive itemid
  | Stage <br> - FG, RM <br> - Error code B - Invalid stage
  | Quantity <br> `Validation` - Qty : Range 0.001 - 99999.999 <br> - Error code C - Qty sould not be negative or greater than 9999999.999  -->

  |Mandatory Fields|  
  |:------|
  | Item  <br> - Select from Inventory Master .
  | Stage <br> - Pre selected as FG (FG, RM.)
  | Quantity <br> `Validation` - Qty : Range 0.001 - 99999.999 .
 

 #### In Process Stock - Features

|Features|   
  |:------|
  | Create New 
  | Modify
  | Delete
  | Import To Excel <br> - To upload budget in csv formate <br> `Validation` - Uploaded file name should be ImportInProcessStock 


  #### Reports available under Materials Requirement Plan are listed below

  |Reports|   
  |:------|
  | 1. Production Plan <br> - 1.1. Production Plan : This report will show the quantity of products that are planned to be manufactured within a date range. <br> - 1.2. Final Production Plan : It will display the final plan qty for products along with plan qty, order qty, stock qty of FG <br> - 1.3. Product Wise Consumption : This report will show the product wise consumption of various items along with Uom, qty. <br> - 1.4. Item Wise Consumption : This report shows customized report which is used to keep track of all products, process, items etc. <br> - 1.5. Item Wise Consumption Summary : It will show the summary of items and its consumption. <br> 1.6. IIRS Qty : This report will show the consumption report for Inventory Issues & Receipts (IIRS) quantity with rack info.
  | 2. Procurement Plan <br> - 2.1. Procurement Plan : It will show the purchase information of goods and services and also it lists all requirements expected to be procured over a period of time. <br> 2.2. Procurement Based On Max Order : This report displays the the purchase information of goods and services with max order level details.
  | 3. Full kit Plan <br> - 3.1. Fullkit Plan : This report will show plan qty, full kit qty and system qty for all FG items. <br> - 3.2. Fullkit Working : It will display some quantities like plan, full kit, max prdn qty etc details for various FG and RM items with balance.

### Steps to Download a MRP.
- First you need to select the unit code with the given dropdown.
- Then you need to select the year in which you want to create the MRP. Based on the year you will get to select the production plans.
- After you have selected the financial year, you need to select the type of report you want to download. The types you will get to see are the Production plan, Procurement plan and full kit plan.
- Once the report type is selected you need to select the production plans given in the drop-down.
> Note: The Production plans will be displayed based on the financial year you have selected.
- For the full kit plan, the production plans need to be the same.
- Once all the above fields are selected you will get 4 checkboxes.
  1. Add Pending Order Qty [Upto 2 years] to Plan Qty.
  2. Adjust FG Store Stock from Pending Orders.
  3. Adjust RM Store Stock in Procurement.
  4. Scan BOM of Sub Assemblies to Workout Consumption
> Note: By default Adjust RM Store Stock in Procurement will be selected.
- Based on the checkbox you have selected the report will be created.