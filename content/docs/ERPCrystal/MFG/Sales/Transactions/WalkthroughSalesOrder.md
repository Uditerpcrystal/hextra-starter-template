---

title: "Walkthrough - Sales Order"

date: 2023-08-25

draft: false

author: "ERP Crew"

description: ""

pinned: false

hideToc: false

enableToc: true

enableTocContent: false

weight : 1

---

##### Steps to create Sales Order 
1. Click on Menu --> Sales Module --> Sales Order -->**New**
![1](/SalesOrder/WT_01_SO.png)<br>

2. Select **Order type** Proforma Invoice,Quotation or Direct as per your requirements 
Fill in the other details as necessary and click [Save]
![2](/SalesOrder/WT_02_SO.png)<br>

If you will select **Change Payment Terms for this Order**  Yes then system will redirect you to a new page
![3](/SalesOrder/WT_08_SO.png)<br>

Fill in the details and click [Save]. System will redirect you to details page
![3](/SalesOrder/WT_09_SO.png)<br>


3. Click [New] to create Sales Order Line. 
![3](/SalesOrder/WT_10_SO.png)<br>
4. Fill in the  details as necessary and click [Save]
![3](/SalesOrder/WT_03_SO.png)<br>
5. Ensure that rate exist in the Price/Cost master for the same Item/Brand/Currency
If not, please create a new record in Price Cost Master or pass as Yes in [Allow manual rate].
{{< callout type="info" >}} Allow manual rate is possible only for items with [Allow Non Standard Rate] as **Yes** in their Item Group. {{< /callout >}}
![4](/SalesOrder/WT_04_SO.png)<br>

6. To print the sales order click [Print] Ensure that header/footer files in png format are uploaded through System Tools -->Upload Header/Footer
7. To [Email] the Sales Order ensure that a record for the same party/branch is created in the Contact Master.
![5](/SalesOrder/WT_07_SO.png)<br>

8. To create an Invoice for the sales Order click [Make Invoice]<br> Ensure that the following points are satisfied while creating Invoice<br>- Status of all lines in this Order must be OK. <br>- Invoice can be made only if the order type is confirmed order.<br>- If one or more lines in an order is already invoiced, then Make Invoice cannot be used.<br>-  Ensure that **allow invoice** is ‘Yes’ in Party Master for that party<br>- Currency must be only INR
<!-- {{< callout type="info" >}} For more details on [Sales Order] please refer to [**Sales Order**](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/sales/transactions/salesorder/) page. {{< /callout >}} -->

{{< callout type="info" >}} For more details on [Sales Order] please refer to <a href="http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/sales/transactions/salesorder/">**Sales Order** {{< /callout >}}

9. To update Ship to info, click **GST Info,Ship to details --> Create/Modify Ship to info** as shown below
![6](/SalesOrder/WT_05_SO.png)<br>

System will redirect you to a new page. Fill in the details and click [Save]
![7](/SalesOrder/WT_06_S0.png)

[ How to create a Sales Invoice ? ](http://docs.erpcrystal.in/en/docs/erpcrystal/mfg/sales/transactions/walkthroughsalesinvoice/)
 