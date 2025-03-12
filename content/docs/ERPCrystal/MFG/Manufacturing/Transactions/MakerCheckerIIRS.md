---
title: "Maker Checker IIRS"
date: 2022-02-17
draft: false
author: "ERP Crew"
description: ""
pinned: false
hideToc: false
enableToc: true
enableTocContent: false
weight : 9

---

## Introduction
- Maker Checker IIRS is a type of IIRS. You may refer to article on IIRS for more information.
- You need to create 3 types of roles viz., Maker, Checker and QC.
- These roles may have to be created for each transaction type.

> Once Maker Checker IIRS is enabled in the System. You will not be able to create, modify and delete Normal IIRS.

#### Transaction Types
|Transaction Types|
|:------|
| Full Kit Issue to Production.
| Loose Kit Issue to Production.
| Material Return to RM Stores (MRS).
| FG Transfer (Production to FG stores).
| FG to Production for Printing / Re-printing.
| After Re-Work to FG stores.
| Account Scrap.
| Miscellaneous.

#### Maker/Checker Operation
|Maker/Checker Operation|
|:------|
| Only Maker can create, modify and delete IIRS transactions.
| Only Checker can approve IIRS transactions.
| QC Approval is also required before checker can approve in case of transaction types <br> - Material Return to RM stores (MRS). <br> - FG Transfer (Production to FG stores).
| {{<callout>}} **Maker** 
- During create, modify or delete operations same validation as per Normal IIRS will be enforced. {{</callout>}}
| {{<callout>}} **Checker**
- Duplicate item, brand, stage not allowed.
- If Stock is not adequate for any item, brand, stage approval will be aborted.
- IIRS can be approved only for the current Financial Year. {{</callout>}}

##### Points to note:
> - Maker can also create IIRS through Import from Excel option. 
> - Maker Checker IIRS will not be posted in Inventory Ledger.
> - In view of point 2 above, Maker Checker IIRS if not approved within 48 hours from creation will be auto deleted by System. 
