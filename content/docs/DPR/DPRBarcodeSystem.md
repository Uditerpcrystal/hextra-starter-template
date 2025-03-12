---
title: "DPR Barcode System"
date: 2023-01-31
description: ""
draft: false
weight: -1
pinned: true
hideToc: false
enableToc: true
enableTocContent: false
---

#### Changes in DPR Purchase Bill
1. Existing Puchase Bill logic will not be disturbed and users will be able to continue to create/modify bills. For Manual entries, System will not create sub-transaction nos based on the no. of boxes.
2. A feature for Importing transaction-wise data through Excel will be provided and all existing UI logic will be handled during Import from Excel.
3. System will create stickers with QR code and specified text info in PDF format after bill is saved.
4. An additional table will be provided to store sub-transactions (Trn No + 3 digit box info). For e.g. if there are 50 boxes of a given item, the total weight, nos will be equally divided over 50 sub-transactions.
5. If QR code stickers have not yet been printed and if user modifies weight/nos/boxes fields, System will delete and recreate sub-transactions once again. However, if any transaction is already used in Production or Sales user may not modify/delete any transaction.
6. When a given box is scanned during Issue to Production/Invoice, System will update the status of the sub-transaction from Available to Utilized or Partially Utilized.
7. An Excel report of sub-transaction details against each purchase bill will be available in the System.

#### Changes in DPR Stock
1. Existing Stock logic will not be disturbed and users will be able to continue to create/modify stocks. For Manual entries, System will not create sub-transaction nos based on the no. of boxes.
2. A feature for Importing transaction-wise data through Excel will be provided and all existing UI logic will be handled during Import from Excel.
3. System will create stickers with QR code and specified text info in PDF format after stock is saved.
4. An additional table will be provided to store sub-transactions (Trn No + 3 digit box info). For e.g. if there are 50 boxes of a given item, the total weight, nos will be equally divided over 50 sub-transactions.
5. If QR code stickers have not yet been printed and if user modifies weight/nos/boxes fields, System will delete and recreate sub-transactions once again. However, if any transaction is already used in Production or Sales user may not modify/delete any transaction.
6. When a given box is scanned during Issue to Production/Invoice, System will update the status of the sub-transaction from Available to Utilized or Partially Utilized.
7. An Excel report of sub-transaction details against each Stock will be available in the System.
8. There will be no distinction between Good/Rejected stocks while creating/updating sub-transactions.

#### Changes in DPR Production Receipt
1. Existing Production Receipt logic will not be disturbed and users will be able to continue to create Production Receipt. For Manual entries, System will not create sub-transaction nos based on the no. of boxes. Manual entry of production will be disallowed in case the given transaction has been created along with subno and stickers were printed out of the System.
2. System will facilitate stickers with QR code and specified text info in PDF format based upon Production transaction no and no of boxes. These stickers do not represent live transactions in the System. Actual transactions will be generated in the System when users specify RM issues and match them against dummy production transaction no's.
3. An additional table will be provided to store sub-transactions (Trn No + 3 digit box info). For e.g. if there are 50 boxes of a given item, the total weight, nos will be equally divided over 50 sub-transactions.
4. When a given box is scanned during Issue to Production/Invoice, System will update the status of the sub-transaction from Available to Utilized or Partially Utilized.
5. An Excel report of sub-transaction details against each Production Receipt will be available in the System.
6. There will be no distinction between Good/Rejected Production Receipt while creating sub-transactions.

#### Changes in DPR Production Issue
1. Existing Production Issue logic will not be disturbed and users will be able to continue to create Production Issue, without scanner input. However, if the given transaction has subno and stickers have already been printed out of the System, Manual entry will not be allowed.

<!-- 2. Following options will be provided in Scan Production Issue.

    2.1. 10 text boxes will be provided to capture the scanner output.

    2.2. Once 10 text boxes are filled user will be able to navigate to another page of 10 text boxes and so on.

    2.3. Cancel the scan opertion - User will be able to abandon the scan operation, if required.
    
    2.4. Show Summary - System will show a transaction-wise and itemstate-wise summary by consolidating scanner input.<br>
        
    - User will be able to navigate to list of individual scans by clicking a given transaction no. 
        
        - Option to modify weight/nos of an individual scan will be available. Weight/Nos can be reduced but may not be increased.
            
        - If weight is not specified by user, System will compute based on AirGap master.

        - Option to delete individual scan will also be available. 

        - Once view/modify/delete of individual scan(s) is done, user can return to the transaction-wise summary.
        
    - In case a new scan needs to be added, user can click on Continue Scanning.

    - If Rework is set to Yes, only rejected materials can be issued, while if it is set to No, only good materials can be issued. 

    2.5. Once transaction-wise summary is checked and confirmed, user can click on the Create Production Issue button on the summary page. -->

2. When Production Issue entry is created through scanner input, System will update the status of sub-transactions which were created during Purchase Bill/Stock/Production Receipt.
3. Production Receipt entry must be created in the System first and stickers must be printed through System. System will show list of transaction no for which stickers have already been generated. Against this receipt transaction user will import scanned codes from an Excel file for RM to be consumed. When entry is saved in the System, sub-transactions of Production and Bill/Stock will get updated.

#### Changes in DPR Invoice Issue
1. Existing Invoice logic will not be disturbed and users will be able to continue to create Invoice. Sub-transaction no will not be generated for manual entry.

2. Following options will be provided in Scan Invoice.

    <!-- 2.1. 10 text boxes will be provided to capture the scanner output. -->

    <!-- 2.2. Once 10 text boxes are filled user will be able to navigate to another page of 10 text boxes and so on. -->

    2.1. User will first create the invoice document portion in the System. 

    2.2. An option to upload the scanner output through an Excel/CSV file will be provided. System will read and import transaction/sub-transaction no from the imported file.

    <!-- 2.3. Cancel the scan opertion - User will be able to abandon the scan operation, if required. -->
    
    2.3. Show Summary - System will show a transaction-wise and itemstate-wise summary by consolidating scanner input. <br>
        
    <!-- - User will be able to navigate to list of individual scans by clicking a given transaction no. <br> -->
    - User will be able to navigate to list of transactions subno by clicking a given transaction no. <br>
            
        - Option to modify weight/nos of an individual scan will be available. Weight/Nos can be reduced but may not be increased. 
            
        <!-- - If weight is not specified by user, System will compute based on AirGap master. -->
            
        - Option to delete individual scan will also be available. 

        - In case same box is scanned more than once and the data was input through Excel, System will detect and remove such transaction sub no automatic.
            
        - Once view/modify/delete of individual scan(s) is done, user can return to the transaction-wise summary.
        
    <!-- - In case a new scan needs to be added, user can click on Continue Scanning. -->

    - If the scanned transaction contains Scrap material, Invoice creation will be disabled.

    - If the scanned transaction contains any Production entry which is not yet closed, System will disable the option to save the Invoice. 

    2.4. Once transaction-wise summary is checked and confirmed, user can click on the Create Invoice button on the summary page.

3. When Invoice entry is created through scanner input, System will update the status of sub-transactions which were created during Purchase Bill/Stock/Production Receipt.

#### Validation for Manual Transaction Entry
1. In case of Issue to Production/Invoicing, System will not allow Manual entries in case such transactions contain sub-transaction nos and stickers have been printed through the System. In other words, you can operate the DPR System either with System generated stickers or without them. Over a period of couple of months you can gradually introduce stickers of Stock/Bill/Production Receipts.
2. System will provide a date upto which books or closed. If any users attempts to view any Bill/Production/Invoice and Stock entry prior to the book closure date, System will disallow the operation. Further, if any report is requested for a period prior to the book closure date, System will prevent the operation. Only for the Admin user will be able to modify the book closure date in the System.