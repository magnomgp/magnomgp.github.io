---
layout: post
title: From implementation to audit - navigating SOX compliance
categories: [Security, Audit]
---
Ignoring SOX requirements during implementation is a pitfall, frequently overlooked until audits loom. The need for these requirements surfaces then, demanding swift implementation. Dynamics 365 finance and operations apps offers out-of-the-box features that aid in achieving compliance.

## Manage security rights
Role-based security assigns access to security roles, not individual users. These roles grant associated privileges. In finance and operations apps, this security aligns with business structure, and users are assigned based on responsibilities. Administrators grant access to duties, not program elements. Automatic role assignment rules streamline user role changes, and business managers control access based on data.

Out of the box, it offers you 200+ unique security roles that cover a variety of business processes. Think Accounting Manager, Accounting Supervisor, Accounts Payable Manager, Accounts Payable Clerk, and many more.

Microsoft recognizes the importance of adapting these security roles to individual needs. Therefore, creating new security roles is entirely possible. And with the help of Extensible Data Security (XDS) policies, developers can add an extra layer to role-based security by limiting access to table records based on specific security rules.

### Reports and inquiries

![](/images/from-implementation-to-audit-navigating-SOX-compliance/user-role-assignments.png)
_The User role assignments report generates a view of the current user role assignments in your system_

![](/images/from-implementation-to-audit-navigating-SOX-compliance/security-duty-assignments.png)
_The Security duty assignments report provides a view of all the duties contained within a role_

Additional security reports can be generated to enhance the audit of system security. One such report is the Security Role Access Report. It shows you the actual permissions for each security role in an easy-to-understand way. This report breaks down the permissions by type and includes all the sub-roles, duties, and privileges within the main role.

User sign-in/sign-out auditing is enabled, logging sessions and allowing administrators access to audit logs via the User log page.

## Segregation of duties
Dynamics 365 finance and operations apps also incorporates a segregation of duties feature. This empowers a security admin to establish rules to ensure that distinct tasks are carried out by different users, a principle known as segregation of duties. For instance, an accounts payable clerk may not be allowed to both create vendors and process payments. The system will raise a flag if such a conflict arises.

![](/images/from-implementation-to-audit-navigating-SOX-compliance/segregation-of-duties-conflicts.png)
_If a security role's definition or a user's role assignments go against the rules, it's noted as a conflict. These conflicts need to be sorted out by the administrator_

## Embedded workflow capabilities
A workflow embodies a business process, showing how a document moves through the system, including tasks, decisions, and approvals. For example, a workflow for processing expense reports or to create a request for new user.

![](/images/from-implementation-to-audit-navigating-SOX-compliance/create-a-request-for-new-user.jpg)

## Database logging
Database logging lets you track specific changes to tables and fields in finance and operations apps. This includes inserts, updates, deletes, and renaming key operations. When you enable logging for a table or field, the system stores a record of every change in the database log table. It's applicable to particular tables housing sensitive data.

## Audit trail
The audit trail is an inquiry page displaying transaction types, descriptions, creators, and creation times. 

## Alerts 
Alerts constitute a notification system for significant system events, offering you the means to stay informed about events you wish to monitor. Creating personalized alert rules is straightforward, ensuring timely updates about changing configurations and other noteworthy occurrences.

Change-based and due date alerts can be set up to utilize business events, serving as a mechanism to notify or activate external applications and systems.

## Electronic reporting
You can utilize electronic reporting (ER) to generate the necessary SOX reports without needing to involve development. The setup can be managed by a super user, and you don't need a developer for configuration. Instead of dealing with code, you configure formats, making it faster and easier to create and adjust formats for electronic documents.

ER currently supports the TEXT, XML, JSON, PDF, Microsoft Word, Microsoft Excel, and OPENXML worksheet formats.

**Even though they're built-in features, they need setup. Don't wait for audits – consider SOX requirements right from the start of implementation.**

**Gathering solid requirements sets the stage for a successful implementation journey.**

For more information, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/magnomgp).