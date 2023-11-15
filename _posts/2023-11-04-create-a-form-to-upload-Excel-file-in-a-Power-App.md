---
layout: post
title: "Create a form to upload Excel file in a Power App"
date: 2023-11-04 2:52:21
author: James
categories: dataverse, power apps, forms
---

To create a form to upload an Excel file to a Power App that updates an existing Dataverse table, you can follow these steps:

1. Sign in to **Power Apps**.
2. From the home screen, select **Start with data > Create from data > Dataverse**.
3. Select the table you want to update and click **Connect**.
4. From the **Fields tab**, select the fields you want to include in your form.
5. Click **Form** and select **Edit**.
6. From the **Data tab**, select **Add field** and choose **File**.
7. From the **Advanced tab**, select **OnAddFile** and enter the following formula: ~~~~Patch(Table1, Defaults(Table1), {Filename: ThisItem.DisplayName, FileContent: ThisItem.'$content'})~~~~.
8. Save your form and publish it.
