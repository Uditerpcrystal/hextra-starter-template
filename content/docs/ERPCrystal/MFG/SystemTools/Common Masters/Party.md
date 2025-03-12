---
title: "Party"
date: 2022-03-28
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
# - SystemToolModule
# - Party   

---

## Introduction

Handle the master data of customer / vendor, branch, GSTIN, PAN, credit period, payment term etc.


#### Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Party Type <br> - Customer, Supplier, Own company Details
  | Party Name <br> `Validation` - Party name may not contain '&'
  | Short Name
  | Party Group <br> - Pre Selected as Export (Options as per Party Group Master)
  | Party Category <br> - Pre Selected as Genral (Options as per Party Category Master)
  | Party Segment  <br> - Select from Party Segment Master
  | Link to A/c (as per chart of accounts) <br> - Customer Control A/C, Pur.Vendors Control A/C, SER.Vendors Control A/C <br> `Validation` - Control account and party type are mismatched
  | PAN No <br> `Validation` - This Pan No. is already in use in another party.
  | Allow Duplicate PAN No? <br> - Yes / No
  | Hundi Mean Date is Applicable ? <br> - Pre Selected as No (Yes , No) <br>- Consider a mean date while arriving at the date of hundi 
  | Hundi Credit Type <br> - Pre Selected as Days (Days, Month)
  | Hundi Credit Period <br> `Validation` - If Hundi credit type is Month, Hundi Credit Period can not be more than 12.
  | Region <br> - NA, Norht, East, South, West etc. 
  | Select Sales Officer <br> - Select from Sales Officer Master 
  | Allow Invoice/Bill To/From <br>- In case of over due outstanding from a customer you may set this parameter as No to prevent any invoice being generated. <br>-If you do not want to accept any bill from vendor, you may set this parameter as No
  | ACES Type <br> - Pre Selected as Manufacture (Manufacture, Importer, Dealer)
  | Credit Period
  | Credit Limit
  | Select Payment Term <br> - Select from Payment Term Master
  | TDS A/c Code (If Applicable) <br> - TDS Exempt (0%), TDS Not Application, TDS on Rent Payable, TDS on Intrest Payable etc.
  | Apply Discount <br> - Yes / No <br> - To apply discount on all Invoices to a customer set this parameter as Y.  
  | Input Tax Credit <br> - Is Eligible, Not Eligible, NA
  | Is E-Invoice Mandatory?  <br> - Yes / No
  | Multiple Orders in Single Invoice <br> - Yes / No <br>- For a given customer if a single invoice contains a single order reference, you may disable this parameter.
  | Invoice Trn Type <br> - Sales A/c Trading, Labour Charges, Purchase A/c Trading etc.
  | Bill Trn Type <br> - Sales A/c Trading, Labour Charges, Purchase A/c Trading etc.


#### Optional Fields

|Optional Fields|  
  |:------| 
  | MSME No.
  | Notes  


####  Features

<!-- |Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete 
  | **Allow Invoice/Bill To/From** <br> Allow Invoice/Bill To/From <br> - Allow, Stop <br> Reason for Allow/Stock Invoice
  | Change Party Type <br> - To modify party type and link to A/c (as per chart of accounts)
  | Export To Excel <br> - To download report in excel format.
  | **Party Group** <br> - To modify Party Group Master <br> Party Group Name  <br> `Validation` - You can not add a new Party Group in this master.
  | **Payment Terms**  <br> - To create Payment Terms Master  <br> - Payment Term Name
  | **Party Category**  <br> - To create Party Category Master   <br> - Category Name
  | **Party Segment** <br> - To create Party Segment Master <br> - Description
  | Bulk Import <br>- To import multiple parties along with thier branches at once. <br>- Bulk Import can be used only when there is no data in the Party Master Table <br> `Validation` - Uploaded CSV file name should be ImportPartyMst -->


  |Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete 
  | **Allow Invoice** <br> Allow Invoice/Bill To/From <br> - Allow, Stop <br> Reason for Allow/Stock Invoice.
  | Change Party Type <br> - To modify party type and link to A/c (as per chart of accounts)
  | Export To Excel <br> - To download report in excel format.
  | **Party Group** <br> - To modify Party Group Master <br> Party Group Name  <br> `Validation` - You can not add a new Party Group in this master.
  | **Payment Terms**  <br> - To create Payment Terms Master <br>- Different payment terms may be defined eg : COD , 50% Advanced <br> - Payment Term Name
  | **Party Category**  <br> - To create Party Category Master   <br> - Category Name
  | **Party Segment** <br> - To create Party Segment Master <br> - Description
  | Bulk Import <br>- To import multiple parties along with thier branches at once. <br>- Bulk Import can be used only when there is no data in the Party Master Table <br> `Validation` - Uploaded CSV file name should be ImportPartyMst.

  ##### To update the credit limit with an approval code.
  - Added a new way to update credit limit in the party with an approval code. This will be shown only when it is turned on from the system parameters.
  - If the system parameter is on for the approval code then a new input field will be shown, where you need to add the given approval code.
  - If the approval code is valid it will update the credit limit for that particular party.
  - To know more you can go to [Approval code](/content/en/docs/ERPCrystal/MFG/SystemTools/Utilities/Approvalcode).


#### Branch Details - Mandatory Fields

|Mandatory Fields|  
  |:------| 
  | Customer / Supplier ID
  | Branch ID
  | Branch Name
  | Address Line 1
  | Address Line 2
  | City
  | State Name <br> - Select from State Master
  | Pin Code
  | ST Registration No
  | CST Registration
  | GST Registration Type <br> - Registered, Unregistered, Composite
  | GSTIN <br> `Validations` <br> - Please specify GSTIN and should have 15 characters. <br> - For Unregistered Party, you cannot have GSTIN. <br> - This GSTIN is already in use in another party.
  | Customer Type <br> - Business, Consumer, Export
  | TCS Code <br> - NA, TCS @ 1% On Scrap, TCS @ 0.075% On sales etc. 
  | Default Excise / Service Tax Code <br> - Select from Excise Rates Master
  | Is LBT Applicable ? <br> - Yes / No
  | Is Road Permit Required? <br> - Not Required, Offline, Online
  | Distance(In KMs)


#### Branch Details - Optional Fields

|Mandatory Fields|  
  |:------| 
  | ECC No / Service Tax No
  | LBT No
  | PLA No
  | Range / Division


####  Branch Details - Features

|Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete   
  