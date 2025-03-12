---
title: "Contribution Analysis"
date: 2022-01-14
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
# - SalesModule
# - ContributionAnalysis

---
## Introduction

This feature helps to analyze product wise contribution by Weighted Average Cost, Last Purchase Cost, Transfer Price.

#### Options

|Options|   
  |:------|
  | Select Report Type <br> - Contribution By Weighted Average Cost, Contribution By Transfer Price etc.
  | Select Item Group <br> - Select from Item Group master.
  | Select Item Short Name <br> - Select from Inventory master.
  | From Date
  | To Date <br> `Validations` <br> - Gap between date range may not exceed two year <br> - If To Date is selected prior to From Date then this Validation will show "Invalid Date Range". <br> - If To Date is selected later to Current Date then this Validation will show "Future dates are not allowed".


#### Reports available under Sales Analysis are listed below

|Reports|   
  |:------|
  | 1. Contribution By Weighted Average Cost <br> - 1.1. Contribution By Sales : This report shows per unit contribution margin, total, percentage with grand total for sales of items. <br> - 1.2. Contribution By Product : This report compares the profitability of each product by percentage, margin etc. <br> - 1.3. Cost Recovery Report : This report shows recovering costs for various items. 
  | 2. Contribution By Last Purchase Cost <br> - 2.1. Contribution By Sales : This report shows last purchase cost with contribution margin, total, percentage and grand total for sales of items. <br> - 2.2. Contribution By Product : This report compares the profitability of each product by percentage, margin etc. <br> - 2.3. Cost Recovery Report : This report shows recovering costs for various items.
  | 3. Contribution By Transfer Price <br> - This report displays Contribution of transfer price for various items with qty, value, rate along with other details.
  | 4. Transfer Price Master <br> - This report displays transfer price for various items with WEF date.
  <!-- 4.1. This report display transfer price for various items with WEF date. -->
  <!-- 3.1. report display Contribution of transfer price for various items with qty, value, rate along with other details. -->



