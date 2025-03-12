---
title: "Walkthrough - Purchase Indent"
date: 2023-08-26
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
---

#### Steps to create a Purchase Indent
1. Click on Menu  -->  Supply Chain Module  -->  Purchase Indent  -->  **New**
![1](/PurchaseIndent/WT_PI_01.png)<br>

2. **Send To** -  if you want to send material to job worker. 
Fill in other details as necessary and click [Save].
![1](/PurchaseIndent/WT_PI_02.png) <br> 

3. System will redirect you to the item creation page
![1](/PurchaseIndent/WT_PI_03.png) <br>

4. In case [**Get ReqdBy From Lead Time Master**] parameter is On in **Menu --> System Tools --> [System parameters]**, then ensure that vendor/branch/item/mode of the indent is matched with those of the Leadtime Master. 
If the above parameter is Off, lead time will be fetched from Item Master.
{{< callout type="info" >}} For more details please refer to [**Purchase Indent**](https://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/purchaseindent/#indent-item-create---manadatory-fields) page. {{< /callout >}}
![1](/PurchaseIndent/WT_PI_04.png) 
Also ensure that the rate for this item/party/brand/currency is available in Price Cost Master.
If not, please create a new record in Price Cost Master or pass as **Yes** in [Allow manual rate].
{{< callout type="info" >}} Allow manual rate is possible only for items with [Allow Non Standard Rate] as **Yes** in their Item Group. {{< /callout >}}
![1](/PurchaseIndent/WT_PI_05.png) <br>

5. In order to print or email the indent click  [**Print/Email**] <br> Ensure that header/footer files in png format are uploaded for appropriate unit through **Menu --> System Tools --> Upload Header/Footer.**
![1](/PurchaseIndent/WT_PI_06.png) <br> **Print Indent** - Prints a copy of indent with cost <br> **Print Store Copy** - Prints a copy of indent without cost
![1](/PurchaseIndent/WT_PI_07.png)<br>

6. In order to Email the indent, ensure that a record for the same party/branch is created in the Contact Master.
![1](/PurchaseIndent/WT_PI_08.png)<br>

7. To authorize indent, click [**Authorize Indent**] link in the details page. 
![1](/PurchaseIndent/WT_PI_09.png)

[ How to create a GRN ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/walkthroughgrn/)

{{< callout type="info" >}} For more details please refer to <a href="https://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/purchaseindent/">**Purchase Indent** {{< /callout >}}