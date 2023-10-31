---
title: Sign in issue when app is blocked
description: Troubleshoot and resolve sign in issues when app is blocked.
ms.date: 10/31/2023
ms.topic: article
ms.service: microsoft-sales-copilot
ms.collection: highpri
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
---

# Sign in issue when app is blocked

This article helps you troubleshoot and resolve sign in issues when app is blocked by the administrator.

## Who is affected?

| Requirement type |Description  |
|---------|---------|
|**Client app**     |  Sales Copilot Outlook add-in and Teams app    |
|**Platform**     | Web and desktop clients         |
|**OS**     | Windows and Mac         |
|**Deployment**     | User managed and admin managed       |
|**CRM**     | Salesforce      |
|**Users**     | Users trying to authentication to their Salesforce instance |

## Symptoms

1. When trying to sign in to Salesforce CRM from Sales Copilot add-in for Outlook, the following error message is displayed: `Failure passed to redirect url. error=OAUTH_APP_BLOCKED error_description=this app is blocked by admin`

    :::image type="content" source="media/tsg-app-block-error.png" alt-text="Screenshot showing app blocked error.":::

2. In Salesforce CRM, Microsoft Power Platform is shown as blocked on the **Connected Apps OAuth Usage** page.

    :::image type="content" source="media/tsg-app-blocked.png" alt-text="Screenshot showing app blocked in Salesforce CRM.":::

## Root cause and resolution

### Issue 1: The Microsoft Power Platform app in Salesforce CRM is blocked by an administrator 

#### Root cause

Sales Copilot connects to Salesforce CRM through the **Microsoft Power Platform** connected app. When the **Microsoft Power Platform** app is blocked by an administrator, the Salesforce authentication process fails, threreby resulting in the error message.

#### Resolution

Sales Copilot uses the **Microsoft Power Platform** connected app to connect to Salesforce CRM. Ensure that the connected app is not blocked in Salesforce CRM.

1. Sign in to Salesforce CRM as an administrator.
1. Go to **Setup** > **Platform Tools** > **Apps** > **Connected Apps** > **Connected Apps OAuth Usage**.
1. For the **Microsoft Power Platform** app, select **Unblock**.
    The **Microsoft Power Platform** app disappears from the list, but it's unblocked.
    After the first successful sign-in from the first user using Sales Copilot, the **Microsoft Power Platform** app appears in the list again.


## Is your issue still not resolved?

Visit the [Sales Copilot - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.

