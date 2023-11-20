---
layout: post
title: Streamline product master data translations through automation
categories: [Product information management, Power automate, AI builder]
---
**Low-code solutions** should always be considered when addressing a GAP. Here's a quick example demonstrating how the **Power Platform can enhance a Dynamics 365 Supply Chain Management** process GAP through low-code implementation.

The deal is, whenever the master data expert creates a new product in D365 SCM, they want the **product and description translations to just auto-populate or get suggested automatically**.

The Power Automate flow kicks in when a business event happens in D365 SCM. We're talking about using the Alerts category specifically, with the business event called 'When an alert rule is triggered.' To make this work, setting up an Alert rule configuration in D365 SCM is needed for this type of business event.

![](/images/streamline-product-master-data-translations-through-automation/alerts.png)

To send alerts outside your organization, use the business events framework. When setting up an alert, make sure to set Organization-wide to No and toggle Send externally to Yes. - [How to create alert rules](https://learn.microsoft.com/en-us/dynamics365/fin-ops-core/fin-ops/get-started/create-alerts)

