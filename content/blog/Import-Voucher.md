---
title: "Create Vouchers From Excel"
date: 2021-03-19
draft: false
author: "ERP Crew"
description: "Guide to importing vouchers through Excel"
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- voucher
- import through Excel
categories:
- Finance

---
## Introduction
Import Voucher is used to create multiple Payment Vouchers and Receipts in a single pass. 
Traditionally, users would create the Payment Vouchers and Receipts one by one which is time consuming and tedious.

This blog shows you how to use the Import Voucher feature to create multiple Payment Vouchers and Receipts in a single pass, without any hassles.

## Steps for Import Voucher
- Click on the Import Voucher button from the Voucher grid.
![1](/Import-Voucher/importvoucherlink.png)
- From Import Voucher options page, click on the Download model link to download the Excel file for entering the data.
![2](/Import-Voucher/optionspage.png)
- Key in the data in the Excel sheet.
{{< callout type="warning" >}}
Ensure that the numbers do not contain any **commas**.
{{< /callout >}}
- Save the file in CSV format.


![3](/Import-Voucher/VoucherModel.png)
- On the options page, select the Document Type and the Bank/Cash name and then select the file to be uploaded.
- Click on the Upload button which will import all the vouchers and generate an Excel sheet which contains all the voucher details and would display a success or error message.
- If there are any errors in the file then those would be displayed using error codes as described below.
- Guidelines for entering data in the Excel file:

    1. The Reference document must be SI , PB , OA , AD or GL only. (Refer to Error code A)
    
    2. Voucher amounts must not be greater than 999999999.99 (Refer to Error code B)
    
    3. Voucher type must be P-Payment or R-Receipt only. (Refer to Error code C)
    
    4. Reference Date / Cheque Date must be dd-MMM-yy format. (Refer to Error code D)

    5. Mainac and Subac must be valid as per Chart of Accounts.  (Refer to Error code E)
	
    6. Party code must be valid as per Party Master. (Refer to Error code F)

    7. Reference Number / Reference Date must be a valid Invoice Number & Date for the given Party.(Refer to Error code G)

    8. Reference Number / Reference Date must be a valid Bill Number & Date for the given Party.(Refer to Error code H)

    9. Voucher Amount must be equal to the total of the line amounts. (Refer to Error code I)

	1.  Reference Number must be blank for GL, OA & AD. (Refer to Error code J)

    1.  Cash / Bank Balance will go negative after importing the records. (Refer to Error code K)

    2.  Transaction Number is invalid. (Refer to Error code L)

	2.  On the options page, if Document type is selected as GL then the Reference document in the model must be GL. (Refer to Error code M)

	3.  On the options page, if Document type is selected as AR/AP then the Reference document in the model must be SI, PB, OA, AD only. (Refer to Error code N)

    1.  Voucher Amount must be greater than 0. (Refer to Error code O)

    2.  For SI/OA, the Receipt/Payment column must be 'R' and For PB/AD, the Receipt/Payment column must be 'P'. (Refer to Error code P)

    3.  Duplicate Reference document, Reference Number, Reference Date for the same Party. (Refer to Error code Q)

    4.  In case of Reference document 'PB', multiple parties are not allowed in a single transaction. (Refer to Error code R)

    5.  Payment exceeds due amount. (Refer to Error code S)


## Epilog
System creates Payment Vouchers and Receipts for multiple Voucher entries in a snap.











