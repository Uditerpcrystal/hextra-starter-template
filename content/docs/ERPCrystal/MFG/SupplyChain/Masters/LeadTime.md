---
title: "Lead Time"
date: 2022-01-20
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
# - SupplyChainModule
# - LeadTime

---

## Introduction 

This feature helps to maintain lead time of procurement of materials by vendor, mode of transport.

#### Manadatory Fields

|Mandatory Fields|  
  |:------|
  | Customer / Supplier / Branch <br> - Pre selected (Options as per Party Master) <br> `Validation` - A record with this party / branch / item already exists.
  | Item <br> - Pre selected (Options as per Inventory Master)Select from Inventory Master
  | Lead Time <br> `Validation` <br> - Lead time must be between 1 - 365 
  | LT No

#### Optional Field

|Optional Fields|  
  |:------|
  | Notes

#### Features

|Features| 
  |:------|
  | Create New 
  | Modify
  | Delete
  | Export To Excel <br> - To download lead time report.
  | Update Lead Time <br> `Validation` <br> - Upload Csv file to update lead time with file name as UpdateLeadTime
  | Update Transit Days <br> `Validation`  <br>- Upload Csv file to update transit time with file name as UpdateTransitDays 

#### Create New Line - Manadatory Fields

|Mandatory Fields|  
  |:------|
  | No <br> - Auto fetched from main document.
  | Mode <br> - Pre selected as Air (Air, Road, Rail etc.) <br> `Validation` <br> - A record with this Mode already exists.
  | Transit Days <br> `Validation` <br> - Transit days must be between 0 - 365
  | Is This Default? <br> - Pre selected as Yes (Yes / No)

#### Create New Line - Features

|Features| 
  |:------|
  | Create New 
  | Modify
  | Delete
