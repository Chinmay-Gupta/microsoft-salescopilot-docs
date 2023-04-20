---
title: Update fields in forms through Viva Sales admin settings
description: Troubleshoot and resolve error messages in Viva Sales related to field level security in Salesforce.
ms.date: 04/20/2023
ms.topic: article
ms.service: viva
ms.collection: highpri
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
ms.subservice: viva-sales
---

# Update fields in forms through Viva Sales admin settings

This article helps you troubleshoot and resolve error messages in Viva Sales related to field level security in Salesforce.

## Who is affected?

|  |  |
|---------|---------|
|**Client app**     |  Viva Sales Outlook add-in        |
|**Platform**     | Web and desktop clients         |
|**OS**     | Windows and Mac         |
|**Deployment**     | User managed and admin managed       |
|**CRM**     | Salesforce        |
|**Users**     | Users who do not have permissions to view fields added in Viva Sales forms   |


## Symptom

When using Viva Sales in Outlook, users see error such as "To see this data in Viva Sales, ask your Salesforce admin to delete the fields listed in the error details from Viva Sales."

## Root cause and resolution

### Root cause

Users don't have access to view all fields added in Viva Sales forms.

### Resolution

Change the admin settings from the Viva Sales admin settings in Microsoft Teams to hide the fields or remove edit capabilities.

1. Sign in to Microsoft Teams with your administrator credentials.
2. In the navigation bar on the left, select **Viva Sales**.
3. On the **Settings** tab, select Forms.
4. Select **Edit** for the entity you are seeing the error.
5. Under **Manage fields**, perform one of the following actions:
    - If the issue is related to editing of a field, turn off **Allow editing** for the corresponding field.
    - If the issue is related to viewing the field, hover over the field, and select **Remove field** (![Delete icon.](media/delete-icon.png "Delete icon")).
6. Select **Publish** to save your changes.

## Is your issue still not resolved?

Visit the [Viva Sales - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.
