---
title: "Sales Order"
date: 2022-02-26
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
# - SalesModule
# - SalesOrder
---

## Introduction
Sales Order helps to create, view, modify, delete different types of orders like Proforma Invoice, Quotation, Direct Orders. It also contains other features like Email to Customer and Print to PDF.
<!-- Sales Order helps to create, view, modify, delete orders received from customers.  -->

#### Mandatory Fields

|Mandatory Fields|  
  |:------|   
  | Year <br> - Pre Selected as current year.
  | Created On <br> - Pre Selected as current date <br> `Validation` - Date Must be between F.Y. Start Date and End Date |
  | Select Order Type <br> - Pre-Selected as Direct (Direct, Proforma Invoice, Quotation)|
  | Select Order From  <br> - Select GST Unit Name |
  | Select Place of Supply | 
  | Customer/Supplier/Branch <br> `Validation` - If Party type is Registered, Valid GST Registration No. must be entered  in Party Master  |
  | Customer PO Number <br> {{< callout type="info" >}} If same Customer PO Number exists, System prompts appropriate message. {{< /callout >}}  |
  | Currency <br> - Pre-Selected as INR (Options as per Currency Master) |
  | Order Category <br> - Pre-Selected as OTHERS (OTHERS, Replacement, SAMPLES, VIP) |
  | Salesman <br> - Pre-Selected as Auto-Fetch (Options as per Salesmen Master) |
  | Is Freight Mandatory? <br>  - Pre-Selected as No (Yes, No) |
  | Select Freight Type <br> - Pre-Selected as NIL (Options as per Freight Master) |
  | Form `Validations` <br> - Outstanding exceeds credit limit.

#### Optional Fields

|Optional Fields| 
  |:------|
  | Deliver At <br> `Validation` - Ordering and Delivery branches should be that of same customer. |
  | Ship To Party Name (Optional)
  | Bypass Duplicate PO Number? <br> - If customer PO No. is duplicate the System will give callout message if you really want to submit then select yes.
  | PO Date  <br> `Validation` - PO Date cannot be later than Order Date. |
  | Required By <br> `Validation` - Required By cannot be before Order Date. |
  | Freight Amount |
  | No. of Installations |
  | Change Payment Terms for this Order  <br> - This option will show only when System Parameter [Show Pay Terms in Orders] is ON. | 
  | TCS Code 
  | Discount Amount <br> `Validations` <br> - May not be more than order value. <br> - Discount must be zero if there are no lines in the order |
  | Notes |
  <!-- | Sales Enquiry No. <br> `Validation` - Must exist in Sales Enquiry Table.  | -->
  <!-- | Select Payment Term / Credit Days <br> - If System parameter is on, master value from Party Master can be overridden. | -->
  

#### Features

|Features|   
  |:------|
  | Create New 
  | Modify <br> - If Invoice is already created, this option will be disabled.
  | Delete <br> - If Invoice is already created, this option will be disabled. <br> - If document is linked to Advance License, this option will be disabled. <br> - Relevant notes needs to be filled before deletion.
  | Make Invoice <br> `Validations` <!-- <br> - HSN / SAC Code is not available in Inventory Master. --> <br> - Status of all lines in this Order must be OK. <br> - GST code of all lines in this Order must be the same. <br> - If invoice will result in Negative Stock then it will be aborted. <br> - Invoice cannot be made for this Party if allow invoice is 'No' in Party Master, . <br> - Invoice cannot be made for order type Proforma Invoice. <br> - If one or more lines in an order is already invoiced, then Make Invoice cannot be used. <br> - Currency must be only INR.
  | Convert To Order <br> - Helps to Convert Proforma Invoice or Quotation into Confirmed Order. <br> - This feature only will show when order type is Proforma Invoice or Quotation in Modify Page.
  | Order Pay Terms <br> - Helps to change payment terms & credit days.
  | Print <br> - To print Proforma Invoice / Order Confirmation / Quotation.
  | Email <br> `Validations` <br> - **Please create new record in Standard Instructions for Sales Order Email**. If Standard Instruction is not available for Document type Email in Standard Instruction(Supply Chain Module) then this Validation will show. <br> - **Type of Contact must be Orders to sent Sales Order Email** . Contact details needs to available for the party in Contact Master (System Tools Module).In Contact Master contact type must be available in Multiple or Orders.
  | PO Number <br> - To download scanned PO details uploaded in System.
  | Create/Modify Ship to info <br> - To Create/Update shipping info before/after invoicing is done.<br> `Validations` - GSTIN No. must be in valid format.<br>Fields are needed to be filled in page i.e., GSTIN No., Party Name, Address, Location, Pincode, State.
 | Negative Stock. <br> - To view list of items with negative stock.

#### Item Details - Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Select Order Status <br> - Pre Selected as OK (Options as per Order Status Master)
  | Select Item <br> {{< callout type="info" >}} BOM is not available for this product, in the System... {{< /callout >}} <br> `Validation` - HSN / SAC Code is not available in Inventory Master
  | Select Brand Name
  | Qty  | 
  | Rate <br> {{< callout type="info" >}} Auto fetched from Price Master based on customer, item, brand & currency. <br> Rate will be validated from Price Master. {{< /callout >}}  <br> `Validations` <br> - Rate should be greater then 0 in Price Master <br> - Rate can not be 0 for Non Standard Item.
  | Is this Non Standard Item? <br> - Yes / No <br> - If System Parameter is on, Price Master rate can be overridden. 
  | Lead Time <br> {{< callout type="info" >}} Auto fetched from Inventory Master. {{< /callout >}}
  #### Item Details - Optional Fields
  
|Optional Fields|  
  |:------|
  | GST Code <br> - Auto fetched from GST master <br> `Validations` <br> - In Inventory master GST Code must available for the selected item. <br> - GST Code must be same as GST Code of 1st line in Order.
  | Required By
  | Effective Date <br> - Date on which age of the Order is determined.<br> - Effective date may be as Order Date, PO Date, Required Date.
  | Planned Date <br> - Scheduled date for production
  | MRP <br> - Maximum Retail Price
  | Is this Elephant Order? <br> - Yes / No
  | Non Standard Item Name 
  | PR No <br> - Purchase Requisition Number
  | PR Date <br> - Purchase Requisition Date
  | CPS No 
  | CPS Date
  | Warranty(Years)
  | Notes
  | Re-update price from Price Master? <br> - Yes / No
  | Reserved Qty
  | Factor <br> `Validation` - If currency = INR, must be 1. Otherwise more than 1.

#### Item Details - Features

|Features| 
  |:------|
  | Create New <br> {{< callout type="info" >}} If item is already invoiced, this option will be disabled. {{< /callout >}} 
  | Modify <br>{{< callout type="info" >}}  If item is already invoiced, this option will be disabled. <br> If discount is already entered, this option will get disabled. {{< /callout >}}
  | Delete <br> {{< callout type="info" >}} If item is already invoiced, this option will be disabled. <br> Before deleting a line discount has to be removed. <br> If Order is already linked with Advance License (Supply Chain Module), this option will be disabled. {{< /callout >}} 
  | Next Line <br> - Save and create next line
  | Item Details <br> - Redirect to index of all Sales Order items
  | Allocate MTA (Make To Availability) <br> - Helps to set MTA month, quantity. <br> {{< callout type="info" >}}  MTA Qty can only be amended through Allocate MTA link.{{< /callout >}}<br> `Validation` - Allocated qty can not exceed balance MTA Qty.  
  <!-- {{< callout type="info" >}} {{< /callout >}}  -->
 
