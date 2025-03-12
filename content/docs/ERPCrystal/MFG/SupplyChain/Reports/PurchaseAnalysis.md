---
title: "Purchase Analysis"
date: 2022-01-21
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
# - SupplyChainModule
# - PurchaseAnalysis

---
## Introduction

This feature helps to analyze purchase by different factors.

#### Options

|Options|   
  |:------|
  | Select Report Type <br> - Purchase By Bill, Purchase By Product, TDS Payable etc.
  | Select Party Group <br> - Select from Party Group
  | Select Party Name <br> - Select from Party Master
  | Select Item Group <br> - Select from Item Group Master
  | Select Item Name <br> - Select from Item Master
  | Select Unit <br> - Select GST Units
  | From Date 
  | To Date <br> `Validation`  <br> - Gap between date range should not exceed two years. <br> - **Invalid date range.**  If From Date is earlier than To Date. <br> - Future dates are not allowed.
  | Bill Type <br> - GST Bill, Bill has both excise and sales tax etc. 
  <!-- | Year -->

#### Reports available under Purchase Analysis are listed below

|Reports|   
  |:------|
  | 1. Purchase By Bill <br> - 1.1. Purchase By Bill : This report will show information of the parties who had directly done the purchase by bill and also show details like unit, tax amounts, supplier bill no, GSTIN etc. <br> - 1.2. DNCN : This report displays the purchase debit credit notes with other details. <br> - 1.3. Purchase By Account Head : This report shows details of the purchase done by account head with other details like trn type, ac codes, ac name, basic amount etc. <br> - 1.4. ITC : Input Tax Credit report shows the credit of the GST paid on purchase of goods and services.
  | 2. Purchase By Product <br> - 2.1. Purchase By Product : This report provides insight into the purchases made for various items and focusing mainly on quantity and cost. <br> - 2.2. Item Wise Summary : It will display the summary of quantity and value item wise. <br> - 2.3. Itemgroup Wise Summary : This report shows item group code wise summary for purchases. <br> - 2.4. Party Wise Summary : This report gives party wise summary by displaying details like party shortname and value.
  | 3. Month-Wise Summary <br> - It will show the month and financial year wise summary for purchases made with different taxes and total amount.
  | 4. TDS Payable <br> - This report shows AC name, bill amount, TDS %, basic and tax amounts and finally TDS amount for various parties.
  | 5. TCS Payable/Receivable <br> - 5.1. TCS Payable : This report displays total amount of tax collected from parties. <br> - 5.2. TCS Receivable : It will dispaly the total amount for TCS received.
  | 6. GST Bills Payment Details  <br> - This report displays GST bills payment details for various parties unit wise.
  | 7. Bill-Wise QA Analysis <br> - It will show bill-wise QA analysis for various parties.

