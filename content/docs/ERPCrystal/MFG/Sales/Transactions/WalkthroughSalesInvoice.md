---

title: "Walkthrough - Sales Invoice"

date: 2023-09-01

draft: false

author: "ERP Crew"

description: ""

pinned: false

hideToc: false

enableToc: true

enableTocContent: false

weight : 1

---
##### Steps to create Sales Invoice
1. Click on Menu --> Sales Module --> Sales Invoice -->**New**
![1](/SalesInvoice/WT_01_SI.png)<br>

2. Fill in **Invoice Sub-Type** as per your requirements
Ensure the Vendor/Currency is same as that of Order for which you have to create Invoice 
Make sure that the firts two digits of GSTIN No. for this party matches with the statecode of the selected state  
Fill in the other details as necessary and click [Save]
![2](/SalesInvoice/WT_02_SI.png)<br>

3. Search the Order No. for which you have created sales Invoice and click[Select]
![3](/SalesInvoice/WT_03_SI.png)<br>

System will redirect to Invoice Line Page.Ensure that you have updated the stocks in Opening/closing Inventory for the same Item/Item State/Stage
![4](/SalesInvoice/WT_04_SI.png)<br>

4. To Print the invoice click  [**Print/Email**] <br> Ensure that header/footer files in png format are uploaded for appropriate unit through **Menu --> System Tools --> Upload Header/Footer.**
5. To [Email] the invoice, ensure that a record for the same party/branch is created in the Contact Master.
6. Click [Make SDN/SCN] to create Debit/credit Notes.Fill in the details and click [Save]
![5](/SalesInvoice/WT_05_SI.png)<br>

{{< callout type="info" >}} For more details on [Sales Invoice] please refer to <a href="https://docs.erpcrystal.in/en/docs/erpcrystal/mfg/sales/transactions/salesinvoice/">**Sales Invoice** {{< /callout >}}