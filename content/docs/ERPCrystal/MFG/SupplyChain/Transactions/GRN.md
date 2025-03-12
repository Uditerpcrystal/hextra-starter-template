---
title: "GRN"
date: 2022-01-18
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
# - GRN

---

## Introduction 

Goods received note (GRN), is a two-way document that acknowledges the delivery of goods by a supplier and their receipt by the customer.Goods received note confirms that an order has been delivered and received and it’s satisfactory to all the parties involved.
<!-- This feature helps to record goods received from suppliers. -->

#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Year <br> - Pre-Selected current fiscal year.
  | GRN Date <br> - Pre-Selected as current date. <br>`Validation` <br>- **Date must be between FY Start and FY End** If the selected date is outside Fiscal Year 
  | GRN Type <br> - Pre selected as Purchase (Purchase, Manufacturing etc)
  | GRN From <br> - Select GST Unit Name
  | Customer/Supplier <br> - Select Party Name
  | Branch <br> - Select Branch Name for the selected Party
  | Transporter Name <br> - Select Transporter Name


#### Optional Fields

|Optional Fields|   
  |:------|
  | Inspection Report No
  | Inspection Report Date <br> - Pre selected as current date
  | Reference No
  | Reference Date<br> - Pre selected as current date
  | In / Out No  <br> `Validation` <br>- Party/Unit must be same as indent and must be present  In / Out register. <br> - Document type must be Purchase Bill (PB). <br> - In/Out No is already linked to another Grn No.
  | In / Out Date <br> - Pre selected as current date
  | Supplier Chalan No
  | Supplier Chalan Date <br> - Pre selected as current date
  | Notes

#### Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If lock is applied to the document, this option will be disabled.
  | Delete <br> - If lock is applied to the document, this option will be disabled.
  | Print <br> - To download PDF of GRN
  | Print Excel


#### GRN Item - Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Quantity Received
  | Qty Accepted <br> `Validations` <br> - Qty must be between 0.001 - 9999999.999 <br> - Accepted qty can not exceed Received Qty. <br> - Accepted qty can not exceed pending indent qty   
  | Store Location <br> - Select Store Name


#### GRN Item - Optional Fields

|Optional Fields|   
  |:------|
  | Batch No
  | Pallet No <br> `Validation` <br>   - Invalid format.
  | Stores In-charge's Note (if any) <br> `Validation`<br>  - Please key in suitable remarks as qty accepted is lower than qty received..


#### GRN Item - Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If lock is applied to the document, this option will be disabled.
  | Delete <br> - If lock is applied to the document, this option will be disabled.
  | Indent Info <br> - Shows list of GRN indent details.  

[ How to create a GRN ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/walkthroughgrn/)