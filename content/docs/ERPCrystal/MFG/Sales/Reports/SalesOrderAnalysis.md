---
title: "Sales Order Analysis"
date: 2022-01-13
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
# tags: 
# - ERPCore 
# - SalesModule
# - SalesOrderAnalysis

---
## Introduction

This feature helps to generate information of Sales Order Register, Pending Orders, Dispatch Plan etc.

#### Options

|Options|   
  |:------|
  | Select Report Type <br> - Pending orders, Dispatch plan, Delivery performance etc.  
  | Select Party Group <br> - Select from Party Group master.
  | Select Party Name <br> - Select from Party master.
  | Select Item Group <br> - Select from Item Group master.
  | Select Item Short Name <br> - Select from Inventory master.
  | Select Unit <br> - Select GST Units
  | From Date 
  | To Date <br> `Validations` <br> - Gap between date range may not exceed two year <br> - If To Date is selected prior to From Date then this Validation will show "Invalid Date Range". <br> - If To Date is selected later to Current Date then this Validation will show "Future dates are not allowed".

#### Reports available under Sales Order Analysis are listed below

|Reports|   
  |:------|
  | 1. Pending Orders <br> This report will display the details of all sales orders made to a party which are not closed by ordered qty, pending qty, payment terms, aging etc.
  | 2. Delivery Performance <br> This report will show shipment history by region, value, order category, days etc.
  | 3. Sales Order Register <br> It will display the sales order whether the status is approved, pending or rejected by unit wise with other details like PO date, rate, qty, category etc. <br> - 3.1. Customer PO details : Shows the customer purchase order details.
  | 4. Dispatch Summary <br> This report will show the summary of dispatches by qty, rate, invoice amount, party & branch name, delivery date etc for the given period.
  | 5. Marketing Activities <br> This report contains set of data related to the marketing process like category, activity type, activity performed, status etc. 
   | 6. Dispatch Plan <br> It will display the dispatch plan for various items with pending qty, dispatch to, standard packing, standard weight etc.
   <!-- | 5. Marketing Activities <br> This report contain set of data related to the marketing process like category, activity type, activity performed, status etc.   -->

  

