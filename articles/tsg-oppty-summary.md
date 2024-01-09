---
title: Opportunity summary not displayed in deal rooms
description: Troubleshoot and resolve issues when the opportunity summary isn't displayed in deal rooms.
ms.date: 01/09/2024
ms.topic: article
ms.service: microsoft-sales-copilot
author: sbmjais
ms.author: shjais
ms.custom:
  - ai-gen-docs-bap
  - ai-gen-title
  - ai-seo-date:11/21/2023
  - ai-gen-desc
---

# Opportunity summary not displayed in deal rooms

This article helps you troubleshoot and resolve issues when the opportunity summary isn't displayed in deal rooms.

## Who is affected?

| Requirement type |Description  |
|---------|---------|
|**Client app**     |  Copilot for Sales app in Teams        |
|**Platform**     | Web and desktop clients         |
|**OS**     | Windows and Mac         |
|**Deployment**     | User managed and admin managed       |
|**CRM**     | Dynamics 365 and Salesforce      |
|**Users**     | Users trying to update a CRM record from Copilot for Sales |

## Symptom

When you create a deal room from Copilot for Sales in Outlook, and then open it in the Copilot for Sales app in Microsoft Teams, the opportunity summary isn't displayed in the deal room. The following message is displayed instead: `To unlock AI-powered opportunity summaries, install the Copilot for Sales Teams app.`

:::image type="content" source="media/tsg-oppty-summary-error.png" alt-text="Screenshot showing a message instead of opportunity summary.":::

## Root cause and resolution

### Issue 1: Copilot for Sales Teams app isn't installed

#### Root cause

When you set up a deal room from Copilot for Sales in Outlook, the Copilot for Sales Teams app and bot are automatically installed for the selected team, and opportunity summary is displayed in the deal room. If the Copilot for Sales Teams app isn't installed for the team, a message is displayed instead of the opportunity summary in the deal room.

#### Resolution

To resolve this issue, you must manually install the Copilot for Sales Teams app and bot for the team, and then generate the opportunity summary again.

1. In Microsoft Teams, hover over the team name, and then select **More options (...)** > **Manage team**.

2. Go to the Apps tab, and then select **Get more apps**.

3. Search for **Copilot for Sales**, and then select its card.

4. Select the down arrow next to **Open**, and then select **Add to a team**.

    :::image type="content" source="media/tsg-oppty-summary-add-team.png" alt-text="Screenshot showing option to add the app to a team.":::

    The **Add Copilot for Sales to a team** dialog box is displayed with the team name preselected.

5. Select **Set up a bot**.

    :::image type="content" source="media/tsg-oppty-summary-bot.png" alt-text="Screenshot showing button to set up a bot.":::

6. Open the deal room channel, and select **Start a post**.

7. In the message box, type `@Copilot for Sales`, select the Copilot for Sales app, type `show opportunity summary`, and then select **Post** to generate the opportunity summary.

    :::image type="content" source="media/tsg-oppty-summary-generate.png" alt-text="Screenshot showing prompt to generate opportunity summary.":::

## Is your issue still not resolved?

Visit the [Copilot for Sales - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/viva-sales/bd-p/VivaSales) to engage with our experts.
