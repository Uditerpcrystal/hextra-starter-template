---
title: "Bill Of Matertials"
date: 2023-01-02
draft: false
author: "ERP Crew"
description: "Guide to uses Bill of Materails."
pinned: true
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- BOM

---

### Introduction
<!-- - A Bill of Materials is used to manage the productivity of the product.
- It contains a list of items which are required to make a product.
- The bill of materials also takes care of the quantities required to create a product.
- Multiple items can be added to one single bill of material. -->
- The Bill of Materials (BOM) is a comprehensive list of all the components and parts needed to manufacture a particular product.
- The system calculates the cost for each input item using two methods: weighted average and loss rate.
- Users can manually set the rate for certain items if needed.

#### Create a new BOM
- BOM can be created in three ways.
    1. Enter the data through User Interface.
    2. Import BOM through Excel.
    3. Duplicate the existing BOM with the duplicate method.

- There are different input types given while creating a BOM.
- The following input types are: 
    1. Raw materials
    2. Packing materials
    3. Labor  charges
    4. Overhead
    5. Sub Assembly

- When the input type is selected as a Sub Assembly then you need to make sure that the BOM already exists in the Sub Assembly item. eg. To manufacture  a car, we neen an engine as a sub assembly.

#### Import BOM through Excel
- To import data, you need to create header data first and then download the Excel template.
- Save the template as a .csv file and upload it to the system.
- Please ensure that all fields in the template are filled in.

#### Create Cost sheet using BOM
- You can enter different input quantities and rates against every input item in order to build a cost sheet.
- Cost sheets quantities and rates will not affect the BOM quantities and rates.

<!-- #### Line level Creation.
- BOM can be created in three ways.
    1. Through the System, you can create one line-level BOM at a time.
    2. Through Excel. You can import multiple items at the same time in the BOM.
    3. Duplicate. Duplicate means a duplicate BOM will be created of the Existing BOM.

- There are different input types given while creating a BOM.
- The types are: 
    1. Raw materials.
    2. Packing materials.
    3. Labour charges.
    4. Overhead.
    5. Sub Assembly.
    6. By product.
- When the input is selected as a Sub Assembly then you need to make sure that the BOM already exist in the table with the same item, party.
- There will be an option that the rate should be manual or not. If the user selects it as 'Yes', they have to enter the rate in the rate input field. -->


<!-- #### Adding BOM items through excel.
- One can add multiple items through an excel sheet.
- While writing the data in the system-generated excel, you need to make sure all the fields are filled.

#### Additional inputs in modify for line level records.
- On the Modify page, there are 3 new inputs, CS flag, CS Qty and CS Rate.
- CS stands for Cost sheet.
- The CS flag by default is selected as System but if you change it to Manual you need to enter the CS qty and CS rate.
- When the CS flag is selected as a system then the CS Qty and CS Rate be zero.
- The cost sheet rates and quantities may differ from the bill of materials (BOM) rates and quantities if the user manually enters them while the cost sheet flag is set to "Manual." -->

#### Reports for BOM.
- After the BOM creation, the user can download the report for the specific BOM or all items.
- There are two types of BOM reports, the normal BOM and the cost sheet.
- The user can add the cost sheet quantity and rate for the BOM, in the BOM items modify.
- If the user has given the cost sheet quantity and rate, then it will be shown in the BOM report.
- While printing the cost sheet report, if the cost sheet rates and quantity are not given still you can print the report but the values will be the same as of BOM.
> Note: BOM report is for internal use and the Cost sheet is for external use.
