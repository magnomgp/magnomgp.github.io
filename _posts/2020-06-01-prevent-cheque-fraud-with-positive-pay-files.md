---
layout: post
title: Prevent cheque fraud with positive pay files
categories: [Cash and bank management, Accounts Payable]
---
Prevent your business from fraudulent cheques. Although the cheque usage dropped or has been phase-out, registered fraud has increased according to [UK Finance](https://www.ukfinance.org.uk/system/files/Fraud-The-Facts-2020-FINAL-ONLINE-18-March.pdf).

![](/images/prevent-cheque-fraud-with-positive-pay-files/image1.webp)

##Positive pay overview
This post provides a **business process model** of how you can use the positive pay in **Microsoft Dynamics 365 Finance.**
> Positive pay is used to generate an electronic list of checks that can be presented to a bank. Positive pay files can help banks prevent check fraud. You set up positive pay to generate an electronic list of checks every time that checks are printed. Then, when a check is presented to the bank, the bank compares the check with the list of checks that you previously submitted. If the check matches a check in the list, the bank clears it. If the check doesn’t match a check in the list, the bank holds it for review.

### 1st – Send the cheque to the vendor

![](/images/prevent-cheque-fraud-with-positive-pay-files/image2.png)

### 2nd – Generate a positive pay file

![](/images/prevent-cheque-fraud-with-positive-pay-files/image3.pmg)

Generate a positive pay file for a single bank accout
- Go to the **Bank accont**
- Click on **Positive pay file**
- Enter the **Cut-off date**
    - “enter the last check date to include in the positive pay file. All checks that haven’t been included in a positive pay file by the end of this check date are included in the file.”

Generate a positive pay file for multiple bank accounts
- Go to Cash and bank management > **Periodic tasks > Positive pay file**
- Enter the **Format**
- Select all Companies and Bank accounts
    - Or you can specify the company and bank account
- Enter the **Cut-off date**

Positive pay file summary inquiry
- Go to Cash and bank management > Inquiries and reports > **Positive pay**
- You can see the cheque details clicking on **Positive pay file details**

![](/images/prevent-cheque-fraud-with-positive-pay-files/image4.jpg)

![](/prevent-cheque-fraud-with-positive-pay-files/image5.jpg)

### 3rd – The bank compares the cheque with the positive pay file

![](/images/prevent-cheque-fraud-with-positive-pay-files/image6.png)

### 4th – Confirm a positive pay file

![](/images/prevent-cheque-fraud-with-positive-pay-files/image7.png)

- Go to Cash and bank management > Inquiries and reports > **Positive pay**
- Select the positive pay file paid and click on **Enter confirmation**
- Enter the **confirmation number** receive from the bank

## Setups check-list
- Set up a **positive pay format**
    - Cash and bank management > Setup > Positive pay format
    - Ask your bank about the format, and you can manage it through the XSLT file
- Assign the positive pay format to a **bank account**
    - Cash and bank management > Bank accounts
- Assign a **number sequence** for positive pay files
    - Cash and bank management > Setup > Cash and bank management parameters > Number sequences