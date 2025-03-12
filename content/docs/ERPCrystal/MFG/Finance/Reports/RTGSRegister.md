---
title: "RTGS Register"
date: 2022-03-11
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 2
# tags: 
# - ERPCore 
# - FinanceModule
# - RTGSRegister

---
## Introduction

This feature helps to generate report of RTGS / NEFT payments.


#### Options

|Options|   
  |:------|
  | Year <br> - Pre Selected as current fiscal year
  | Division <br> - Pre Selected Na (Options as per Division master).
  | Select Report Type <br> - Pre Selected as RTGS/NEFT Register (RTGS / NEFT Register, Counter Foil, Receipt Register (TCS))
  | Select Date Range <br> - Only applicable for Receipt Register (TCS) report type.
  | Payee Type <br> - Pre Selected as Party (Party, Employee)
  | Bank Name <br> - Select from Bank Master.
  | Lock RTGS / NEFT Voucher <br> - Pre Selected as No (Yes, No)
  | Cheque No.
  | Date Range <br> `Validation` - Gap between date range may not exceed two year.


#### Reports available under RTGS Register are listed below

|Reports|   
  |:------|
  | 1. RTGS / NEFT Register <br> - 1.1. RTGS Register: This report will show all the beneficiary details along with payment details.
  | 2. Counter Foil <br> - It will show the record of transactions.
  | 3. Receipt Register (TCS) <br> - It will display transaction receipts for various parties.