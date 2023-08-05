---
layout: post
title: From implementation to audit - navigating SOX compliance
categories: [Security, Audit]
---
Ignoring SOX requirements during implementation is a pitfall, frequently overlooked until audits loom. The need for these requirements surfaces then, demanding swift implementation. Dynamics 365 finance and operations apps offers out-of-the-box features that aid in achieving compliance.

## Manage security rights
Role-based security assigns access to security roles, not individual users. These roles grant associated privileges. In finance and operations apps, this security aligns with business structure, and users are assigned based on responsibilities. Administrators grant access to duties, not program elements. Automatic role assignment rules streamline user role changes, and business managers control access based on data.

Out of the box, it offers you 200+ unique security roles that cover a variety of business processes. Think Accounting Manager, Accounting Supervisor, Accounts Payable Manager, Accounts Payable Clerk, and many more.

Microsoft recognizes the importance of adapting these security roles to individual needs. Therefore, creating new security roles is entirely possible.

User sign-in/sign-out auditing is enabled, logging sessions and allowing administrators access to audit logs via the User log page.

## Segregation of duties
Dynamics 365 finance and operations apps also incorporates a segregation of duties feature. This empowers a security admin to establish rules to ensure that distinct tasks are carried out by different users, a principle known as segregation of duties. For instance, an accounts payable clerk may not be allowed to both create vendors and process payments. The system will raise a flag if such a conflict arises.

## Embedded workflow capabilities
A workflow embodies a business process, showing how a document moves through the system, including tasks, decisions, and approvals. For example, a workflow for processing expense reports or to create a request for new user.

## Database logging
Database logging lets you track specific changes to tables and fields in finance and operations apps. This includes inserts, updates, deletes, and renaming key operations. When you enable logging for a table or field, the system stores a record of every change in the database log table. It's applicable to particular tables housing sensitive data.

## Audit trail
The audit trail is an inquiry page displaying transaction types, descriptions, creators, and creation times. 

## Alerts 
Alerts constitute a notification system for significant system events, offering you the means to stay informed about events you wish to monitor. Creating personalized alert rules is straightforward, ensuring timely updates about changing configurations and other noteworthy occurrences.

Change-based and due date alerts can be set up to utilize business events, serving as a mechanism to notify or activate external applications and systems.

**Even though they're built-in features, they need setup. Don't wait for audits – consider SOX requirements right from the start of implementation.**

**Gathering solid requirements sets the stage for a successful implementation journey.**

For more information, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/magnomgp).