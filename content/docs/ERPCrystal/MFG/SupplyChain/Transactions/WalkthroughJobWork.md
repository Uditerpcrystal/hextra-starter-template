---
title: "Walkthrough - Job Work"
date: 2023-09-12
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
---

#### Steps to create a Job Work
1. Click on Menu  -->  Supply Chain Module  -->  Job Work  -->  **New**
![1](/JobWork/WT_JW_01.png) <br>

2. System will redirect you to the job work creation page.
![1](/JobWork/WT_JW_02.png) <br>

3. Ensure that the first 2 digits of GSTIN No of this party matches with the code of the selected state.
{{< callout type="info" >}} For GSTIN No check Party Master and for state code check State Master {{< /callout >}} 
Fill in other details as necessary and click [Save].
![1] (/JobWork/WT_JW_03.png) <br>

4. System will redirect you to job work details page.
We can create line level details either by clicking [Import From Bill] or [In-Stock through GRN] or [New]
![1] (/JobWork/WT_JW_04.png) <br>

5. Import from Bill is used to enter the details of the out stocked quantity. When the bill is created and the material has to be sent from vendor to the job worker directly, then import from bill is used. <br> After clicking [Import From Bill] you have to search for the bill no of the same party and click import.
![1](/JobWork/WT_JW_05.png) <br> When importing from bill it will check whether stock is available in the inventory or not. If not then it will redirect you to Job work negative stock page and it will not allow you to import.
![1](/JobWork/WT_JW_06.png) <br>Otherwise, after clicking [Import] line details will be imported from the referenced bill.

6. In-Stock through GRN is used to enter the details of the in stocked quantity. If for every incoming material a GRN is created and now we want to a create job work for this in stocked material then we can use [In-Stock through GRN] option.<br> In case of [In-Stock through GRN] you have to search for the GRN No and click [Select].
![1](/JobWork/WT_JW_07.png) <br>System will redirect you to the job work line creation page.
Fill in details as necessary and click [Save].
![1](/JobWork/WT_JW_08.png) <br>

7. [New] can be used to  enter details of both out stocked and in stocked quantity. <br>If you click [New] for line creation then system will redirect you to the job work line creation page.
Fill in details as necessary and click [Save].
![1](/JobWork/WT_JW_09.png) <br>

{{< callout type="info" >}} The job challan will be balanced and closed when the **total weight out** becomes equal to the **total weight in** {{< /callout >}} 

8. If you want to print a line then go to the job work item details page and click [Print]
![1](/JobWork/WT_JW_10.png) <br>


{{< callout type="info" >}} For more details please refer to <a href="https://docs.erpcrystal.in/en/docs/erpcrystal/mfg/supplychain/transactions/jobwork/">**Job Work** {{< /callout >}}