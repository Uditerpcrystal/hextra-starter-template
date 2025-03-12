---
title: "Transfer Fund"
date: 2022-02-24
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 3
# tags: 
# - ERPCore 
# - Finance
# - TransferFunds

---

## Introduction

Helps to transfer funds between cash to bank and bank to bank. 


#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Year <br> - Pre-Selected current fiscal year.
  | Date <br> - Pre Selected as current date <br> `Validation` - Date must be between the Financial year's Start Date and the End Date. 
  | Division <br> - Select from Division Master
  | Transfer Out Of <br> - Select from Bank Master
  | Transfer Into <br> - Select from Bank Master
  | Cheque No
  | Cheque Date <br> - Pre Selected as current date
  | Amount <br> `Validation` - Amount can only be between 0.01-9999999999.99
  | Cash Collection Date <br> - Applicable only when CASH ind is available in profitfycfd table.
  | Form `Validations` <br> - **In Chart of Accounts Master, please create an Account Code with A/c Type as F, to activate Transfer of Funds..**.In Chart of Accounts Master, A/c needs to be available with A/c Type as F(Funds Transfer). <br> - **Cash Collection Date needs to be filled**. <br> - **Balance Amount to be transfered must be.**