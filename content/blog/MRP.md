---
title: "Material Requirement Plan"
date: 2021-04-16
draft: false
author: "ERP Crew"
description: "Guide to download MRP report"
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- MRP report
categories:
- Manufacturing
---

# Introduction

Material requirement planning (MRP) is a production planning, scheduling, and inventory control system used to manage manufacturing processes.
This blog walk you through on the steps for MRP.

## Material Requirement Plan
- On options page you can select unit, year, report type, plan range from, plan range to and there are specific checkbox to select;
1. Add pending order qty to plan qty.
- If there are any pending orders those can be added to the plan qty in the production plan.
2. Adjust FG store stock from pending orders.
- If there are finished goods in stock, those can be reduced from pending orders quantity.
3. Adjust RM store stock in procurement.
- If there are raw material in the stock already those can be adjusted in the procurement plan.
4. Scan BOM of Sub Assemblies to Workout Consumption.
- Bill of material of sub assemblies can be adjusted to compute the consumption in the procurement plan.

### Production Plan Report
- Production plan worksheet is all about production plan details and plan qty.
- In final production plan, calculate final summation of plan qty,pending order qty and fg stock qty.
- Product wise consumption will show how much consumption of the product in the production plan has been done .
- Item wise consumption will show how much consumption of item in the production plan has been done.
- Item wise consumption summary will show summarization of consumption of item has been done.
- IIRS qty will show final consumption of item in the production plan with production process and rack info.

### Procurement Plan Report
- Procurement plan is all about procuremnet plan details of item.
- For procurement plan, purchase indent, pending indent, inventory master, QA stock has to be updated.
- Procuremnet plan consider computed qty,stock qty, pending indent qty,make indent qty of item with re order level qty. 
- Procuremnet based on max order will show max order level of item.

## Steps in MRP
###### To understand MRP, create a model as follows:
  - Create a few items in the **Inventory Master** under various categories as follows:
>**Category : Finished Goods** 
    - FG-01 
    - FG-02
>**Category : Raw Materials**
    - RM-01 
    - RM-02 
    - RM-03 
    - RM-04 
    - RM-05 
>**Category : Finished Goods - Sub Assembly**
    - SA-01 
    - SA-02

![1](/MRP/inventorymasterindex.png)

###### Create BOM records in  **Bill Of Material** Module for Finished Goods and Sub Assembly items, as shown in the following table.

  ![2](/MRP/billofmaterial.png)
  
  ###### BOM OF FG-01:
  |Input item|  Type |  Quantity |
  |:------:|:------:|:------:|
  | RM-01 | RM  | 2 |
  | RM-02 | RM | 4 |

  ###### BOM OF SA-02 :
  |Input item|  Type |  Quantity |
  |:------:|:------:|:------:|
  | RM-05 | RM  | 7 |

  ###### BOM OF SA-01 :
  |Input item|  Type |  Quantity |
  |:------:|:------:|:------:|
  | RM-04 | RM  | 6 |
  |SA-02 | SA  | 6 |
  
  ###### BOM OF FG-02 :
  |Input item|  Type |  Quantity |
  |:------:|:------:|:------:|
  | RM-02 | RM  | 3 |
  | RM-03 | RM | 5 |
  |SA-01  | SA  | 4|
 
###### Create a new Production Plan as shown below.

![4](/MRP/productionplan.png)
 
###### Report production of FG to System via **IIRS**.

![5](/MRP/iirs01.png)


 ## Generate Report

![8](/MRP/mrp.png)


The report is generated in excel and you can see the following various sheet in it.

A.Production Plan.

B. Final Production Plan.

C. Product wise consumption.

D. item wise consumption.

E.Item wise consumption Summery.

F.IIRS Qty.

 Production Plan Table : 

  So this is how Production Plan tables looks like 
 

 |Plan No | Period From | Period To | Product Id  | Product Name | Product Qty |
 |:------:|:------:|:------:|:-------:|:------:|:-----|
 |   000019   |  19-Jul-21  |   19-Jul-21 | 007138 | FG-01 | 50
 |  000080  |  19-Jul-21   |   19-Jul-21| 007139|FG-02|100


 
 Item Wise Consumption Summery:

 So this is how Item wise Consumption Summery looks like

 |Input Id | Item Shortname| Consumption | 
 |:------:|:------:|:-------:|
 |  007144|  SA-01|  420
 |  007146  |  SA-02  |  250
 |  007156 | RM-01 | 400
 | 007157 |RM-02 |440
 | 007158 |RM-03 |120



2.Production plan with adding pending order Quantity to plan Quantity.

Select this option if you want to add current pending order to your plan quantity.

 we can perform following step

-	Enter data as per previous steps.
-	Click on check box for adding pending order Qty to plan Qty.
-	If any other checkbox in checked , uncheck it.

![9](/MRP/mrp02.png)


In sales order if production order is pending it will add to plan order. 

Final production plan table : 

  So this is how Final production plan tables looks like 
 

 |Product Id | Product Name | Input Plan Qty | Pending Order Qty  | FG Stock Qty | Final Plan Qty |
 |:------:|:------:|:------:|:-------:|:------:|:-----|
 |   007238  |  FG-01 |   50 | 55 | 0 | 105
 |  007238 |  FG-02   |  60| 0|0|60

  Item Wise Consumption Summery:

 So this is how Item wise Consumption Summery looks like

 |Input Id | Item Shortname| Consumption | 
 |:------:|:------:|:-------:|
 |  007144|  SA-01|  420
 |  007146  |  SA-02  |  525
 |  007156 | RM-01 | 840
 | 007157 |RM-02 |660
 | 007158 |RM-03 |120

3.Production plan with Adjust FG Store Stock from Pending Orders

Select this option if you want to consider current FG stock and reduce it from pending orders.

 we can perform following step

-	Enter data as per previous steps.

-	Click on check box for adjust FG store stock from pending orders.

-	If any other checkbox in check, uncheck it.

     >Note: Example :- Suppose you have 1000 pending order of a particular product and 400 pic of that  product is already there in stock so if you check this box it will adjust the plan through 600.

4. Production plan with Adjust RM Store Stock in Procurement

 - Select this option if you want to Adjust RM Store Stock in Procurement with production plan. 

  we can perform following step
-	Enter data as per previous steps.

-	Click on check box for Adjust RM Store Stock in Procurement

-	If any other checkbox in check, uncheck it.


>Note: Example :- Suppose we have requirement of 1000 raw material and there is already stock of 200 raw material so if we want to adjust the balance of 800 raw material we can check this box.



5.Production plan with Scan BOM of Sub Assemblies to Workout Consumption

 Select this option if you want to Scan BOM of Sub Assemblies to Workout Consumption in production.

 We can perform following step
-	Enter data as per previous steps.

-	Click on check box for Scan BOM of Sub Assemblies to Workout Consumption

-	If any other checkbox in check, uncheck it.

Item wise consumption summery table : 

  So this is how Item wise consumption summery tables looks like 
 

 |Item Id | Item shortName | Consumption
 |:------:|:------:|:------:|
 |   007144  |  SA-01 |   420 |
 |  007146 |  SA-02   |  250|
 |  007156 | RM-01 | 400 |
|  007157 | RM-02 | 440 |
|  007158 | RM-03 | 120 |
|  007159 | RM-04 | 2940 |
|  007160 | RM-05 | 2000|

IIRS Qty table : 

  So this is how IIRS Qty tables looks like 
 
 |Itemid |Item Short Name | Process| Stage  | UOM | Consumption |
 |:------:|:------:|:------:|:-------:|:------:|:-----|
 |   007144 |  SA-01 |   FABRICATION | 07 | BOX | 420
 |  007146 |  SA-02   |  FABRICATION | 07 |BOX | 250
  |  007156 |  RM-01  |  FABRICATION | 00 |BOX | 400
   |  007157 |  RM-02   |  FABRICATION | 00 |BOX | 440
   |  007158 |  RM-03  |  FABRICATION | 00|BOX | 120
   |  007159 |  RM-04   |  FABRICATION | 00 |BOX | 2940
 |  007160 |  RM-05   |  FABRICATION | 00 |BOX | 2000


 6. Procurement plan without any checkbox.

- Select report type as Procurement Plan.

- Select Plan range from as 19-july-2021. 
- Select Plan range to as 19-july-2021.
- If any checkbox in check, uncheck it.
- Then click on submit to generate the report.

![10](/MRP/mrp03.png)

The report is generated in excel and you can see the following various sheet in it.

A.Procurement plan

B.Procurement Based On Max Order Level


Procurement plan table : 

  So this is how Procurement plan tables looks like 
 
 |Itemid |Item Short Name | Item Group name | Uom  | Computed Qty| Stock | Reorder Level | Pending Indent | Make Indent | QA Stock
 |:------:|:------:|:------:|:-------:|:------:|:-----|:------:|:-------:|:------:|:-----|
 |   007144 |  SA-01 |   ACCESSORIES | BOX | 420 | 0 |1 |0 | 421 | 0
 |  007146 |  SA-02   |  ACCESSORIES | BOX | 250 | 0 |1 |0 | 251 | 0
|  007156 |  RM-01  |   ACCESSORIES | BOX |400 | 0 |1 |0 | 401 | 0
|  007157 |  RM-02   |   ACCESSORIES | BOX | 440 | 0 |1 |0 | 441 | 0
|  007158 |  RM-03  |   ACCESSORIES | BOX |120 | 0 |1 |0 | 121 | 0
  

  9.Procurement plan  with adding pending order Quantity to plan Quantity

Select this option if you want to add current pending order to your plan quantity.

You can perform following step

-	Enter data as per previous steps.
-	Click on check box for adding pending order Qty to plan Qty.
-	If any other checkbox in checked , uncheck it.

Procurement plan table : 

  So this is how Procurement plan tables looks like 
 
 |Itemid |Item Short Name | Item Group name | Uom  | Computed Qty| Stock | Reorder Level | Pending Indent | Make Indent | QA Stock
 |:------:|:------:|:------:|:-------:|:------:|:-----|:------:|:-------:|:------:|:-----|
 |   007144 |  SA-01 |   ACCESSORIES | BOX | 420 | 0 |1 |0 | 421 | 0
 |  007146 |  SA-02   |  ACCESSORIES | BOX | 525 | 0 |1 |0 | 526 | 0
|  007156 |  RM-01  |   ACCESSORIES | BOX |840 | 0 |1 |0 | 841 | 0
|  007157 |  RM-02   |   ACCESSORIES | BOX | 660 | 0 |1 |0 | 660 | 0
|  007158 |  RM-03  |   ACCESSORIES | BOX |120 | 0 |1 |0 | 121 | 0

10. Procurement plan with Adjust FG Store Stock from Pending Orders

Select this option if you want to consider current FG stock and reduce it from pending orders in Procurement plan.

You can perform following step



-	Enter data as per previous steps.

-	Click on check box for adjust FG store stock from pending orders.

-	If any other checkbox in check, uncheck it.

     >Note: Example :- Suppose you have 1000 pending order of a particular product and 400 pic of that  product is already there in stock so if you check this box it will adjust the plan through 600.

11. Procurement plan with Adjust RM Store Stock in Procurement


 - Select this option if you want to Adjust RM Store Stock in Procurement with production plan. 

  we can perform following step

-	Enter data as per previous steps.

-	Click on check box for Adjust RM Store Stock in Procurement

-	If any other checkbox in check, uncheck it.


>Note: Example :- Suppose we have requirement of 1000 raw material and there is already stock of 200 raw material so if we want to adjust the balance of 800 raw material we can check this box.


12.Procurement plan with Scan BOM of Sub Assemblies to Workout Consumption

Select this option if you want to Scan BOM of Sub Assemblies to Workout Consumption in Procurement plan.

 We can perform following step
-	Click on check box for Scan BOM of Sub Assemblies to Workout Consumption

-	If any other checkbox in check, uncheck it.

Procurement plan table : 

  So this is how Procurement plan tables looks like with Scan BOM of Sub Assemblies.
 
 |Itemid |Item Short Name | Item Group name | Uom  | Computed Qty| Stock | Reorder Level | Pending Indent | Make Indent | QA Stock
 |:------:|:------:|:------:|:-------:|:------:|:-----|:------:|:-------:|:------:|:-----|
 |   007144 |  SA-01 |   ACCESSORIES | BOX | 420 | 0 |1 |0 | 421 | 0
 |  007146 |  SA-02   |  ACCESSORIES | BOX | 250 | 0 |1 |0 | 251 | 0
|  007156 |  RM-01  |   ACCESSORIES | BOX |400 | 0 |1 |0 | 401 | 0
|  007157 |  RM-02   |   ACCESSORIES | BOX | 440 | 0 |1 |0 | 441 | 0
|  007158 |  RM-03  |   ACCESSORIES | BOX |120 | 0 |1 |0 | 121 | 0
|  007158 |  RM-04  |   ACCESSORIES | BOX |2940 | 0 |1 |0 | 2941 | 0
|  007158 |  RM-05  |   ACCESSORIES | BOX |2000 | 0 |1 |0 | 2001 | 0



So here is a link for [Consumption Of Material](/blog/consumption-of-material) Blog


























