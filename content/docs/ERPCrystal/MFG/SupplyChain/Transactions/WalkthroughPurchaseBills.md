---
title: "Walkthrough - Purchase Bills"
date: 2023-09-04
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
---

#### Steps to create a Purchase Bill
1. Click on Menu  -->  Supply Chain Module  -->  Purchase Bill  -->  **New**
![1](/PurchaseBills/WT_PB_01.png) <br>

2. System will redirect you to the Purchase Bill creation page
![1](/PurchaseBills/WT_PB_02.png) <br>
Account particulars lets you to define whether any TDS or TCS, Service Tax etc is applicable,.
![1](/PurchaseBills/WT_PB_12.png) <br>

3. Ensure that the first 2 digits of GSTIN No of this party matches with the code of the selected state.
{{< callout type="info" >}} For GSTIN No check Party Master and for state code check State Master {{< /callout >}} If E-Invoice is set as mandatory in party master then [Is E-Invoice Submitted?] as **Yes** for the selected party.
![1](/PurchaseBills/WT_PB_03.png)
If transaction type is 'Not Applicable' in party master then either go to party master to change the transaction type or change it from here.
Fill in other details as necessary and click [Save].
![1](/PurchaseBills/WT_PB_04.png) <br>

4. System will redirect you to the Purchase Bill Line index page
![1](/PurchaseBills/WT_PB_05.png) <br>

5. In the invoice, if freight carrier charges are filled in, then we can refer to it by using [Link to carrier charges (No GRN)] while creating bill. This helps to avoid duplicate payment of freight charges.
![1](/PurchaseBills/WT_PB_06.png) <br>

6. If you want to create a purchase bill line referring to a GRN then search the GRN No and then click [Select]
Fill in the necessary details and Click [Save].
![1](/PurchaseBills/WT_PB_07.png) <br>

7. Otherwise, if you want to create a purchase bill line without referring to a GRN then click [Add Line without GRN Reference] (Usually used for services).
Fill in the necessary details and Click [Save].
![1](/PurchaseBills/WT_PB_11.png) <br>
GST Code defines how much GST % is applied for that item
![1](/PurchaseBills/WT_PB_13.png) <br>

8. If you want to modify some details in the bill after bill payment is done, you can click [Modify Other Info] 
![1](/PurchaseBills/WT_PB_08.png) <br>

9. In order to create multiple line records without referring to GRN you can click [Import Non GRN]
![1](/PurchaseBills/WT_PB_09.png) It will redirect you to Import No Ref GRN page. 
Download the model and fill in the records in it. 
Click [Upload].
![1](/PurchaseBills/WT_PB_10.png) <br>

{{< callout type="info" >}} For more details please refer to <a href="https://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/purchasebill/">**Purchase Bills** {{< /callout >}}