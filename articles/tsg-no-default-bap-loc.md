---
title: No default BAP location found for this tenant 
description: Troubleshoot and resolve issues in Sales Copilot when users are unable to use Sales Copilot due to missing default environment
ms.date: 10/19/2023
ms.topic: article
ms.service: microsoft-sales-copilot
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
---

# No default BAP location found for this tenant

This article helps you troubleshoot and resolve issues in Sales Copilot when users are unable to use Sales Copilot due to missing default environment.

## Who is affected?

| | |
|----------------|--------------------|
| **Client App** | MS Outlook Only        |
| **Platform**   | Any (Web & Desktop)    |
| **OS**         | Any (Mac & Windows)    |
| **Deployment** | User and admin managed |
| **CRM**        | CRM less experience    |
| **Users**      | Users who do not have any Dynamics 365 licenses  |


## Symptom 

When you open the Sales Copilot pane in Microsoft Outlook, the following error message is displayed: `No default BAP location found for this tenant`. 

:::image type="content" source="media/tsg-bap-location.png" alt-text="Screenshot showing BAP location error.":::

## Root cause and resolution

### Issue 1: Default environment is not created in Power Apps

#### Root cause

Sales Copilot requires a Power Apps environment for every organization. When Sales Copilot is launched for the first time, it calls a Power Platform API to get the region details. If the organization does not have an existing Power Platform environment an error message is displayed when attempting to get region details.

#### Resolution

To resolve the issue, navigate to [Power Platform admin center](https://admin.powerplatform.microsoft.com/). A default environment is created for the tenant.

## Is your issue still not resolved?

Visit the [Sales Copilot - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.