---
title: "Contact"
date: 2022-03-29
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 5
# tags: 
# - ERPCore 
# - SystemToolModule
# - Contact   

---

## Introduction

Maintain contact details of various parties/prospects.

#### Mandatory Fields

<!-- |Mandatory Fields|  
  |:------| 
  | Contact Category <br> - Party, Prospect
  | Contact Name / Branch <br> - Select from Party Master
  | Title <br> - MR, MRS, MS, DR
  | Last Name
  | First Name
  | Type of Contact <br> - Multiple, C Forms, Indents, Orders etc. -->

  |Mandatory Fields|  
  |:------| 
  | Contact Category <br> - If new party contact button is clicked then a party contact will be created else prospect contact will be created.
  | Contact Name / Branch <br> - Select from Party Master/Prospect Master
  | Title <br> - MR, MRS, MS, DR
  | Last Name
  | First Name
  | Type of Contact <br> - Multiple, C Forms, Indents, Orders etc. <br> `Validation` - For this Party/Branch type of contact already exists.
  | Form `Validation` <br> - Either Telephone 1, Cell No 1 or Email1 needs to be filled.
  

#### Optional Fields

|Optional Fields| 
  |:------|
  | Designation
  | Telephone 1 <br> `Validation` - Telephone No. may be upto 14 digits.
  | Telephone 2 <br> `Validation` - Telephone No. may be upto 14 digits.
  | Cell No 1 <br> `Validation` - Please enter a valid number with 10 digits.
  | Cell No 2 <br> `Validation` - Please enter a valid number with 10 digits.
  | Email1 <br> `Validation` - Please enter a valid E-mail address.
  | Email2 <br> `Validation` - Please enter a valid E-mail address.
  | Email3 <br> `Validation` - Please enter a valid E-mail address.
  | Email4 <br> `Validation`- Please enter a valid E-mail address.

####  Features

<!-- |Features|   
  |:------|
  | Create New 
  | Modify  
  | Delete  
  | Export To Excel   -->

  |Features|   
  |:------|
  | Create New Party Contact <br>`Validation` - Type of Contact should be either multiple or any other types Indents/Orders etc.
  | Create New Prospect Contact <br>`Validation` - Type of Contact should be either multiple or any other types Indents/Orders etc.
  | Modify  
  | Delete  
  | Export To Excel  
  | Bulk Import <br>- To import multiple contacts at once. <br>- Bulk Import can be used only when there is no data in the Contact Master Table.<br>`Validation` -Uploaded CSV file name should be ImportContactMst.