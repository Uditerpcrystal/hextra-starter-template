---
title: "Import Adjustments"
date: 2021-03-19
draft: false
author: "ERP Crew"
description: "Automatic Reconciliation of Import Adjustment A/c"
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- import adjustment a/c

---
## Import Purchase Accounting
In case of Import Purchase transactions, purchases are made from the main foreign vendor who supplies the material. Further other vendors provide services of transportation, clearing and forwarding etc. 

When we create the landed cost working in the System, we are adding all such expenses like clearing, forwarding, duty etc. and hence the purchase bill of the main foreign vendor is inflated by such expenses also. So the foreign vendor's account gets debited by the gross amount, in stead of the basic cost.

Users have to create several JVs and use Suspense accounts to reconcile the balances. The Import Adjustment Account feature has been designed to eliminate the need for such reconcilitation and to simplify booking of import transactions. 

This blog shows you how to use the Import Adjustment Account to automatically reconcile your books without any hassles.

## Assumptions
- Indent on the Party in foreign currency has been created already.
- GRN for this Indent has been done on receipt of consignment.
- Import document for this consignment is already booked in the System and the indent rates have been updated. 
- Bills for the foreign vendor has been created at the gross value i.e. basic cost plus other service expenses like CLF, freight.
- Bills from service vendors have also been booked in the System.

## Steps for Reconciliation
 ### To link the transaction type to the Chart of Accounts
  - From the Menu, select **Finance** >> **Chart of Accounts**
  - At the bottom of the grid, select **Transaction Type Master** link
    ![1](/Import-Adjustments/trntypemstlink.png)
  - Select **Import Purchase Adjustment Account**
    ![2](/Import-Adjustments/trntypemstgrid.png)
  - Modify and link the Account code to the Trn type **Import Adjustment A/C**
    <!-- ![3](/Import-Adjustments/trntypeACC.png) -->
    >Note: Linking of Account code to the Transaction Type Master is a one time process.
    
### Link Service Bill to Main Import Bill
  - Open the Service vendor's bill
  - Select the bill line which is to be linked
    ![4](/Import-Adjustments/servicevendorline.png)
    >Note: If Service vendor bill is related to more than one main vendor's bill, then split the particular expense into several lines and you can link each line to a different main vendor's bill.
  - Select the Customer / Supplier and key in the reference bill no. and click Save.
    ![5](/Import-Adjustments/connectmainbill.png)
    >Note: The reference import bill no. is to be specified as Year billno. eg. 202021 (Financial year) followed by 003808 (System Bill no.)

### Modify TRN Type in Service Vendor Bill
  - At the document level, Select **Modify Other Info** link
  - Select the transaction type as **Import Purchase Adjustment A/c** and click Save
    ![6](/Import-Adjustments/modifyotherinfo.png)
    >Note: TRN Type - Import Adjustment Account will be available only if you have linked ALL lines of the service vendor's bill to the main vendor's bill.

### Epilog
System creates debit entries in the main vendor's account for every line that you have linked in the service vendor's bill.
The contra effect will be given in the Import Adjustment Account.
The Import Adjustment Account balance will always be zero. 
You no longer need to pass any journal entries or do any reconciliation!













