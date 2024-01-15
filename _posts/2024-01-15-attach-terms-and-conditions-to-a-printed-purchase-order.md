---
layout: post
title: Attach terms and conditions to a printed purchase order 
categories: [Business document management, Electronic reporting]
---
Business document management is a useful feature built on top of the Electronic Reporting (ER) framework. It is a **no-code/low-code solution** that assists businesses in editing documents according to their requirements. Users can start from a Microsoft template or create a document from scratch.

One common requirement in my project experience is to attach Terms and Conditions (TCs) to a printed purchase order or invoice. Rather than customizing SSRS reports, we can leverage the capabilities of the Electronic Reporting framework to extend the Business document and achieve this without any code changes.

We can create a configuration for Electronic Reporting by using the current Purchase Order layout and then simply adding your TCs extension.

![](/images/attach-terms-and-conditions-to-a-printed-purchase-order/image002.png)

In the extended configuration, we have the option to include additional components, such as PDF files. In my scenario, I have added two PDF files - one with the Terms and Conditions (TCs) in English for non-Portuguese vendors and another with TCs in Portuguese for Portuguese vendors.

![](/images/attach-terms-and-conditions-to-a-printed-purchase-order/image003.png)

After adding the two complements, we can use formulas in the enabled property of the mapping configuration to control their visibility based on the vendor's language.

**Terms and Conditions for non-Portuguese Vendors**

![](/images/attach-terms-and-conditions-to-a-printed-purchase-order/image004.png)

**Terms and Conditions for Portuguese Vendors**

![](/images/attach-terms-and-conditions-to-a-printed-purchase-order/image005.png)

It is now time to mark the ER configuration version as completed, update the printout configurations, and run tests.