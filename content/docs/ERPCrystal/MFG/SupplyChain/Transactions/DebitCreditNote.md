---
title: "Debit/Credit Note"
date: 2022-01-18
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
# - SupplyChainModule
# - Debit/CreditNotes

---

## Introduction

A Debit / Credit Note  is a document sent by a Buyer / Seller  to the Supplier / Customer, notifying that a Debit / Credit has been made to their account against the goods returned

To create Debit/Credit Notes go to the Sales Invoice (sale module) click on record and in the details page, click on Make SDN/SCN or go to Purchase Bills (supply chain), click on record and in the details page you will see Make PDN/PCN, click on that button and form will get open.

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Document Type <br> - Sales Debit Note, Sales credit Note
  | GST Type <br> - Pre selected as GST (GST, Non GST, TCS)  
  | Category <br> - Pre selected as Against Particular (Against Particular,SI/PB, Adhoc)  <br> `Validations` <br> - If Gst Type is TCS, category must be Adhoc
  | Book this DNCN in Last FY <br> - Pre selected as No(Yes / No) <br> `callout` <br> - Option to book in Last FY is disabled (If System Parameter is off for back dated DNCN)
  | Item (Only for Adhoc DNCN) <br> - Select from Item Master.
  | Transaction Type <br> - Pre selected ( Select from Transaction Type Master.)
  | Remark <br> - Select from Remark Master.
  | Mode <br> - Pre slected as NA (Road, Rail, Air etc.)
  | Currency <br> - Pre selected as INR (Options as per Currency Master).
  | **Only for JSON** <br> Unit <br> - Select from GST units. <br> Document Type <br> - Debit/Credit Number From <br>  To <br> `Validations` <br>  - System is unable to find the range of documents for the unit <br> - One or more of the selected documents are not enabled for e-invoicing.
  | TCS Amount <br> `Validation` <br> - TCS Code can not be 0 (If Gst Type is TCS )
  | Adhoc Value <br> `Validation` <br> - Amount may be filled only for Adhoc Category <br> - In case of TCS Adhoc amount must be 0
  | Freight / Packing
  | Discount
  | FCNR Amount <br> `Validation` <br> - FCNR amount may not be zero (If selected currency is Non-INR)  <br>  - FCNR Amount must be zero (If selected currency is INR)

#### Optional Fields

|Optional Fields|   
  |:------|
  | Document Date <br> `Validation` <br>  - Date must be between FY Start AND FY End
  | TCS Code (If Applicable)  <br> - Pre selected as NOT APPLICABLE (NOT APPLICABLE , TCS on Scrap 1%, TCS on sales, TCS on Scrap 0.75% ) <br> `Validation` <br> - TCS Code can not be Not Applicable ( If TCS Amount is not 0 AND If Gst Type is TCS and TCS code is NA  )
  | Account Particulars <br> - Select from Chart Of Accounts Master
  | Due Date
  | Update Stock <br> - Yes / No
  | Transporter Name <br> - Select from Transporter Master
  | LR No
  | Vehicle Details
  | Eway Bill No
  | No of Boxes
  | Notes
  | **Only for Modify Other Info** <br> - Additional Notes  
  | Reference Invoice / Bill No <br> `Validation`  <br>  - Invoice No. does not belong to this customer <br> - Bill No. does not belong to this supplier
  | `Form Validation` <br> - The total value of this document must be more than zero.

  <!-- | TCS Code (If Applicable) <br> - NA, TCS on Scrap 1%, TCS on sales, TCS on Scrap 0.75% etc. <br> `callout` - TCS Code must be Not Applicable -->

#### Features

|Features|  
  |:------|
  | Modify <br>`callout` <br>  - If lock is applied to the document, this option will be disabled.
  | Delete <br> `callout` <br> - If lock is applied to the document, this option will be disabled. <br> - If document is already linked to a GRN, this option will be disabled. <br> - You have to delete the whole document itself if Only one line is there in this document.
  | Print <br> - To print PDF.
  | Email  <br> `callout` <br> - Please create new record in Standard Instructions for DNCN Email. **If standard notes is not there** <br> - In Contact Master, Type of Contact must be Multiple to sent DNCN Email .**If the party contact is not there in the contact master**
  | JSON <br> `callout` <br> - E-invoice can't be done if 1) It is a PCN / PDN. 2) It is a Non-GST document. <br> - Document Lock has been applied to this document. If JSON is downloded <br> - E-Invoice JSON has already been generated. <br> - There are no lines in this document hence E-invoice can't be generated. If there is no line level . <br> - In case of E-invoice, Freight and Packing Forwarding charges must be zero. <br> - Pincode of the Party is invalid.
  | Modify Other Info <br> - To update additional notes etc
  | Invoice Grid <br> - To show sales invoice index.
  | Bill Grid <br> - To show purchase bill index.


#### Debit/Credit Note Line Create - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Quantity <br> `Validation` <br>  - Qty must be greater then 0 <br> - **System Stock Qty is less than DNCN Qty** If Update Stock Is selected as Yes for the SCN / SDN and  selected item's Stock Qty is less than the qty entered
  | Rate <br> `Validation` <br>  - Rate must be greater then 0
  | Store Location
  | Value <br> `Validations` <br>  - Value needs to be in the format 99999999.99 <br> - Value needs to be greater than zero



#### Debit/Credit Note Line Create - Optional Fields

|Optional Fields|   
  |:------|
  | Non Standard Note
  | **Only for Modify Taxable Value** <br> -  Taxable Value
  | `Form Validation` <br> - Only G type Invoices will be fetched.

  

#### Debit/Credit Note Line Create - Features

|Features|  
  |:------|
  | Create New
  | Delete
  | Modify Taxable Value <br> - To update taxable value.

  [How to create a Debit/Credit Note ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/walkthroughdebitcreditnote/)