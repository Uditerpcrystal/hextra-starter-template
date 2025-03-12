---
title: "Receivable"
date: 2022-03-12
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 6
# tags: 
# - ERPCore 
# - FinanceModule
# - Receivable

---
## Introduction

Download Receivable Statement along with Summary and Age Analysis.


#### Options

|Options|   
  |:------|
  | Party Group <br> - Pre Selected as All (Options as per Party group master)
  | Party <br> - Pre Selected as All (Options as per Party master) <br> Mandatory to select individual party when report type is Matched Documents etc.
  | Sales Officer <br> - Pre Selected as All (Options as per Sales Officer Master)
  | Account Type <br> - Pre Selected as Customer Control A/C - Outside (Customer Control A/C - Outside, Customer Control A/C -Intercompany, Inter-Branch Control A/C)
  | Scan Documents based on <br> - Pre Selected as Ref date (Ref date, Doc date)
  | Compute Aging based on <br> - Pre Selected as Ref date (Ref date, Doc date)
  | Date Range <br> `Validations` <br> - Invalid Date Range. <br> - Date cannot be after financial year end date.
  | Show Only what is due <br> - Pre Selected as No (Yes, No)
  | Additional Reports <br> - Pre Selected as Summary (Summary, PO Details, Matched Documents etc.)
  | Include Grace Period <br> - Yes / No <br> - Only will show when Sys Parameter will **ON** for **Allow Grace Period.**
  | While computing target, ignore invoices after <br> - If report type selected as  **Collection Target as per Due Date vs Actual** then it will show the actual To Date for Report. <br> - To Date needs to be same as Computing Target Date.


#### Reports available under Receivable are listed below

|Reports|   
  |:------|
  | 1. Summary <br> - 1.1. Receivable : This report will show the detailed summary of account receivables. <br> - 1.2. Summary : It will show the age analysis for all parties with amount. <br> - 1.3. PDC Register :  It will show all the Post Dated Cheques (PDC) records.
  | 2. Collection Target as per Due Date vs Actual <br> - 2.1. Receivable : This report will show the detailed summary of account receivables. <br> - 2.2. Collection Report : It will display detailed data of all collected transactions received within a specific date range. <br> - 2.3. Duedate wise Report : This report will show all the transactions details of various parties along with grand total.
  | 3. Interest on Overdue OS <br> - 3.1. Receivable : This report will show the detailed summary of account receivables. <br> - 3.2. Overdue Report : It will show the overdue details of account payables and receivables. <br>- 3.3. Late Receipt Report : It will show the overdue details with delay in days of account payables and receivables.
  | 4. Partywise Receipts / Payments <br> - 4.1. Receivable : This report will show the detailed summary of account receivables. <br> - 4.2. Receipts Payments : It will show the transaction receipts for all parties.
  | 5. Matched Documents <br> - 5.1. Receivable : It will show the detailed report of receivables for matched documents.
  | 6. PO Details <br> - 6.1. Receivable : This report will show the detailed summary of account receivables. <br> - 6.2. PO Details : This report will show all the PO details.
