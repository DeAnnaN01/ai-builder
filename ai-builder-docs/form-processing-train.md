---
title: Train and publish your form processing model - AI Builder | Microsoft Docs
description: Walks you through the steps to train, validate, and test your form processing model in AI Builder.
author: JoeFernandezMS

ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 12/31/2019
ms.author: jofernan
ms.reviewer: v-dehaas
---

# Train and publish your form processing model


After you create your form processing model, you can train, test, and publish it to make it available.

## Train and validate your model

1. Select **Next** to check your selected form fields. If everything looks good, select **Train** to train your model.
1. When training completes, select **Go to Details page** in the **Training complete** screen.

## Quick-test your model

The Details page allows you to test your model before you publish or use it:

1. On the Details page, select **Quick test**.
2. You can either drag and drop a document, or select **Upload from my device** to upload your test file. The quick-test should only take a few seconds before displaying the results.
3. Select **Start over** to run another test, or **Close** if you're finished.

## Troubleshooting tips

If you have trouble training your model, try these suggestions:

- Optimize your data using the guidance in the [Requirements](form-processing-model-requirements.md).
- If you're getting bad results or low confidence scores for certain fields, create a new Form Processing model and upload more documents. The more documents you tag, the more AI Builder will learn how to better recognize the fields.
- Download and test with [sample material](https://go.microsoft.com/fwlink/?linkid=2103171).

## Publish your model

If you're happy with your model, you can select **Publish** to publish it. When publishing completes, your model is promoted as **Published** and is ready to be used. For more information about publishing your model, see [Publish your model](publish-model.md).

After you've published your form processing model, you can use it in a [Power Apps canvas app](/ai-builder/form-processor-component-in-powerapps) or in [Power Automate](/ai-builder/form-processing-model-in-flow).

### Related topics

[Form processing model in Power Automate](form-processing-model-in-flow.md)  
[Form processing model in Power Apps](form-processor-component-in-powerapps.md)
