---
title: "Short Close Order"
date: 2022-01-10
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
# - ShortCloseOrder

---

## Introduction

This feature helps to download the System computed Pending Orders records on the basis of their Qty and Age. By using System generated Pending orders report, we can Update the order status as EXPIRED using the import button by uploading the same generated report.
<!-- This feature helps download the System computed Pending Orders records basis on their Qty and Age. By using System generated Pending orders report, We can Update the order status as EXPIRED using import button by uploading the same generated report. -->
#### Mandatory Fields

|Mandatory Fields|   
  |:------                  
  | Select Report Type <br> - Qty, Age
  | Qty / Age <br> `Validations` <br> - If Report type selected as Qty then Qty / Age should be between 0 and 10. <br> - If Report type selected as Age then Qty / Age have to be at least 60 days old.
  | From Date
  | To Date <br> `Validations` <br> - Invalid date range <br> - Future dates are not allowed <br> - Gap between date range may not exceed 2 years.
  | Form `Validation` <br> - In Sales Order Status Master, record with description as EXPIRED must be available.
#### Reports available under Short Close Orders are listed below

|Reports|   
  |:------                  
  | Qty <br> - This report shows short close orders by pending quantity with other details like status, PO no etc.
  | Age <br> - It will display age wise pending orders with other details.

#### Features

|Features|  
  |:------|
  | Submit <br> - Helps to download report with the selected type i.e Qty/Age
  | Import <br> - To upload file in format to get report. <br> `Validation` - Uploaded file name should be ShortCloseOrders and file type must be as .csv file.
  




