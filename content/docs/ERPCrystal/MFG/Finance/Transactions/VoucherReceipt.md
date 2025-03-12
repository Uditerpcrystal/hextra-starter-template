---
title: "Voucher / Receipt"
date: 2022-02-23
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 1
# tags: 
# - ERPCore 
# - Finance
# - Voucher/Receipt

---

## Introduction

It helps to manage Cash/Bank  Vouchers/receipts of customers, vendors, income and expenditure.
<!-- It helps to manage Cash / bank Vouchers / receipts of customers, vendors, income and expenditure. -->

#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Year <br> - Pre-Selected current fiscal year
  | Division <br> - Pre Selected as NA (Options as per Division Master).
  | Voucher Date <br> - Pre Selected as current date. <br> `Validation` - Date must be between Financial Start Date and End Date. 
  | Bank / Cash Name <br> - Pre Selected (Options as per Chart Accounts Master where Account Type is in Bank/Cash).
  | Payment Mode <br> - Pre Selected as Not Applicable(Not Applicable, RTGS, NEFT, Manual Cheque, Print Cheque through System) <br> Print Cheque through System - To print cheque using cheque master available cheques.
  | Is Post Dated <br> - Pre Selected as No (Yes, No) <br> Select Yes For creating Future Date Voucher and you can change Voucher date as per your requirement using modify button.
  | Currency <br> - Pre Selected as INR (Options as per Currency Master) 
  | FCNR Amount <br> `Validations` <br> - FCNR amount may not be zero for non INR. <br> - FCNR Amount must be zero for INR currency.
  | Cheque No (Only for bank) <br> `Validation` <br> - This cheque is not available in cheque master for this Bank / Division <br> - This cheque is already issued. You can not print this cheque.
  | Cheque Date (Only for Bank) - Pre Selected as current date. <br> `Validation`  - If cheque date selected prior of 3 months from Voucher date or 6 months later to voucher date then System will show correct date range for Cheque date.
  | Document Type <br> Pre Selected as GL (GL, OA, AD, NA) / Receipts related to business transactions like Accounting Charges, Interest  Received etc. <br> OA - Receipts from customers. <br> AD - Advance Payments / Receipts from customers or to Vendors. <br> NA - For add multiple Sale Invoice or Purchase Bills Payments/Receipts using ref no.
  | A/c Codes <br> - Select from Chart Of Accounts Master only for Document type GL.
  | Select Party <br> -  Select from Party Master, Mandatory to select when Document type is not GL.
  | Debit / Credit <br> - Pre Selected as Debit (Debit, Credit)
  | Amount <br> `Validations` <br>  - Amount must be between 0.01 - 999999999.99 <br> - **Insufficient balance in selected Bank / Cash**  If Document type is GL or AD and its Debit transaction and Allow negative for selected Bank is N in Charts of Account then this Validation will show.   
  | Form `Validation` -  **System Vouchers are being DONE, User cannot Create Voucher.** In System Parameter, if Sys Condition for [Is Voucher Import From XL] is off then this Validation will show.

#### Optional Fields

|Optional Fields| 
  |:------|
  | Is TDS applicable for this A/c.?
  | Ref No <br> - Only for OA Document type.<br>`Validations` <br> - Mandatory to fill when Document type is SI or PB. <br> - **Ref No and / or Ref date can not be located.**  Filled Ref no. must be available in Selected Document type on selected Ref Date for selected Party other wise System will show this Validation .
  | Ref Date <br> - Only for OA Document type.
  | Drawn On
  | UTR No  
  | Notes <br> Mandatory to fill for GL Document type.
  <!-- | Trn No   -->


#### Features

|Features|   
  |:------|
  | Create New
  | Modify <br> - If System lock is applied to the document, this option will be disabled. <br> If Voucher is Post Dated then It will redirect to you on PDC modify Page where you can Modify Voucher Date.
  | Delete <br> - If System lock is applied to the document, this option will be disabled. <br> `Validation` - Notes need to be filled, it should be relevant / relevant for audit trial.
  | ***Print / Email** <br> Select Bank Name <br> - Select from Bank Master <br> Voucher No. From <br> To. <br>  `Validations` <br> - Selected vouchers may not belong to this particular bank. <br> - Email may be sent only when Refdoc is PB or AD. <br> - At a time only 100 vouchers can be printed <br> - Starting/Ending Voucher No has to be same, for Email <br> - Email may be sent only when it is payment voucher
  | Modify More Info <br> - To update currency and FCNR amount. <br> - FCNR amount may not be zero for non INR. <br> - FCNR Amount must be zero for INR currency
  | Upload Document <br> - For Uploading supported Document. <br> - Only PDF format is allow.
  | Cheque Status <br> - To authorize cheque for printing.
  | **Print Cheque**  <br> - To print cheque for given cheque types.<br> Mandatory Fields <br> Cheque No - Select from Cheque Master. <br> Payee - Needs to fill only for GL Document type. <br> Cheque Type - A/c Payee Only, Bearer,  RTGS Cheques  <br> `Validations` <br> -  **This Cheque is not available in cheque master for this Bank / Division** If Selected Cheque no. is not available in cheque master for selected Bank, Division. then System will show this Validation. <br> - **This Cheque is already issued. You can not print this cheque.** If Cheque no. status is in issued in cheque master or already used for another voucher the System will show this Validation . <br> - **Only Payment voucher can be printed.** If Voucher Type is not Paid then System will show this Validation .
  | Process Cheque Return <br> - To return the cheque.
  | Cancel / Stop Cheque <br> - To cancel the cheque.
  | Voucher Details <br> - To show voucher details index.
  | Duplicate Voucher <br> - Helps to Duplicate entire voucher at once click. <br> - Only will show when Document type is GL for all lines in Voucher. <br> `Validation` -**Duplicate Voucher could not succeed as there is insufficient balance**. If document type is paid and allow negative for selected Bank is N in Charts of Accounts then System will show this Validation. <br> - You may not duplicate PDC (Post Dated Cheque) voucher. <br> - When import is in progress you may not duplicate voucher. <br> - **Duplication failed as voucher amount is zero.** <br> - You can duplicate voucher only if it is of current year.
  | **Import Voucher**  <br> Select Doc Type <br> -Ar/Ap, GL <br> Select File <br> `Validations` <br>  - Uploaded CSV file name should be ImportVoucher <br> - Import csv file to get voucher report.

#### Voucher Line - Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Document Type <br> - GL, OA, AD, SI etc. 
  | A/c Codes <br> -  Select from Chart Of Accounts Master
  | Select Party <br> - Select from Party Master <br> `Validation` <br> - **You may not add different party accounts in a single payment voucher**. In single voucher if you are trying to add 2 different parties or more then for Document type PB or AD then System will show this Validation.
  | Ref No
  | Ref Date 
  | Debit / Credit  <br> - Debit, Credit
  | Amount <br> `Validation` <br> - Amount must be between 0.01 - 999999999.99 <br> - **Insufficient balance in selected Bank / Cash**. If Document type is not OA and its Debit transaction and Allow negative for selected Bank is N in Charts of Account then System will show this Validation.   
  | Ref Date From
  | Ref Date To <br> `Validation` - Ref Date To must be greater than ref Date From 
  | Form `Validation` - **System Vouchers are being DONE, User cannot Create Voucher.**. In System Parameter if Sys Condition for [Is Voucher Import From XL] is off then System will show Validation.


#### Voucher Line - Optional Fields

|Optional Fields| 
  |:------|
  | Notes
 #### Voucher Line - Features

|Features|   
  |:------|
  | Create New 
  | Add Multiple <br> - Only will show at line level creation when document type is SI or PB. <br> - Will show list of Document of Payments/Receipts for Selected Party on selected Ref Date Range. <br> - Using this list data for add multiple just you need to fill amount System will automatically create lines. <br>`Validations` <br> - For selected Document, Receipt/Payment amount can not be greater then System Due Amount or Bill amount. <br> - **Insufficient balance in selected Bank / Cash**. If Allow negative for selected Bank is N in Charts of Account then System will show this Validation .<br> - **System Vouchers are being DONE, User cannot Create Voucher.**
  | Modify 
  | Delete   
  | Modify Reference No. and Reference Date <br> - Only for AD Document type.<br> To modify reference no. & reference date.<br>`Validations`<br> - **Document No/Date may not belong to this Party.**.  Filled Ref no. must be available in Selected Document type on selected Ref Date for selected Party other wise System will show Validation  <br> - **The Bill amount does not match the original amount in this voucher** If Voucher amount is not same as Bill amount the this Validation will show.