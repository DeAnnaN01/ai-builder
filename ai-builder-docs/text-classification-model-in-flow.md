---
title: Use category classification model in Power Automate - AI Builder | Microsoft Docs
description: Provides information about how to use a category classification model in Power Automate.
author: raaourik
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 12/12/2019
ms.author: raaourik
ms.reviewer: v-dehaas
---

# Use category classification model in Power Automate


[!INCLUDE[cc-beta-prerelease-disclaimer](./includes/cc-beta-prerelease-disclaimer.md)]

> [!IMPORTANT]
 > To use AI Builder models in Power Automate, you have to create the flow inside a solution. The steps below won't work if you don't follow these instructions first: [Create a flow in a solution](/flow/create-flow-solution).

1. Sign in to [Power Automate](https://flow.microsoft.com/), select the **My flows** tab, and then select **Create from blank**.

1. Search for *manually*, select **Manually trigger a flow** in the list of triggers, and then select **+Add an input**.
1. Select **Text** and set as input title: **My Text**
1. Select **+ New step**, search for **Predict**, and then select **Predict Common Data Service (current Environment)** in the list of actions.
    >[!NOTE]
    > **Predict Common Data Service (current Environment)** doesn't appear unless you've followed these instructions first: [Create a flow in a solution](/flow/create-flow-solution).
1. Select the category classification model you want to use, and then:

   - In the **Text** field, add **My Text** from the trigger.
   - In the **Language** field, select the 2 letter language code for the supported language you want to use.

      > [!div class="mx-imgBorder"]
      > ![Trigger a flow screen](media/trigger-flow.png "trigger a flow screen")

1. In your flow's successive actions, you can iterate through the outputs returned by the category classification model. The following example, saves each inferred tag into a SharePoint list.

    > [!div class="mx-imgBorder"]
    > ![Trigger a flow example](media/trigger-flow-example.png "trigger a flow example")

Congratulations! You've created a flow that uses a category classification AI Builder model. Select **Save** in the upper-right corner, and then select **Test** to try out your flow.

To learn more about the triggers and actions, see [Get started with Power Automate](/flow/getting-started).

### Related topic

[Category classification model overview](text-classification-overview.md)
