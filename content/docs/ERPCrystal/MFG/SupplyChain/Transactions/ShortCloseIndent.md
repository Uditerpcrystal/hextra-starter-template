---
title: "Short Close Indent"
date: 2022-01-18
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight  : 8
# tags: 
# - ERPCore 
# - SupplyChainModule
# - Short Close Indent

---

## Introduction

This feature helps to download the System computed Pending indents records basis on their Qty and Age. By using System generated Pending indents report, We can Update the indent status as EXPIRED using import button by uploading the same generated report.
<!-- This feature manage to close left over quantities of pending indents. -->

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Select Report Type <br> - Pre selected as Oty (Qty, Age)
  | Qty / Age <br> `Validations` <br> - Pending qty should be between 0 and 10. <br> - Pending indent have to be at least 60 days old <br> Value is Invalid
  | From Date
  | To Date <br> `Validations` <br> - Invalid date range (If To Date is before the From Date) <br> - Future dates are not allowed. <br> - Gap between date range may not exceed 2 years.
   <!-- | Year <br> - Select from year combo box. -->

#### Features

|Features|   
  |:------|
  | Submit
  | Details <br> `callout`  <br> - In Indent status master,there is no existing status as 'EXPIRED'.
  | Import <br> `Validation` <br>  - Uploaded file name should be ShortCloseIndents
