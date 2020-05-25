---
title: Use entity extraction model in Power Automate - AI Builder | Microsoft Docs
description: Provides step by step instructions to use AI Builder entity extraction in Power Automate.
author: mfotedar
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 3/19/2019
ms.author: mfotedar
ms.reviewer: v-dehaas
---

# Use an entity extraction prebuilt model in Power Automate

[!INCLUDE[cc-beta-prerelease-disclaimer](./includes/cc-beta-prerelease-disclaimer.md)]

> [!IMPORTANT]
 > To use AI Builder models in Power Automate, you have to create the flow inside a solution. The steps below won't work if you don't follow these instructions first: [Create a flow in a solution](/flow/create-flow-solution).

1. Sign in to [Power Automate](https://flow.microsoft.com/), select the **My flows** tab, and then select **Automated-from blank**.
1. Enter a name for your flow.
1. Search for *email*, select **When an email arrives** in the list of triggers, and then select **Create**.
1. Select **+ New step**, search for *html to text*, and then select **Html to text** in the list of actions.
   > [!div class="mx-imgBorder"]
   > ![Select 'html to text'](media/html-to-text.png "Select 'html to text'")
1. Select **+ New step**, search for *predict*, and then select the **Predict Common Data Service (current Environment)** action.
   > [!div class="mx-imgBorder"]
   > ![Choose an a action'](media/predict-cds-2.png "Select 'Predict Common Data Service'")

    >[!NOTE]
    > **Predict Common Data Service (current Environment)** doesn't appear unless you've followed these instructions first: [Create a flow in a solution](/flow/create-flow-solution).
1. Select **EntityExtraction model**. In the **Sentence** field select the **plain text** parameter.
1. Select **+ New step**, search for *Add a row into a table*, and then select the **Add a row into a table** action.
1. Complete the necessary fields to find the location of your excel table. Make sure you created a table and designated columns where you want to store the results of entity extraction. Find the results of entity extraction in the available dynamic content such as **Entity type** and **Entity value** as shown here:
   > [!div class="mx-imgBorder"]
   > ![Add a row to table'](media/flow-add-row2.png "Add a row to table")

Congratulations! You've created a flow that uses a entity extraction model. Select **Save** in the upper-right corner, and then select **Test** to try out your flow.

### Related information:

[Entity extraction model](prebuilt-entity-extraction.md)

[AI Builder in Power Automate overview](use-in-flow-overview.md)