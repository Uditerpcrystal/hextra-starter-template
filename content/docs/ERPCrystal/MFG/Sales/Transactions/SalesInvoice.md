---
title: "Sales Invoice"
date: 2022-02-26
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
# - SalesInvoice

---

## Introduction
 <!-- {{< callout type="info" >}} {{< /callout >}}  -->
Helps to create and modify Goods & Services types of Invoices with different GST types like Export, Reverse Charge, Domestic, etc. It contains features like Make Debit OR Credit Note, JSON, Email to Customer and Print to PDF.
<!-- Helps to create, modify Goods & Services types of Invoices with different GST types like for Exporter, Reverse Charge, Domestic etc. Its contain features like Make Debit OR Credit Note, JSON, Email to Customer at once click, Print to PDF. -->


#### Mandatory Fields

|Mandatory Fields|   
  |:------|                   
  | Invoice Date / Time <br> - Pre Selected as current date <br> `Validation` - Invoice Date must be between the Financial year's Start Date and the End Date. 
  | Select Supply Type <br> - Goods / Services.
  | Select Invoice From <br> - Select GST Unit Name.
  | Select Place of Supply <br> `Validations` <br> - **Place of Supply (State) is mismatched with GSTIN of Party.**. If selected state's code is not matched with GSTIN No. state code for the selected party in Party Master(System Tools) then this validation will show.  <br> - If invoice type is Export then Place of Supply must me outside from Origin country.
  | Customer/Supplier/Branch <br> `Validation` - **Invoices for this party are blocked in Party Master**. If allow invoice is stopped for selected party in Party Master then this validation will show. 
  | Select Invoice Sub-Type <br> Domestic - For selling of Goods & Services between Business to Customer <br> Export - For selling of Goods & Services to outside the country.  <br> Reverse Charge -  For selling of Goods & Services between Business to Business . <br> E-Commerce , Local Services, etc.
  | Select Transaction Type <br> - If invoice transaction type is already set for the party in Party Master then auto fetch will be done by System. <br> `Validation` <br>**Please set default transaction type in Party Master**. If transaction type is [Not Applicable] in Party Master then you need to select transaction type for the invoice OR you need to change transaction type in Party Master itself for the Party <br> **Please fix invalid A/c head in Transaction Type Master** Selected transaction type A/c head's mainac & subac must be same as Charts of Account mainac, subac.
  | Net Weight
  | Vehicle Details <br> - `Validation` Vehicle No. is mandatory to fill when  mode of transport is road and invoice type is not Reverse Charge.
  | Select Transporter Name <br> - `Validation` - Mandatory to fill when invoice type is not services & GST type is not Reverse Charge.
#### Optional Fields

|Optional Fields|   
  |:------|
  | Discount Rate <br> `Validation` - In Party Master if Apply Discount is Yes, then Discount Rate cannot be 0.
  | Discount Amount <br> `Validation` - Discount must be less then invoice value.
  | Select Freight Type <br> - Select from Freight Options Master.
  | Freight Amount <br> `Validation` - If Freight is set as mandatory in Sales Order, it needs to be entered.
  | Packing / Forwarding
  | Due Date <br> - Due Date is auto computed based on credit days specified in Party Master but maybe 
  overridden. <br> `Validation` - If Due Date is filled manually, it cannot be prior to Invoice Date.
  | Account Particulars <br> `Validation` - Account head needs to be selected when Transaction Type is user defined.
  | Removed Date / Time 
  | Cases
  | Shipping Bill No.
  | Shipping Bill Date
  | Select Currency <br> - Select from Currency Master.
  | FCNR Amount <br> `Validation` - If currency = INR, FCNR amount must be 0. Otherwise more than 0.
  | Exchange Rate <br> `Validation` - When invoice sub-type is Export and currency is Non INR then exchange rate must be more than 0.
  | Load Factor <br> `Validation` - When invoice sub-type is Export and currency is Non INR then load factor must be between 1 to 10.
  | Select Mode <br> - Road, Rail, Ocean, Air. <br> `Validation` - Vehicle number is mandatory if mode of transport is Road.
  | LR No/Transporter Doc No. <br> `Validation` - Lory receipt number / transporter doc no. need to fill when mode of transport is not road.
  | LR Date/Transporter Doc Date <br> `Validation` - Selected date must be between the Financial year's Start Date and the End Date. 
  | Select Category <br> - Cash, Credit, COD etc.
  | Is Purchase Return <br> Yes / No
  | Year / Bill Reference No <br> `Validation` - If invoice is for return then reference no. must be available in Invoice.
  | Inspection Date
  | Inspection Report
  | Carrier Charges <br> Carrier Charges are linked with the purchase bill
  | Notes
  | **Only For E-Invoicing** <br> - Select E-Invoice UOM 

#### Features

|Features|  
  |:------|
  | Create New 
  | Modify <br> - If document lock is applied to the document, modify option will be disabled. <br> `Validation` <br> - Non standard price can be keyed in only when the following system parameter is set to On <br> In Sales Order, allow non-std price. <br> - If audit trail feature is enabled when an invoice is modified, a valid reason needs to be specified. <br> - Invoice value cannot be negative. The discount specified by the user cannot be more than the invoice value.
  | Delete <br> {{< callout type="info" >}} If document lock is applied to the document, delete option will be disabled. <br> If invoice is linked with Receipt, Debit Credit Note, JV, Hundi, Purchase Bill then delete option will be disabled. {{< /callout >}} <br> `Validation` - Notes needs to be filled.
  | Print / Email <br> - To print / email invoice <br> `Validation` - If bill type is not Reverse Charge then Eway Bill No. needs to be filled.
  | Make SDN / SCN <br> - To create debit credit notes.
  | Reactivate JSON <br> Helps to reactivate the JSON.
  | Modify More Invoice <br> - Helps to update more invoice details like material receipt no, special notes etc.<br> `Validation` - Carrier charges are linked with the purchase bill
  | Bill To / Ship To Details <br> - In order to view Ship to info, you need to 1st update ship to info in Sales Order which is used as 1st line in invoice.
  | Update Ship To from Sales Order <br> Auto update Ship to Details in invoice from Order which Order no.  is used as a 1st line in invoice.
  | L R Number <br> - Download lorry receipt (LR) in PDF format


#### Item Details - Mandatory Fields

|Mandatory Fields| 
  |:------|
  | Select Stage <br> - RM, FG,etc.
  | Select Item State <br> - Good, Rejected.
  | Indent No & Indent Date <br> - Need to fill when item state is Rejected and sys paramter is on for auto indent create for rejected qty. <br> `Validations` <br> - Item is not available in the Indent <br> - Indent No / Date does not contain the invoiced item.
  | Select Store Location <br> - Select from Store Master <br> `Validations` - Store Location must be same as the Store Location of invoice line one.
  | Invoiced Qty <br> `Validations` <br> - Invoiced qty must be more than 0 <br> - Invoiced qty can not exceed pending order qty <br> If the following system parameter is on <br> **Invoiced Qty can exceed pending order Qty upto 10%** <br> then invoiced quantity can exceed pending order quantity by 10%. <br> Credit days in Price Master for current line being added, differs from credit days of first item in this invoice. <br> Qty must be available in inventory master for given item.
  | Supplementary Rate <br> Only for reference invoice <br>  `Validations` - Supplementary Rate must be greater than Invoice Rate
  | Packing Info
  | Form `Validations` <br> - Multiple GST tax code, Delivery Location, Store Location are not 
  allowed in a single invoice. <br> - Currency in Sales Order and in Invoice must be the same. <br> If multiple order for party is not active in party master then system will through message <br> As this invoice has references to multiple Orders, Deliver At/Excise/ST Codes must be same in all of them. <br>


#### Item Details - Optional Field

|Optional Fields| 
  |:------|
  | Warranty No, Period <br> End No. must be greater then To No. & must be numbers only
  | Bypass Negative Stock Check <br> - Yes / No <br> `Validation` - If System parameters is set, negative stock check maybe bypass.
   
#### Item Details - Features

|Features|  
  |:------
  | Create New <br> - If document lock is applied to the document, this option will get disabled.
  | Modify <br> - If document lock is applied to the document, this option will get disabled.
  | Delete <br> - If document lock is applied to the document, this option will get disabled. <br> - Delete is disabled if any discount is available in Invoice. 
  | Item Details <br> - To show the list of PO / Item details of Invoices


#### Export Invoice - Mandatory Fields

|Mandatory Fields|  
  |:------
  | Export Invoice No
  | Exporter Ref No
  | Origin
  | Destination
  | Mode
  | Vessel / Flight No.
  | Received At
  | Loading Port
  | Discharge Port
  | Total Pallets
  | Volumetric Weight <br> If Flight No. is By Air is 
  | Total CBM
  | Payment Terms
  | Shipment Terms
  | Is Consignee different? <br> - Yes / No
  | Consignee <br> - If Consignee is different, details are mandatory.
  | Remarks
  | Invoice Declaration
  | Packing List Declaration
 
#### Export Invoice - Optional Field

|Optional Fields| 
  |:------|
  | Remarks

#### Export Invoice - Features

|Features|  
  |:------
  | Create New  
  | Modify
  | Delete <br> `callouts` <br> This item is related to the main invoice line and may not be deleted.
  | Excel Print

  #### Export Invoice Item Details - Mandatory Fields

|Mandatory Fields|  
  |:------
  | Pallet No
  | Series
  | Qty / Box <br>  `Validations` <br> - Qty / Box must be between 1-99999.999 <br> - Qty / Box X No. of boxes must tally with item qty.
  | No. of Boxes
  | Net Weight
  | Gross Weight

  #### Export Invoice Item Details - Features

|Features|  
  |:------
  | Modify
  | `callout` - Export Invoice items are related to main invoice items. Hence options to add any new items / delete are disabled.  

   #### Reverse Charge Item Details - Mandatory Fields
   |Mandatory Fields| 
   |:------
   |Select Item
   |Is this Manual Value? <br> Yes / No
   |Qty <br> Only when manual value selected as No
   |Rate <br> Only when manual value selected as No
   |Value <br> Only when manual value selected as Yes
   |Goods and Service Tax <br> Auto-fetch did not succeed. GST code specified in Inventory Master may NOT be valid
   
   #### Reverse Charge Item Details  - Optional Fields
   |Optional Fields| 
   |:------
   | Non Standard Notes

   #### E-Invoice
   |E-Invoice|
   | :------
   | Steps to create E-Invoice <br> - After creating an Invoice click on Json <br> - The Json file will be downloaded <br> - The user has to login into the GSTIN Portal using his credentials and then upload the Json file
   | `Validation` <br> - There are no lines in this document hence E-invoice can't be generated.   <br> - If E-invoice JSON has already been generated, System prompt appropriate message.   <br> - **Please enter Ship To Party in Sales Order and do update in Invoice**. If ship to info is available in sales order which is referenced in the first line of invoice, you may click on update ship to info from first line of invoice. {{< callout type="info" >}} Steps to update Ship to details <br> - Go to the details of the first item in the invoice to get the order no since Ship to details can only be fetched from the connected orders <br> - Fill the ship to details for that order <br> - Go to that invoice, click on update from first item of invoice link inorder to update the ship to details from connected sales order. {{< /callout >}}   <br> - **Address, Location, Pincode & State are mandatory if E-invoice has Ship To**.Ship to Address, location, pincode & state are needs to be filled in Order, if ship to party name is already filled for the order. <br>  - UOM is mandatory for E-invoice.     <br> - Invoice rate can't have more than 3 decimal places.  <br> - Buyer GSTIN, buyer state, seller state, place of supply must be valid. <br> - **Pincode of the party is invalid** if it is null or its length is not equal to 6 (Only for domestic invoice ) {{< callout type="info" >}}  If there is any error during JSON download, option to reactivate is available. <br> System enables you to download JSON file for a single / range of invoices for a given unit. {{< /callout >}}  

   <!-- JSON -  <br> System enables you to download JSON file for a single / range of invoices for a given unit. -->
