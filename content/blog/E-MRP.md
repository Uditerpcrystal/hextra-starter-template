---
title: "Enhanced MRP"
date: 2021-04-20
draft: false
author: "ERP Crew"
description: "Guide to download E-MRP report"
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- Enhanced MRP report
categories:
- Manufacturing
---

# Introduction

E- MRP means Enhanced material requirement planning. To increase production planning, scheduling we used E- MRP.

## Enhanced MRP
- On options page, show run date that is current date only. You have option to select unit.
- If print working is no then only final allocation, make indent and excess indent will appear in report.Otherwise option is yes pending indent, indent allocation, FG allocation will appear in report.
- Click on submit button and report gets downloaded.
- If print working is yes, report is downloaded with pending indent, indent allocation, FG allocation etc.
1. P_Indents : Shows pending indent qty.
2. MTA : Make to Availability shows how many items are available.
3. FG_08 : Shows FG packed allocation with pending indent qty,total of pending indent qty, stock qty, allocated qty and balance qty.
4. FG_07 : Shows FG unpacked allocation with pending indent qty,total of pending indent qty, stock qty, allocated qty and balance qty.
5. RM_Reqd : Shows requirements qty of raw material.
6. RM_Stock : Shows store stock qty and safety stock and finally how many allocable qty is there.
7. RM_Allocation : Shows allocation of raw material according to RM qty, Total RM qty , Stock qty and finally allocated qty.
8. Indent_Allocation : According to BOM type, RM qty, pending indent qty, total RM qty allocate indent qty and finally shows balance.
- If print working is no then
1. Final Allocation : According to BOM type, RM qty, stock allocation, indent allocation done final allocation of order.
2. Make Indent : Indent making details shows over here.
3. Excess Indent : After calculating pending indent qty, allocate the stock qty and finished with making indent whatever excess indent qty is there will appear over here.
