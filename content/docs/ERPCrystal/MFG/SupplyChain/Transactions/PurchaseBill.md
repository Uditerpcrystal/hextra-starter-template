---
title: "Purchase Bill"
date: 2022-01-18
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 4
# tags: 
# - ERPCore 
# - SupplyChainModule
# - Purchase Bills

---

## Introduction 

This feature helps to record purchase bills for goods and services.

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Year <br> - Pre-Selected current fiscal year
  | System Bill Date <br> - Pre selected as current date <br> `Validation` <br> - Date must be between FY Start and FY End
  | Bill Sub-Typ <br> - Pre selected as Direct Purchase(Direct Purchase, Imported Purchase, Purchase - Reverse Charge.)
  | Purchasing Unit <br> - Select GST Unit Name.
  | Supply From <br> - Select states from State Name  <br> `Validation` <br>- Supply from (State) is mismatched with GSTIN of Party <br> - Supply from has to be 'Outside India' for GST type = Imported Purchase.
  | Customer/Supplier/Branch <br> - Select from Party Name.
  | Input Tax Credit <br> - Pre selected as Is Eligible (Is Eligible, NA, Not Eligible.)
  | Is E-Invoice Submitted? <br> - Pre selected as No( Yes / No ) <br> `Validation` <br> - Submission of E-Invoice is mandatory.
  | Is RCM Applicable? <br> - Pre selected as No( Yes / No )
  | Type of Input <br> - Pre-Selected as Not Applicable (Not Applicable, Import - Raw Material, Import - Capital Goods, Import -    Services , Domestic - Raw Material, Domestic - Capital Goods, Domestic - Services) <br> `Validation` <br> - For Imported purchase, type of import must be specified.
  | Discount %
  | Ad-hoc / Discount Amount
  | Round-off
  | Supplier Bill No
  | Supplier Bill Date <br> `Validation` <br>- Supplier bill date cannot be later than bill date.
  | Supplier Bill Value <br> `Validation`<br> - Supplier bill value must be greater than zero
  | Transaction Type <br> - Select  Transaction Type <br> `Validation` <br> - Please set default transaction type in Party Master (If Transaction Type is Auto Fetch From Party Master.)
  | TCS
  | Freight Type <br> - Pre selected as By Ocean - FCA(Options as per Freight master) 
  | Freight,Octroi,Carriage & Packing
  | Currency <br> - Pre selected as INR (Options as per Currency Master) .
  | FCNR Amount <br> `Validations` <br> - FCNR amount may not be zero (If selected currency is Non-INR) <br> - FCNR amount must be zero
  | **Only for Bill payment status** <br> Ok To Pay <br> - Yes / No
  | **Only for Revoke Authorization** <br> Revoke <br> - Yes / No
  | **Only for Modify Other Info** <br> GST Reco Status <br> - Not Set

 <!--
  |System Bill Date <br> `Validation` - Date must be between 01-Apr-21 AND 31-Mar-22
  | Purchasing Unit <br> - Select GST unit.
  | Supply From <br> - Select states from State Master  
  | Customer/Supplier/Branch <br> - Select from party Master.
  | Transaction Type <br> - Select from TransactionType  
  | Freight Type <br> - Select from Freight Master
  | Currency <br> - Select from Currency Master.
  -->

#### Optional Fields

|Optional Fields|   
  |:------|
  | Original Bill No (if Supplementary)
  | E-Way Bill No
  | Account Particulars <br> - Select Account Particulars  <br> `Validation` <br>- A/c head needs to be selected for User Defined transaction type (If Transaction Type is User Defined)  <br> - Please fix invalid A/c head in Transaction Type Master
  | TDS A/c Code (If Applicable) <br> - Select from the list of party master.
  | Due Date
  |  **Only For Duplicate Supplier Bill No** <br> Go ahead?  <br> - Yes/No
  | L R No
  | L R Date
  | Port Code / BE No <br> `Validation` <br>- For imported purchase, port no / BE no must be specified.
  | BE Date
  | **Job Work Details** <br> - Jobwork Challan No. <br> `Validation` <br> - **As this item was sent directly to the jobworker, challan No. & date must be specified in the purchase bill.** In Job work module when material is directly send to the Job Worker , you have to key in the ship to party as per the indent  and then this Annexure No and Annexure Date has to be mentioned in the Purchase Bill. <br> -  Jobwork Challan Date
  | Notes for Authorization
  | Notes
  | **Only for Modify Other Info** <br> - Availed in 3B on <br> - Shown in 2B on
<!-- 
| Account Particulars <br> - Select from Chart Of Accounts Master <br> `Validation` - Invalid accounts codes .Please select valid accounts codes

 -->
#### Features 

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If lock is applied to the document, this option will be disabled. <br> - If payment is already made, this option will be disable.
  | Delete <br> - If lock is applied to the document, this option will be disabled. <br> - If LC is made against document, this option will be disable <br> - If debit / credit note is already made, this option will be disabled  <br> - If payment is already made, this option will be disabled. <br> `callouts`  <br> - If you delete this record, cost allocation details, if any, would be removed. <br> - Journal entry has already been made in the System, this option will be disabled.<br> - Debitcredit Note has already been made in the System. You may NOT delete this record... <br> - Payment has already been made against this indent. You may not modify or delete it.<br> - Hundi has already been made in the System. You may NOT delete this record... <br> - LC has already been made in the System. You may NOT delete this record...
  | Details <br>`callout`<br> - There is difference between System Bill Amount & Supplier Bill Amount . 
  | Make PDN/PCN <br> - To create debit/credit notes 
  | Modify Other Info <br> - To update additional details like GST reco status, availed in 3B on (date), shown in 2B on (date)
  | Revoke Authorization <br> - To revoke authorization for the bill.
  | Related Voucher <br> - To view, create and modify voucher account details
  | GRN/Indent Info <br> - To show list of purchase bill GRN Info
  | Cost Allocation <br> - Helps to allocate and De-allocate to the cost center
  | Bill payment status <br> - To show purchase bill details to change payment status
  | Related Import No <br> - To display related import document details

#### Bill Item - Mandatory Fields 

|Mandatory Fields|   
  |:------|                   
  | Quantity Billed Now <br> `Validations` <br> - Quantity billed must be greater than zero <br> - Billed Qty can not exceed Grn pending qty.
  | **Only for Add Line without GRN Refernce** <br> Item <br> - Select from Inventory Master. <br> GST Code <br> - Select from GST Rates Master <br> Value <br> `Validation` <br> - Value must be between 1 and 999999999.99  <br>  Taxable Value

#### Bill Item - Optional Fields

|Optional Fields|   
  |:------|
  | **Only for Add Line without GRN Reference** <br> - Non Standard Item Name
  | Customer / Supplier <br> - Select from Party Master
  | Reference Import Bill No <br> `Validation` <br>  - Given import bill No for this party is not available
  | HSN / SAC Code <br> `Validation`  <br> - Length of HSN code in inventory master must be between 2 to 8 characters. <br> `Validation` <br>   - HSN code is not present in Inventory Master, Please key in HSN code

  
#### Bill Item - Features

|Features|  
  |:------|
  | Create New <br> - If LC is made against document, this option will be disable
  | Modify <br> - If lock is applied to the document, this option will be disabled.
  | Delete <br> - If lock is applied to the document, this option will be disabled.
  | Next Line
  | Add Line without GRN Refernce <br> - To create a record without GRN.

[How to create a Purchase Bill ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/walkthroughpurchasebills/)