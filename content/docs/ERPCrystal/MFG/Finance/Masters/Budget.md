---
title: "Budget"
date: 2022-03-01
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 9
# tags: 
# - ERPCore 
# - Finance
# - Budget

---

## Introduction

Maintains budget of income and expenses.

#### Mandatory Fields

|Mandatory Fields|  
  |:------|
  | Year <br> - Select from Year combo list.
  | Select Budget Year-Month <br> `Validation`<br> - **This record already exist**. If budget records for this year - month, A/c Codes are already exists.
  | Select A/c Codes <br> - Select from Chart Of Accounts Master
  | Select Cost Center <br> - Select from Cost Center 
  | Amount <br> `Validation` - Amount must be between 0.01 - 99999999.99 
  | Debit / Credit <br> - Debit, Credit  
  | MainAc 

#### Features

|Features|   
  |:------|
  | Create New
  | Delete     
  | **Import From Excel** <br> - To import data and download budget report <br> Select File <br> `Validation` <br> - Uploaded CSV file name should be Budget  <br> - Budget records for this year - month are already available 
  | Download Model
