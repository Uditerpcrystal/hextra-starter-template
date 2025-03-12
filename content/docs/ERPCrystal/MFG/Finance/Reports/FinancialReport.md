---
title: "Financial Register"
date: 2022-03-11
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
# - FinanceModule
# - FinancialRegister

---
## Introduction

Generate BS, P & L, Trial Balance, General and Party ledgers.


#### Options

|Options|   
  |:------|
  | Year <br> - Pre Selected as current fiscal year.
  | Report Type <br> - Pre Selected as Ledger (Ledger, Final Accounts, Confirmation of Balances) <br> `Validation` - **Report aborted as following JVs has discrepancy.** If any JVs has discrepancy then this validation will show.
  | Unit <br> - Pre Selected as All
  | Division <br> - Pre Selected NA (Options as per Division Master)
  | Account Type <br> - Pre Selected as General Ledger (General Ledger, Customer Control, Vendor Control)
  | Type of Grouping <br> - Only for Final Accounts Report Type
  | Select Groups <br> - Pre-Selected as All Groups (Options as per BS/PL master)
  | Select Account Particulars <br> - Pre Selected as All A/C Head (Options as per Account Master )
  | Select Party Group 
  | Select Party 
  | Show Report header 
  | From Date <br> `Validation` - From date can not be before F.Y start.
  | To Date <br> `Valudation` <br> - Invalid Date Range. <br> - End date can not be After F.Y end <br> - **Report can only be downloaded for 1 Year**. If Sys Parmeter  is **ON** for Allow Calendar Year then you can select To date after F.Y. end date also but gap between Start Date & End Date is only 1 year is allow.
  | Exclude MIS JV <br> - Pre Selected as Yes (Yes, No)
  | Show In Dashboard <br> - Pre Selected as No (Yes, No) <br> - It will show Opening & Closing Bal. only of those Accounts Heads which is selected as **Yes for Show in Trial Balance Dashboard** in Charts of Accounts Master. <br> `Validation` - Dashboard can be printed only for Final Accounts >> General Ledger.
  | Exclude System JV For Visual Match-off <br> - Pre Selected as Yes (Yes, No)
  | Form `Validation` <br> - **Link Profit for the year A/c. in Transaction Type Master.** If Trn type Code **P0 i.e., Profit for the year** is not available in Transaction Type Master then this validation will show. 
  
  <!-- | Date Range <br> `Validation` - Invalid date range. -->


#### Reports available under Financial Register are listed below

|Reports|   
  |:------|
  | 1. Ledger <br> - 1.1. Ledger New : This report will show the financial statements of business.
  | 2. Final Accounts <br> - 2.1. Trial_Balance : It will display all the ledger balances categorized into debit and credit. <br> - 2.2. P & L Statement : This report will show company's revenues and expenses for running the business. <br> - 2.3. Balance Sheet : It will show the statement / summary of a business's assets.
  | 3. Confirmation of Balances : This will display a letter to confirm the balance as per the books or records.
