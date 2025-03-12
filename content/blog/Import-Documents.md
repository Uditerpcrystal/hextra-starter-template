---
title: "Import Documents"
date: 2021-03-19
draft: false
author: "ERP Crew"
description: "Guide to create landed cost module through Excel"
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- landed cost
- import through Excel

---
## Introduction
Import Lines link is used to create multiple lines in Import Documents in one go. 
Earlier, users would create the Import Document lines one by one - which is time consuming and tedious.

This article shows you how to use the Import Lines feature to create multiple lines in Import Documents without any hassles.

## Steps for Import Voucher
- Click on the Import Line button from the Import Document Details Page.
![1](/Import-Document/ImportLink.png)
- From import line options page, click on the [Download model] link to download the Excel file for entering the data.
![2](/Import-Document/DownloadModel.png)
- Key in the data in the Excel sheet and then save the file in CSV format. 
    >Note: To key in data, you can take help of Indent Register report.

![3](/Import-Document/Excel.png)
- Select the file to be uploaded. Click on the Upload button which will import all the lines and download an Excel file.
- The above generated file will contain all the import document line details and if everything went fine, would display a success message.
- If there are any errors in the file then those would be displayed using error codes with each error code has a special meaning.
- Points for entering data in the Excel file:

    1. The Weight / CBM must be greater than 0 and less than 9999999.99 (Refer Error code A)

    2. If Landed cost is already done against related indent, you can not add a line with that indent. (Refer Error code B)

    3. If Party is mismatched between Import Document and related Indent, then it would show the error as Party is Mismatched. (Refer Error code C)

    4. If Quantity of related GRN and Indent is different, then it would show the error as Quantity is mismatched between GRN Quantity and Indent Quantity. (Refer Error code D)

    5. If Foreign Currency rate is zero in an already converted Indent Line, then it would show this error. (Refer Error code E)

    6. In related Indent Line, if the Foreign Currency rate is zero, then it would show this error. (Refer Error Code F)


## Epilog
System creates Import Document with multiple Lines in a few seconds from Excel data.
This feature will come in handy when you have several hundreds of lines in a single import purchase document.









