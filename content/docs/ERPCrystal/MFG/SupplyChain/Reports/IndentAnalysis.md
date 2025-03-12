---
title: "Indent Analysis"
date: 2022-01-20
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
# - SupplyChainModule
# - IndentAnalysis

---
## Introduction

This feature helps to analyze pending indents, vendor performance and indent register.

#### Options

|Options|   
  |:------|
  | Select Report Type <br> - Pending Indents, Vendor Performance, Indent Register.
  | Select Party Group  <br> - Select from Party Group
  | Select Party Name  <br> - Select from Party Master
  | Select Item Group  <br> - Select from Item Group Master
  | Select Item Name  <br> - Select from Inventory Master
  | Select Unit <br> - Select GST units
  | From Date 
  | To Date  <br> `Validations` <br> - Gap between date range should not exceed two years. <br> - **Invalid date range.**  If From Date is earlier than To Date <br> - Future dates are not allowed


#### Reports available under Indent Analysis are listed below

|Reports|   
  |:------|
  | 1. Pending Indents <br> - 1.1 Pending Indent : This report shows pending indents by unit, user qty, pending qty, status etc.<br> 1.2 Color Codes.
  | 2. Vendor Performance <br> - This report displays vendors performance measure by showing details like received/accepted qty, qty rating, delivery rating on qty etc.
  | 3. Indent Register <br> - 3.1. Indent Register : This report shows unit wise indent details for indian currency by party, qty, rate, status, payment terms etc. <br> - 3.2. Foreign Currency Indents : This report shows unit wise indent details for foreign currency by branchname, qty, currency, currency/load factor etc.
