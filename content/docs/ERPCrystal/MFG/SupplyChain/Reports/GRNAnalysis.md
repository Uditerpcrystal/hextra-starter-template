---
title: "GRN Analysis"
date: 2022-01-21
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
# - SupplyChainModule
# - GRNAnalysis

---
## Introduction

This feature helps to analyze unit wise pending GRN, GRNs billed, QA protocol report etc.

#### Options

|Options|   
  |:------|
  | Select Report Type  <br> - Pending GRN, GRNs Billed, GRN Register etc.
  | Select Party Group  <br> - Select from Party Group
  | Select Party Name  <br> - Select from Party Master
  | Select Item Group  <br> - Select from Item Group Master
  | Select Item Name  <br> - Select from Inventory Master
  | Select Unit <br> - Select GST Units
  | From Date 
  | To Date  <br> `Validation` <br> - Gap between date range should not exceed two years. <br> - **Invalid date range.** If From Date is earlier than To Date  <br> - Future dates are not allowed
  | Consider Bill Date Upto

#### Reports available under GRN Analysis are listed below

|Reports|   
  |:------|
  | 1. Pending Grn <br> - This report shows pending GRN by showing details like Grn type, Grn qty, pending qty, rate etc.
  | 2. GRNs Billed <br> - This report helps to analyse information about GRN bills by showing Grn qty, bill qty, bill no. etc.
  | 3. GRN Register <br> - It displays the goods receiving data entered in the system for selected unit and given date range.
  | 4. QA Rejection Report <br> - This report shows the information about rejected indents with details like QA remarks, rejected qty, QA report no. etc.
  | 5. QA Protocol Report <br> - It dispalys the QA protocol report with detailed information for various parties.
  | 6. Sales Rejection <br> - 6.1. Sales Rejection Report : This report shows sales rejection details by showing party name, ref no, status and sales officer etc. <br> - 6.2. Sales Rejection Details : This report gives detailed information of sales rejection.

