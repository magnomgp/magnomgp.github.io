---
layout: post
title: Electronic reporting – configure the vendor payment filename
categories: [Electronic Reporting, Accounts Payable]
---
## Why?
- As an accounts payable clerk, when I generate a vendor payment, I would like to export the **payment file with a specific name** to be easier to identify the payment.

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image1.webp)

I will show you how to transform the ISO20022 credit transfer filename dynamic. Filename output “As is” and “To be” analysis:

## As is (filename provided by Microsoft)
“ISO20022 Credit transfer”
- Fixed filename.

## To be (you want to have a dynamic output)
NURG_ISO20022 Credit transfer_280520201601
- “NURG” – service level configured in the method of payment and copied to the journal. Dynamic output.
- “ISO202002 Credit transfer” – free text and set in the ER parameters. Fixed output.
- “280520200555” – date and time set in the ER parameters. Dynamic output.

After imported from LCS repository all the GER configurations, you should do the following steps to achieve the to be filename purposed.
1. Go to **Electronic reporting workspace** > Reporting configurations > Payment model > ISO20022 Credit transfer > ISO20022 Credit transfer (CE), here CE correspond to country extension;
2. Click on **Create configuration**;
3. Select **Derive from Name: ISO20022 Credit Transfer (CE), Microsoft**;
4. Enter a **Name and Description**. E.g. Name: CM_ISO20022 Credit Transfer CE and description: Core Model ISO20022 Credit Transfer CE.
5. **Configuration provider** will be automatically filled in with the configuration provider that you have created.
5.1 In case you didn’t have created:
5.1.1. Go to **Organization administration** > Electronic reporting > Configuration provider table;
5.1.1.1. Click on New.
5.1.1.2. Enter your company name in the name column;
5.1.1.3. Enter your company internet address in the internet address column.
5.1.2. Go to **Electronic reporting workspace** > Configuration providers;
5.1.2.1. Click on the provider created and set as active.
6. Click on **Create configuration.**

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image2.jpeg)

7. After the configuration created, you should click on **Designer**.

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image3.jpeg)

8. Select the **XML Header** and click on **Mapping**.

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image4.jpeg)

9. On the bottom of the page, in the right side, click on **Filename** edit.

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image5.jpeg)

10. And now, on the Formula side, you can enter the formula that you want.
10.1. You have different ways how to use the formula designer. More details here: [Formula designer in Electronic reporting (ER)](https://docs.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/analytics/general-electronic-reporting-formula-designer)
10.2. On my example, I am using the advanced formula editor.
11. On the left, you have the Data Soure.
12. On the right, you have all the Formulas available.
13.Once you have entered the formula, you can test and save it.
13.1 More details about formula language and functions: [Electronic reporting formula language](https://docs.microsoft.com/en-us/dynamics365/fin-ops-core/dev-itpro/analytics/er-formula-language?toc=%2Fdynamics365%2Fcommerce%2Ftoc.json)

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image6.jpeg)

14. You should change the status to **Complete**. 

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image7.jpeg)

15. Finally, you are ready to start to **generate payments** with the file name that you want.
15.1. In the method of payment, in the field “Export format configuration” you should have selected the format configuration created (CM_ISO20022 Credit Transfer (BE)).

![](/images/electronic-reporting-configure-the-vendor-payment-filename/image8.jpeg)