---
title: "5 Star"
description: ""
date: 2022-10-06T00:08:29+09:00
draft: false
weight: 1
---
<!-- ##### Approve Party Credit Limit with unique token
- You can optionally create an approval code or a unique token from System Tools. The token will valid only for five mins. You can share the token with another user for changing the credit limit of a Party. -->
<!-- Added approval code for  -->
<!-- ##### Approve Sales order if there is an oustanding with unique token
- You can optionally create an approval code or a unique token from System Tools. The token will valid only for five mins only. You can share the token with another user for creating the sales order even if there is an outstanding amount for that party.
##### Map Party to Invoice/Bill Transaction Type
- In Party Master you can setup the default transaction type for invoices as well as purchase bills. When you create an invoice or a purchase bill System will show you Auto Fetch option against transaction types. In case you want to select another TRN type instead auto fetching some party master, you may do so.
##### ERP Crystal Website has been redesigned
- You can now create Support Requests for clarifying any doubts, new reports or bug fixes.
- You can also get to know new features which are introduced, while signing in.
##### Import Bulk Price Records
- Option to create multiple Price/Cost records from XL template is introduced.
##### Create Multiple Lead Time Records
- Option to create multiple records of lead time & transit days from XL template is introduced.
##### Handle NAPS, Capped PF in Payroll
- New Pay Basis to compute pay for NAPS worker is available.
- Option to cap PF deduction at Rs.1800p.m. is introduced.
##### Maker Checker IIRS
- In IIRS, several transaction types (e.g. Issue to Shop floor, Transfer to FG store) have been introduced.
- For each transaction type, you can allot roles for creating as well as for approving IIRS entries.
- While Maker/Checker IIRS are being approved, System will check for negative stock qty. -->

<!-- #### Approve Sales order if there is an outstanding with unique token
- To use this feature you need to change the approval code and party credit limit status to "On".
- You can create an approval code or a unique token from System Tools. 
- The token will valid only for five mins only.
- The token can be used to create a sales order by another user.
- The other user can use this code to create a sales order even if the party for which they are creating the sales order has an outstanding amount.
- This provides temporary access to the system for a specific purpose, without giving ongoing access to the user. -->

<!-- #### Bypass party credit limit with approval code
- You can optionally create an approval code or a unique token from System Tools. The token will valid only for five mins. You can share the token with another user for changing the credit limit of a Party. -->

#### E-Invoice Feature
- E-Invoices can now be directly generated and uploaded with a single click, with the help of the E-Invoice feature in Sales Invoice.

#### Email Feature in Receivables and Payables
- Email Feature is now enabled in Receivables and Payables
#### Audit Trail reports are now available in the System
- As per MCA rules all companies have to maintain a complete Trail of creation, modification, deletion of all financial documents in their ERP Systems. We have now enabled this optional feature. 
#### Added Combo Unit and changed the date condition in Indent.
- Previously on the main level, you were not able to change the indent from in the modify.
- Now you can change the indent from in the modify as well.
- When making a line level modification, if the user enters a "to be received by" date that is less than the indent creation date, a message will be displayed.
- The message will indicate that the "to be received by" date cannot be less than the indented date.
The system will prevent the user from submitting the modification until a valid "to be received by" date is entered, which is not less than the indent creation date.

#### Indent Sub No.
- A Sub No logic is being added to the indent creation.
- The Sub no will be based on the new feature called Indent type.
- The Indent type will be a drop-down and it will be a mandatory field.
- The user needs to select a particular indent type
- Based on the indent type Sub-no will be generated by the system.
- The import of Indent logic is also changed.
- Now you can only import one indent at a time with multiple items.
- You can also see the Indent sub no and type added in the pdf print as well.

#### Import Voucher.
- Previously the voucher date was taken from the system while importing multiple vouchers.
- Now the user will have a column in the Excel model for adding the voucher date as per user requirements.
- There are a few validations as well for the voucher dates.
    1. The user needs to add the voucher date more than the latest voucher date.
    2. The voucher date cannot be more than the current date.
#### Assign a transaction type of invoice/bill to a specific party. 
- In Party Master, you can choose the default transaction type for invoices and purchase bills.
- When you create an invoice or purchase bill, the system suggests a transaction type using Auto Fetch.
- If you don't want to use the suggested transaction type, you can choose a different one.

#### ERP Crystal Website has been redesigned
- You can now create Support Requests for clarifying any doubts, new reports or bug fixes.
- You can also get to know new features which are introduced, while signing in.
#### Import Bulk Price Records
- You can now create multiple Price/Cost records using an Excel template.
- This new feature allows you to quickly and easily add many new records at once, without having to enter them manually one by one.
#### Create Multiple Lead Time Records
- This feature includes the option to create records for both lead time and transit days.
#### Handle NAPS, Capped PF in Payroll
- New Pay Basis to compute pay for NAPS worker is available.
- New feature has been added that allows for capping of PF deductions at Rs. 1800 per month.
#### Maker Checker IIRS
- To use the Maker/Checker IIRS feature in the system, you need to turn it on in the system parameters.
- In IIRS, new transaction types have been introduced (e.g. Issue to the Shop floor, Transfer to FG store, etc.).
- For each transaction type, you can assign roles for creating and approving IIRS entries.
- When using the Maker/Checker IIRS feature, the entries created by a "Maker" must be approved by a "Checker" before they can be posted to the system.
- During the approval process, the system will check for any negative stock quantities to prevent errors in inventory management.

#### Import Masters through Excel
- Excel can be used to create many new records in the system at once.
- This feature is available for the following masters: Party, Item, Employee, Contact, Account, and Ceiling/Floor Price Master.
- However, you can only use Excel to create records if there are currently no records in the system for that master.

#### Ship to in Sales Order.
- A new form has been created where you have to give the ship-to details.
- You will find it on the sales order details page under GST info and ship-to details.

#### Deletion of line-level BOM
- Now you need to specify the reason for the deletion of the line-level BOM.

#### HSN-DNCN Sheet in the GSTR1 report.
- Added a new sheet in the GSTR1 report named HSN-DNCN.

#### Added item state in import IIRS.
- When adding data from Excel into the system, a new drop-down menu has been added for the item state.
- The item state can be either "good" or "rejected" for the particular sheet you are creating.
- The "rejected" option will only be available for "Account Scrap" and "Miscellaneous" transaction types.

#### Added Mode in Transporter.
- A new "mode" option has been added for transporters in the system.
- This option is used when creating DNCNs, and if the transporter name and mode are mismatched, an error will occur.

<!-- #### MKRCKR IIRS stock check.
- Now, the stock will not be checked while creating an MKRCKR IIRS through System and Import too. -->

#### "Financial Year" option removed from Inventory Reports.
- First, we were using the financial year drop-down.
- Now we are using the session year or the work year you have selected.

#### Sales Order Print
- The bill-to and ship-to will render with a new table in the PDF.

#### Voucher Print
- Voucher pdf printing has been reorganized with a new pdf rendering utility.

#### Creation and deletion disabled in Prospect Mst.
- While creating a prospect it will be active by default.
- You cannot create or delete the records if it is inactive.

#### Making a Duplicate Voucher.
- Added few validations while duplicating the voucher.
- One of them is if the amount is 0 you cannot duplicate that voucher.

#### Job Work Report.
- Added number of boxes in the excel report of Job Work.
#### Invoice Print
<!-- - Invoice pdf printing has been reorganized with a new pdf rendering utility. -->
- Printing invoices in PDF format has been made easier with a new tool.

#### Added NA option in QA Protocol.
- Added an option of NA in the Is QA Done drop down.
- This will be shown on the grid and details of the QA protocol.