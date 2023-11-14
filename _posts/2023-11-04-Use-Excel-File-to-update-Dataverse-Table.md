---
layout: post
title: "Use an Excel file to update a Dataverse Table"
date: 2023-11-04 2:52:21
author: James
categories: dataverse, power app
---

To create a form to upload an Excel file to a Power App that updates an existing Dataverse table, you can follow these steps:

Sign in to Power Apps.
From the home screen, select Start with data > Create from data > Dataverse.
Select the table you want to update and click Connect.
From the Fields tab, select the fields you want to include in your form.
Click Form and select Edit.
From the Data tab, select Add field and choose File.
From the Advanced tab, select OnAddFile and enter the following formula: Patch(Table1, Defaults(Table1), {Filename: ThisItem.DisplayName, FileContent: ThisItem.'$content'}).
Save your form and publish it.
