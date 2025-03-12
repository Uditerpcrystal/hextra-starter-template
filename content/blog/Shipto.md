---
title: "Ship To in ERP Crystal"
date: 2022-11-11
draft: false
author: "ERP Crew"
description: "Guide to uses ship to in Sales order and invoice."
pinned: true
hideToc: false
enableToc: true
enableTocContent: false
tags: 
- Shipto

---

### Introduction
We have introduced the Ship to a new way in the Erp System.
This will help you to have your ship-to info in one place itself, you don't need to rewrite the ship-to address in the sales order and also in the invoice. This feature will also be effective for the e-invoice also.

### Steps to use the ship-to and how it will work:
1. In Sales order

    - First, we were giving the ship To as a complete textbox where you can enter the entire ship to address and the Pincode having a different text box in the Sales order create form.
    - That is not in use now, instead a new link is being given.
    - The name of the link is <b>Create/Modify Ship to info</b>. You will find this link on the sales order details page in the GST info, Ship to details section.
    - When a link is clicked, a form will show up where you have to add all the fields individually. 
    -	All fields are mandatory to be filled. It also has a combo where the user has to select the state based on the given list of States.
   - Once all the text fields are saved for a particular sales order, the task is finished at the sales order.
  > Note: This will be effective for newly created sales orders as well as previously created sales orders.

2.  In Invoice.

    - In the invoice first, we were telling the users to add the ship to details in the main level create form. But now that is also not in use now.
    - The ship-to info will be taken from the sales order as soon as you create line-level data for a particular order number where you have given the ship to details.
    - For E-Invoice ship-to details are required, which were first given to enter into the create-form of the main-level invoice.
    - Now that also comes under the ship-to info and details.
> Note: The ship-to data will be fetched from the first line-level invoice only.

3.  Steps to update the ship-to details in the invoice from the sales order:

    - To see if the correct ship-to details are fetched or not. We have given a link where you will get to see the ship-to details.
    - You can find that link on the invoice details page under the transport E-way bill details section. The name of the link is <b>"Bill to/ Ship to details"</b>.
    - If the ship-to details are not according to your requirements then there is a link called <b>"Update from the first item of the invoice."</b>.
    - When the link is clicked it will update the ship-to from the first item of the invoice.
    - If there is no ship-to info for that item in the sales order then a validation message will show on the details saying <b>"there are no ship-to details for that order number."</b>
    - If you want to change the ship-to in the invoice you have to go to the sales order for the order number you have got the validation message and you have to follow the steps mentioned on '1'.
    - Once the ship-to details are filled in the sales order for that particular order number you can click on the <b>"Update from the first item of the invoice."</b> link which will update your ship-to details in the invoice for the order number you have changed or added the ship to details.
    - If you want to modify the ship to details in the invoice then you need to change the ship to details in the sales order for the order number of the first item in the invoice line-level.