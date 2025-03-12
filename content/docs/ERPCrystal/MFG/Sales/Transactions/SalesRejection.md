---
title: "Sales Rejection"
date: 2022-01-11
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
# - SalesModule
# - SalesRejection

---

## Introduction

This feature helps to keep the record of goods that are rejected and returned by customers.
#### Mandatory Fields

|Mandatory Fields|   
  |:------|
  | Year <br> - Pre Selected as current fiscal year                   
  | Select Customer
  | Select Branch <br> `Validations`- First need to select the Party name then branch name.
  | Customer Document Type <br> - Pre Selected as NA (NA, Invoice, Challan, Debit Note, Email).
  | Value as per party <br> `Validation` - Amount needs to be between 0.01 - 999999999.99
  | Status <br> - Pending, Closed <br> `Validations` - For Closed Status, Total Qty of In [Customer] & Out [Customer] must be tallied.

#### Optional Fields

|Optional Fields|   
  |:------|
  | Customer Document No
  | Customer Document Date <br> - Pre Selected as current date
  | QA Report No
  | QA Report Date
  | Do you want to update stock? <br> - Pre Selected as No (Yes, No) <br> `callout` - If Yes, System will update in the rejected goods inventory.
  | Rack Info 
  | In/Out No  <br> `Validation` <br> - In / Out no. must be available in In / Out Register for the selected party. <br> - In / Out no. is already used with another Sales Return. <br> - Document type must be as PB and In / Out type as I  in In / Out Register for given In/out no.
  
    

#### Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If the document status is closed, modify option will be disabled.
  | Delete <br> - If the document is status closed, delete option will be disabled.
  | **Print** <br> Select Report Type : Document, Analysis <br> Document No <br> From Date <br> To Date <br> `Validations` <br> - Invalid date range <br> - Future dates are not allowed <br> - Gap between date range may not exceed 2 years.

#### Item - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Date <br> - Pre Selected as current date.
  | Item <br> `Validations` - If transaction type is related to return like Replacement Given, Sent Back To The Customer, etc. then item must be already exist in Sales return.
  | Select Brand Name <br> - NA, FULHAM,etc.
  | Actual Qty <br> `Validations` <br> - Qty can not be zero <br> - Qty needs to be between 0.001 - 9999999.999.
  | Transaction Type <br> - Pre Selected as Advance Replacement (Advance Replacement, Out of Warranty, Replacement Given, Return to Vendor etc.)
  | Document Type  <br> - Pre Selected as NA (NA, Invoice, Challan, Credit Note, Purchase Bill) <br> `Validations` <br> - If transaction type selected as [Credit Note Given] then Document Type must be Credit Note. <br> - If transaction type selected as [Purchase Bill Booked] then Document Type must be Purchase Bill.<br> - For selected Document type, Document no. must be available for the selected party as given document date.
   <!-- | Document Type <br> - Invoice, Challan, Credit Note <br> - Error code C - Incorrect doc type <br> `Validations` - If transaction type is selected as credit note given, document type must be credit note <br> - If transaction type is selected as purchase bill booked, document type must be purchase bill  -->
   
 
  

#### Item - Optional Fields

|Optional Fields|   
  |:------|
  | Challan Qty (as per customer)
  | Document No.<br> `Validations` - When transaction type is selected as [Advance Replacement,Credit Note Given,Replacement Given,Purchase Bill Booked] then Document No. is mandatory to filled
  | Document Date
  | Document Value
  | Updated On
  | Batch Code
  | Customer Rate
  | Notes

### Item - Features

|Features|  
  |:------
  | Create New <br> - If the document status is closed , this option will be disabled
  | Modify <br> - If the document is completed, this option will be disabled
  | Delete <br> - If the document is completed , this option will be disabled <br> `Validation` - You may not delete this document as it is linked to Purchase Bill
  | Import SRN <br> - To import/upload excel file in specific format for sales rejection. <br> `Validation`<br> - Uploaded file name should be ImportSRN and type of file must be in .csv file <br> - If the document status is closed , this option will be disabled
  | **Only for Warranty Info** <br>- If status is closed then this option will be disabled. <br> - To modify warranty information like warranty qty, ok qty, not ok qty, repaired etc.
  | Srn No <br> - Sales rejection number auto fetched from main document
  | Warranty Qty <br> `Validation` - Addition of ok qty and not ok qty should be equal to warranty qty.
  | OK Qty
  | Not OK Qty
  | Repaired
  | Scrapped <br> `Validation` - Repaired and scrapped qty should be equal to not ok qty.
  | Out Of Warranty Qty <br> `Validation` - Addition of ok qty and not ok qty should be equal to out Of warranty qty.
  | OK Qty
  | Not OK Qty

