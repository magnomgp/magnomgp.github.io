---
layout: post
title: Financial period close workspace – business case
categories: [General Ledger, Workspace]
---
## Why?
- We aren’t happy with the whiteboard where we **list all the month-end close tasks**. Just available physically in the office and permanently cleaned by the facility services team.

![](/images/financial_period_close_workspace-business_case/image1.webp)

- The Excel with the **month-end close tasks and responsible** send every month by email, without being an “online” file, was impossible to manage and not clear about what is happening.

![](/images/financial_period_close_workspace-business_case/image2.webp)

### Options
1. Do nothing.
2. Implement the **Financial period close workspace** and the associated configuration.

![](/images/financial_period_close_workspace-business_case/image3.webp)

### Benefits
> The Financial period close workspace lets you **track your financial closing processes across companies, areas, and people.** Depending on your view of the Financial period close workspace, you’ll see either of all tasks and statuses for a closing schedule, or just the tasks that are assigned to you.

## Financial period close workspace

How does it work?

![](/images/financial_period_close_workspace-business_case/image4.jpg)

- **Summary tiles** – give you a quick sumarize view.

![](/images/financial_period_close_workspace-business_case/image5.jpg)

- **Task and status view options** – different ways to show the task list and track the progress.

![](/images/financial_period_close_workspace-business_case/image6.jpg)

- **Indicators are used for tasks** – an exclamation point icon indicates that the task is past due and a padlock icon indicates that the task depends.

![](/images/financial_period_close_workspace-business_case/image7.jpg)

- **Task link** – a hyperlink to the page where the user should go to complete the task. 

![](/images/financial_period_close_workspace-business_case/image8.jpg)

- **Edit, add and remove** – users with permissions to view all tasks can add tasks to the task list, edit tasks, or remove tasks from the task list.

- **Completed date** – the tasks past due, the due date is highlighted in red.

![](/images/financial_period_close_workspace-business_case/image9.jpg)

- **Attachments** – could be used to add external documents or links. Links as power BI dashboards, bank dashboard, management report or other types of URLs.

![](/images/financial_period_close_workspace-business_case/image10.jpg)

Once completed the task, the user should check it √ . The dependencies will be updated.

## All financial period close tasks list page

This page is very useful if you need to export all the information for reporting or for audit purposes. You can see the “big picture”.

![](/images/financial_period_close_workspace-business_case/image11.webp)

## Financial period close configuration page

Here you are the list of things that you need to configure to use the workspace. You should go to General ledger > Period close > Financial period close configuration.

- **Closing roles** – could be organised by positions ( e.g. Accountant, AP Invoicing Clerk, etc).
- **Resources** – assign the employees to the financial closing process with the respective closing role and view options.
- **Task areas** – areas of action could be organised by team or modules (e.g. Accounts payable, Bank. etc).
- **Calendars** – calendars could be organised by year or quarter. It should reflect the work-days and also holidays.
- **Templates** – the most important part, the default “check-list”. There you should list the tasks organised by area, closing role, companies and task link. You also can set dependencies and associated attachments. Differents template could be created, for example, month-end template and quarter close template. Lastly, the due date could also be defined relating it with the period close date.
- **Closing schedules** – the last set up to be ready the workspace. You should schedule all the closing periods in a list, for example, Jan20, Feb20, Mar20(Q1), etc. It will be based on the period close start date and close date (from Friday, Jan. 31 to Friday, Feb. 7).

## Financial period close ideas

### Use Power Automate to

- Notify
- Assignment questionnaires for audits
- Attach documents
- And more… be creative…
Based on **business events** “alert rules” or getting a **custom entity** with all financial period close tasks.

### Use Power BI to

- Track the current status of the period close process and do performance analysis for insights into the efficiency. 
Based on the **excel downloaded from the All financial period close tasks page** or connection the **custom entity**.

For example, a dashboard to support the status meeting with the team.

![](/images/financial_period_close_workspace-business_case/image12.webp)

Some KPIs, all of them can be filtered by company.

- Workload by Area (team)
- Completed by Completed by (user)
- Task by Responsible (workload by user)
- Count Completed (tasks completed)
