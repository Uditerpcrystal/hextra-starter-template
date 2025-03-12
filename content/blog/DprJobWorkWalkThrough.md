---
title: "Walkthrough for Job Work"
date: 2024-11-30
draft: false
author: "ERP Crystal"
description: "A Step-by-Step Guide for Job Work"
pinned: true
hideToc: false
enableToc: true
enableTocContent: false
tags:
- JobWork
---
### Job Work Walkthrough

1. **Accessing Job Work**
   - Navigate to the **DPR** menu and select **Job Work**.
   - The **Job Work** index page will open, displaying a list of existing Job Works. This page offers options such as **Create** for initiating new Job Work entries and **Item Details** to view all items associated with a specific Job Work.
   ![Access Production Plan](/DprJobWork/WT_DprJW_01.png)

2. **Creating a New Job Work**
   - Click on the **Create New** button and enter the necessary details for the Job Work.
   ![Access Production Plan](/DprJobWork/WT_DprJW_02.png)

3. **Creating Job Work Lines**
   - Click on the **Job Work Line Details** option.
   ![Access Production Plan](/DprJobWork/WT_DprJW_03.png)
   - This will redirect you to the Job Work Items Index. Click **Import From Bill** to begin importing the associated details.

4. **Importing from Bill (Sent From Vendor)**
   - The **Import From Bill** functionality offers two types of imports.
   - Select **Sent From Vendor** to import data from a single Bill.
   - Enter the Bill Date and Bill Party as per the provided Bill Number.
   - Specify the Challan Date as required, ensuring that it is later than the Job Work Date.
   - Click **Create From Bill** to complete the import process.
   ![Access Production Plan](/DprJobWork/WT_DprJW_05.png)

5. **Importing from Bill (Sent From Factory)**
   - Select **Sent From Factory** to import from multiple Bills.
   - Scan the QR Codes and upload the populated Excel file.
   - Specify the Challan Date as required, ensuring it is greater than the Job Work Date.
   - Click **Upload** to proceed with the import.
   ![Access Production Plan](/DprJobWork/WT_DprJW_06.png)

6. **Uploading Coil Numbers**
   - Once the records are imported, click on **Update Coil No**.
   ![Access Production Plan](/DprJobWork/WT_DprJW_07.png)
   - Download the provided model, fill in the Coil Numbers, and upload the updated file.
   ![Access Production Plan](/DprJobWork/WT_DprJW_08.png)

7. **Importing into Challan**
   - After updating the Coil Numbers, click **Import In Challan** to proceed.
   ![Access Production Plan](/DprJobWork/WT_DprJW_09.png)
   - Download the model, fill in the quantities, and import the data.
   ![Access Production Plan](/DprJobWork/WT_DprJW_10.png)
   - Ensure that the corresponding plan has been created for the respective Bills in the Production Plan.

8. **Importing Scrap**
   - Once the Challan is created, click **Import Scrap**.
   ![Access Production Plan](/DprJobWork/WT_DprJW_11.png)
   - Download the model, fill in the quantities, and import the data.
   ![Access Production Plan](/DprJobWork/WT_DprJW_12.png)

9. **Creating an Invoice**
   - To create an invoice for the In Challan, click on the record and select **Create Invoice**.
   ![Access Production Plan](/DprJobWork/WT_DprJW_13.png)
   - Confirm the action, and the invoice will be generated.
   ![Access Production Plan](/DprJobWork/WT_DprJW_14.png)