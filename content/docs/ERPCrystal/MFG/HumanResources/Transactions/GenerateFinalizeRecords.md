---
title: "Generate / Finalize Records"
date: 2022-03-12
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
# - HumanResourcesOverview
# - Generate/Finalize Records

---

## Introduction

Users can generate / finalize payroll records for last date of each month for the selected financial year.


#### Mandatory Fields

|Mandatory Fields|  
  |:------|   
  | Year <br> - Select from year combo list.
  | Pay Date <br> `Validations` <br> - If the month is already finalized, You can NOT generate records now. <br> - If the  month is already finalized, You can NOT finalize records again. <br> - If pay records are not generated for the month, System is unable to finalize. <br> - Previous month is not yet finalized. Please finalize it before generating records.
  | Options <br> - Pre selected as Generate Records (Generate Records, Finalize Records) <br> `Validations` - **System is unable to finalize pay records for this month, because net pay or balance loan is negative in some cases. Please run Payroll Analysis to get more details.** In case Loan amount or deductions are more than the gross pay then pay can become negative and this message will be displayed.{{< callout type="info" >}}You can amend loan installments in payroll analysis to solve this.  {{< /callout >}}
  | Checkbox <br> - I confirm that Holiday Master has been setup for this month and can NOT be modified.