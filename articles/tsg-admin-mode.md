---
title: Users don't have required privileges to access the organization
description: Troubleshoot and resolve error messages in Sales Copilot when users don't have required privileges to access the organization when Administration mode is enabled.
ms.date: 10/31/2023
ms.topic: article
ms.service: microsoft-sales-copilot
ms.collection: highpri
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
---

# User does not have required privileges to access the organization

This article helps you troubleshoot and resolve error messages in Sales Copilot when users don't having required privileges to access the organization when Administration mode is enabled.

## Who is affected?

| Requirement type |Description  |
|---------|---------|
|**Client app**     |  Sales Copilot Outlook add-in and Teams app    |
|**Platform**     | Web and desktop clients         |
|**OS**     | Windows and Mac         |
|**Deployment**     | User managed and admin managed       |
|**CRM**     | Dynamics 365      |
|**Users**     | Users trying to use Sales Copilot when Administration mode is enabled |

## Symptom

When users use Sales Copilot, they see the error message: **Something went wrong** with the following error description: `User does not have required privileges (or role membership) to access the org when it is in Admin Only mode.`

The error might be displayed before or after the user has signed in to an environment from Sales Copilot.

## Root cause and resolution

### Issue 1: Administration mode is enabled on the environment and affected users aren't administrators

#### Root cause

When an administrator enables **Administration mode** on an environment, regular users, regardless of their role assignment, won't be able to access the environment. If a user is already signed in or tries to sign in to the environment, won't be able to access data from the environment and will see the error message.

:::image type="content" source="media/tsg-admin-mode-enabled.png" alt-text="Screenshot showing administration mode enabled.":::

#### Resolution

To resolve this issue, the administrator must disable **Administration mode** on the environment. For more information, see [Administration mode](/power-platform/admin/admin-mode).

## Is your issue still not resolved?

Visit the [Sales Copilot - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.