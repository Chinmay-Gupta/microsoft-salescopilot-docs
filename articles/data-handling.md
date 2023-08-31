---
title: Data handling in Sales Copilot 
description: Know how data is handled in Sales Copilot 
ms.date: 10/03/2022
ms.topic: article
ms.service: viva
ms.collection: highpri
author: sbmjais
ms.author: shjais
manager: shujoshi
ms.localizationpriority: medium
ms.subservice: viva-sales
---


# Data handling in Sales Copilot 

[!INCLUDE[vs-rebrand-note](includes/vs-rebrand-note.md)]

This article gives you an overview of how data is handled in Sales Copilot.

Sales Copilot is built on the [Microsoft Power Platform](https://powerplatform.microsoft.com/). Sales Copilot data is stored in [Dataverse](/powerapps/maker/common-data-service/data-platform-intro) in addition to the connected CRM.

## Data retention 

Since Sales Copilot data is stored in [Dataverse](/powerapps/maker/common-data-service/data-platform-intro), data retention policies differ from other Microsoft 365 applications and non-Dynamics 365 CRM solutions. For example, when your Microsoft 365 subscription ends, your data is retained for 90 days before it's automatically deleted (in accordance to [Microsoft 365 data retention policies](/microsoft-365/compliance/retention-policies)). However, if you use Sales Copilot, that data isn't automatically deleted 90 days after your subscription ends.  

## Sales Copilot, Dataverse, and your CRM

When Sales Copilot is connected to Dynamics 365, Sales Copilot data is stored with the Dynamics 365 Sales Dataverse instance.

When Sales Copilot is connected to a non-Dynamics 365 CRM, a default Dataverse instance specific to Sales Copilot is provided to your tenant. Sales Copilot data is stored in the default instance in addition to your CRM. 

You can find the name and details of your default Dataverse instance named **msdyn_viva** in the [Power Platform admin center](https://admin.powerplatform.microsoft.com/).

> [!NOTE]
> The msdyn_viva environment is of type **Trial**. Do not convert the environment to **Production**.

:::image type="content" source="media/ppac-admin-center.png" alt-text="Screenshot that shows the default Dataverse instance in Power Platform admin center.":::

## Delete Sales Copilot data 

If you need to delete Sales Copilot data (for example, delete data for a specific user), you can choose to [manually delete it](/power-platform/admin/remove-user-personal-data). 

### See also

[Introduction to Microsoft Sales Copilot](introduction.md)<br>
[Install Sales Copilot](install-viva-sales.md)
