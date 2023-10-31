---
title: Sign in issue when opening the Sales Copilot pane in Outlook
description: Troubleshoot and resolve error messages in Sales Copilot when users encounter problem in opening the Sales Copilot pane in Outlook.
ms.date: 10/31/2023
ms.topic: article
ms.service: microsoft-sales-copilot
ms.collection: highpri
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
---

# Sign in issue when opening the Sales Copilot pane in Outlook

This article helps you troubleshoot and resolve error messages in Sales Copilot when users encounter problem in opening the Sales Copilot pane in Outlook.

## Who is affected?

| Requirement type |Description  |
|---------|---------|
|**Client app**     |  Sales Copilot Outlook add-in        |
|**Platform**     | Web    |
|**OS**     | Windows and Mac         |
|**Deployment**     | User managed and admin managed       |
|**CRM**     | Dynamics 365 and Salesforce        |
|**Users**     | All users   |

## Symptom

When you open the Sales Copilot pane in Microsoft Outlook, the following error message is displayed: `There was a problem starting Sales Copilot`. When you copy the error details, the error name displayed is: `Error occurred in the authentication request from Office`. 

:::image type="content" source="media/tsg-sign-in-error.png" alt-text="Sign-in error":::

## Root cause and resolution

### Issue 1: Pop-up or cross-site tracking is blocked in the browser

#### Root cause

When you open the Sales Copilot Outlook add-in, an authentication pop-up window is opened to link the add-in to the current Outlook context. If pop-up or cross-site tracking is blocked in the browser, the add-in is not authenticated and the error message is displayed.

#### Resolution

You must allow pop-ups and cross-site tracking in the browser. Different browsers have different settings to allow pop-ups and cross-site tracking. We have provided the steps to allow pop-ups and cross-site tracking in the following browsers:

##### Edge

You'll receive a notification in the address bar if pop-ups are blocked. Select the option to always allow pop-ups from the Office 365 website. After you allow pop-ups, refresh the page, and then open the Sales Copilot add-in.

:::image type="content" source="media/tsg-sign-in-error-popup.png" alt-text="Pop-up blocked notification.":::

If the notification doesn't appear in the address bar, follow these steps:

1. Open browser settings.

1. In the left pane, select **Cookies and site permissions**.

1. In the right pane, select **Pop-ups and redirects**.

1. In the **Allow** section, select **Add**, enter `https://outlook.office365.com`, and then select **Add**.

    :::image type="content" source="media/tsg-sign-in-error-popup-allow-edge.png" alt-text="Allow pop-ups in Edge.":::

1. Refresh the page, and then open the Sales Copilot add-in.

##### Chrome

You'll receive a notification in the address bar if pop-ups are blocked. Select the option to always allow pop-ups from the Office 365 website. After you allow pop-ups, refresh the page, and then open the Sales Copilot add-in.

:::image type="content" source="media/tsg-sign-in-error-popup.png" alt-text="Pop-up blocked notification.":::

If the notification doesn't appear in the address bar, follow these steps:

1. Open browser settings.

1. In the left pane, select **Privacy and security**.

1. In the right pane, select **Site settings**, and then select **Pop-ups and redirects**.

1. In the **Allowed to send pop-ups and use redirects** section, select **Add**, enter `https://outlook.office365.com`, and then select **Add**.

    :::image type="content" source="media/tsg-sign-in-error-popup-allow-chrome.png" alt-text="Allow pop-ups in Chrome.":::

1. Refresh the page, and then open the Sales Copilot add-in.

##### Safari


1. In the Safari browser, select **Safari** > **Settings**, and then select **Privacy**.

1. Clear the **Prevent cross-site tracking** checkbox. 

    :::image type="content" source="media/tsg-sign-in-error-safari.png" alt-text="Prevent cross-site tracking in Safari.":::

1. Refresh the page, and then open the Sales Copilot add-in. When asked to allow pop-ups, allow pop-ups from the Office 365 website.
    
    If you allowed pop-ups, refresh the page, and then open the Sales Copilot add-in.

### Issue 2: Browser needs to clear session and restart

#### Root cause

In some scenarios, the browser session needs to be cleared and restarted to resolve the issue.

#### Resolution

1. Sign out from Outlook on the web.
1. Close all browser tabs and windows.
1. Open the browser and sign in to Outlook on the web.
1. Open the Sales Copilot add-in.

## Is your issue still not resolved?

Visit the [Sales Copilot - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.