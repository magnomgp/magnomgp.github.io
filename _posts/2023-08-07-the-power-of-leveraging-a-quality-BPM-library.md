---
layout: post
title: The power of leveraging a quality BPM library
categories: [Lifecycle Services]
---
The choice of a robust business process library can shape the entire implementation journey. From initial workshops, through testing, to user training, this library remains a constant companion. It documents processes, captures tests and acceptance, and continues to shine during rollouts for companies with similar needs.

## Business process modeler (BPM)
The Business Process Modeler (BPM) provided by Microsoft Dynamics Lifecycle Services (LCS) is an invaluable tool for identifying differences between standard company processes and how the system works. With BPM, you can conduct a fit-gap analysis between your business requirements and the default processes, as well as introduce new business processes that are not already defined. Empower yourself to optimize your system and streamline your processes with the help of BPM.

Learn the end-to-end scenarios and [business processes that Dynamics 365 supports out-of-the-box](https://learn.microsoft.com/en-us/dynamics365/guidance/business-processes/).

## Initiate
You have the option to begin your project with a pre-existing library of processes or create a new library from scratch. Creating a new library can be made faster by organizing it in Excel and importing it.

![](/images/the-power-of-leveraging-a-quality-BPM-library/bpm-import.png)
_When you click on "Import from Excel," the system lets you download a template that shows the acceptable Excel structure_

Once the process library is linked to the project according to its scope, it can synchronize with DevOps to **generate the work item structure automatically**.

![](/images/the-power-of-leveraging-a-quality-BPM-library/bpm-devops.png)
_Here is an example of how it can be structured_

You now possess the guide for the **workshops**. You can confidently start gathering the necessary requirements to carry out the **fit-gap analysis** at a later time.

## Implement
Now that you have completed the requirements gathering, conducted the fit and gap analysis, and addressed the gaps, it is time to consider the testing strategy.

You can rely on BPM once again to be your ally.

To create **user acceptance test** libraries, you can utilize Task recorder and Business process modeler (BPM). Task recorder enables you to record test cases and arrange them based on business processes using BPM, which is a highly efficient tool. Furthermore, BPM can be synchronized with Azure DevOps, allowing you to **automatically generate test cases (including test steps)** in your Azure DevOps project. By utilizing Azure DevOps, you can configure and manage your tests, create specific test plans and test suites, execute tests, and analyze results.

![](/images/the-power-of-leveraging-a-quality-BPM-library/sync_test_case.png)
_Sync test case_

![](/images/the-power-of-leveraging-a-quality-BPM-library/view_test_case.png)
_View test case_

![](/images/the-power-of-leveraging-a-quality-BPM-library/test_case_details.png)
_Add the test case to a test plan and test suite_

![](/images/the-power-of-leveraging-a-quality-BPM-library/add-dashboard-chart.png)
_Test plan dashboard_

## Prepare
Now it's time for **user readiness**. You have a BPM library with attached task recorders to provide hands-on guidance for the users to prepare.

You can use task recordings to create task guides that are an **important component of the Help experience**. These guides provide a structured and interactive experience for users to complete business processes step-by-step. Each step is accompanied by a pop-up prompt or "bubble" that highlights the relevant UI element and provides instructions on how to interact with it, such as "Click here" or "Enter a value in this field." Additionally, you can save task recordings as Word documents to create printable training guides easily.

![](/images/the-power-of-leveraging-a-quality-BPM-library/screen4.png)
_You can write your description and annotations to explain why the user is doing the step or to give additional context_

**It is absolutely crucial that you recognize the immense value of implementing BPM (Business Process Management) for long-term benefits that extend to future rollouts. With a systematic approach that involves implementing all necessary processes, documenting them thoroughly, conducting associated tests, and providing comprehensive training material for users, you can establish a rock-solid system that leaves nothing to chance. This is not an option, but a necessity, if you want to stay ahead of the curve and achieve sustained success.**

For more information, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/magnomgp).