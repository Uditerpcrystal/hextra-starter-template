---
title: "Sales Analysis"
date: 2022-01-14
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
# - SalesModule
# - SalesAnalysis

---
## Introduction

This feature helps to analyze the sales performance by Product, Invoice, Salesman etc.
<!-- This feature helps to analyze sales performance by Product, Invoice, Salesman etc. -->

#### Options

|Options|   
  |:------|
  | Select Report Type <br> - Sales by invoice, By product, Sales rejection etc. 
  | Payment Term <br> Applicable only for Receipt Against Invoice report type .
  | Select Party Group <br> - Select from Party Group master.
  | Select Party Name <br> - Select from Party master.
  | Select Item Group <br> - Select from Item Group master.
  | Select Item Short Name <br> - Select from Inventory master.
  | Select Unit <br> - Select GST Units
  | From Date 
  | To Date <br> `Validations` <br> - Gap between date range may not exceed two year <br> - If To Date is selected prior to From Date then this Validation will show "Invalid Date Range". <br> - If To Date is selected later to Current Date then this Validation will show "Future dates are not allowed".

#### Reports available under Sales Analysis are listed below

|Reports|   
  |:------|
  | 1. Sales By Invoice <br> - 1.1. Sales By Invoice : Detail report with billing amounts, unit, branch etc. <br> - 1.2. DNCN : This report shows debit and credit notes with other invoice details. <br> - 1.3.Export Invoice : It can display currency, exchange rate, qty, rate, rate in FC, Value in FC for various items.
  | 2. Sales By Product <br> - 2.1. Sales By Product : This report displays sales information by each product sold & generate total amount and grand total. <br> - 2.2. Sales By Product Summary : It can show the summary of sales by product with the grand total of qty and rate. <br> - 2.3. Sales By Party : Generate basic and invoice amount for various direct selling parties. <br> - 2.4. Sales By Product Party : This report displays sales information by each product sold directly by various parties with classification, segment, qty, rate details etc.
  | 3. Receipt Against Invoice <br> - Generate receipt for the invoice report with the details of party name, transporter, A/C name, voucher amount etc.
  | 4. Month-Wise Summary <br> - 4.1. MonthWise Summary : Shows the basic/opening balance for the year and month with different taxes and finally total balance. <br> - 4.2. MonthWise summary Type : Shows the basic/opening balance for the year / month, different taxes and total balance with document type.
  | 5. Dispatch Summary <br> - 5.1. Dispatch Report : This report will show the detailed information about dispatch items for various parties.
  | 6. Freight Vendor Details <br> - This report will show the party, vehicle details, invoice amount, qty etc. of freight vendors.
  | 7. Sales Rejection <br> - 7.1. Sales Rejection Report : This report display information about rejected sales with partyname, branch and status etc. <br> - 7.2. Sales Rejection Details : This report will give detailed information about rejected items.
  | 8. Outstanding In Alternative Currency <br> - Generate outstanding amount and grand total for different currencies.
  <!-- 2.1. Sales By Product : This report display sales information by each product sold & generate total amount and grand total. -->
  <!-- Sales By Product Party : This report display sales information by each product sold directly by various parties with classification, segment, qty, rate details etc. -->
  <!-- Sales Rejection Details : This report wil give detailed information about rejected items. -->
  

  
