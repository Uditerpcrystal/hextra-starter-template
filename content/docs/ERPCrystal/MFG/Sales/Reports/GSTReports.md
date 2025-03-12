---
title: "GST Reports"
date: 2022-01-15
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 4
# tags: 
# - ERPCore 
# - SalesModule
# - GSTReports

---
## Introduction

Generates GST Reports in specified format.

#### Options

|Options|   
  |:------|
  | Select Report <br> - GSTR-1, GSTR-2, GST-ITC-4 etc.
  | Select Unit <br> - Select GST Units
  | Select From Month
  | Select To Month <br> `Validations` <br> - If To Month is selected prior to From Month then this Validation will show "Invalid Date Range". <br> - If To Date is selected later to Current Date then this Validation will show "Future Months are not allowed".
  | Select Date Type <br> - Document Date, Reference Date <br> - Pre-Selected Document Date.


#### Reports available under GST Reports are listed below

|Reports|   
  |:------|
  | 1. GSTR-1 <br> - 1.1. B2B : Business to Business report shows details of no. of recipients, no of invoices, total invoice value, total taxable value for various parties. <br> - 1.2. B2C Large : Business to Customer large report shows details of no. of recipients, total invoice value and total taxable value. <br> - 1.3. B2C Small : Business to Customer small report displays details of total taxable value only. <br> -  1.4. CDNR : Credit / Debit Notes for registered suppliers report shows the details of no. of recipients, no of invoices, no. of notes / vouchers, total note / refund voucher value and total taxable value. <br> - 1.5. CDNUR : Credit /Debit Notes for unregistered suppliers report shows the details of no of invoices, no. of notes / vouchers, total note / refund voucher value and total taxable value. <br> - 1.6. EXP : This report displays the summary for export by showing no of invoices, total invoice value and total taxable value. <br> - 1.7. AT  : This report shows the summary for Advance Received by total advance received and gross advance received. <br> - 1.8. ATADJ : This report shows the summary for advance adjusted by total advance adjusted and gross advance adjusted. <br> - 1.9. EXEMP : This report shows the summary for  nil rated, exempted and non GST outward supplies. <br> - 2.0. HSN : This report displays the summary for HSN by showing total value, total integrated tax, total state / UT tax, total Cess etc. <br> - 2.1. DOCS : This report generates the summary of documents issued during the tax period for total number and total cancelled documeents.<br> - 2.2. HSN - DNCN : This report generate DNCN summary with HSN and different GST rate.
  | 2. GSTR-2  <br> - 2.1. B2B : Business to Business report shows details of monthly tax return for the purchases of registered suppliers. <br> - 2.2. B2BUR : Business to Business report shows details of monthly tax return for the purchases of unregistered suppliers. <br> - 2.3. IMPS : Immediate Payment Service report shows details like invoice number of reg recipient, integrated tax, eligibility for ITC, availed cess etc. <br> - 2.4. IMPG : Import of Goods report shows the details like BE value, rate, taxable value, availed integrated tax etc. <br> - 2.5. CDNR : Credit / Debit Notes for registered suppliers report shows the details like GSTIN of supplier, reason for issuing document, note value, availed integrated tax etc for registered suppliers. <br> - 2.6. CDNUR : Credit / Debit Notes for unregistered suppliers report shows the details like GSTIN of supplier, reason for issuing document, note value, availed integrated tax etc for unregistered suppliers. <br> - 2.7. AT : This report shows summary for tax liability on advance paid under reverse charge(10 A). <br> - 2.8. ATADJ : This report shows summary for adjustment of advance paid earlier for reverse charge supplies. <br> - 2.9. EXEMP : This report shows summary for composition, nil rated, exempted and Non GST inward supplies. <br> - 3.0. ITCR :  Input Tax credit Reversal / Reclaim report shows description for reversal of ITC, to be added or reduced from output liability, ITC integrated tax amount etc. <br> - 3.1. HSNSUM : This report displays the summary for HSN with description, total qty, total taxable value, integrated tax etc.
  | 3. GSTR-3B <br> - This report generates a consolidated summary return of inward and outward supplies.
  | 4. GST-ITC-4 <br> -  4.1. MFG-to-JW :  Manufacturer to Jobworker report shows details like GSTIN of job worker, challan number, description of goods, job work name etc. <br> - 4.2. JW-to-MFG :  Job Worker to Manufacturer report generates details like nature of transaction, original challan number, challan date issued by job worker etc.



