---
title: Key phrase extraction prebuilt AI model - AI Builder | Microsoft Docs
description: Describes the prebuilt key phrase extraction AI model in AI Builder.
author: alanabrito
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 05/11/2020
ms.author: alanab
ms.reviewer: v-dehaas
---

# Key phrase extraction model

The key phrase extraction model identifies the main points in a text document. For example, given input text "The food was delicious and there were wonderful staff", the service returns the main talking points: "food" and "wonderful staff". This model can extract a list of key phrases from unstructured text documents.

## Use in Power Apps

### Explore key phrase extraction

You can try out the key phrase extraction model before you decide to import it into your flow by using the 'try it out' feature.

1. Sign in to [Power Apps](https://make.powerapps.com).
1. In the left navigation pane, select **AI Builder** > **Build**.
1. Under **Get straight to productivity**, select **Key Phrase Extraction**.
1. In the **Key Phrase Extraction** window, select **Try it out**. 
1. Select predefined text samples to analyze, or add your own text in the **Add your own here** box to see how the model analyzes your text.

### Use the formula bar

You can integrate your AI Builder sentiment analysis models in Power Apps maker studio by using the formula bar. More information: [Use formulas for text AI models (Preview)](use-model.md#use-formulas-for-text-ai-models-preview)

## Use in Power Automate

If you want to use this prebuilt model in Power Automate, you can find more information in [Use key phrase extraction model in Power Automate](flow-key-phrase-extraction.md).
 
## Supported language and data format

- Documents can't exceed 5,120 characters.
- For information on language support, see [Language and region support for the text analytics API](/azure/cognitive-services/text-analytics/language-support?#sentiment-analysis-key-phrase-extraction-and-named-key phrase-recognition).

## Model output

If text is detected, the key phrase extraction model will output the following information:

- **Results**: A list of phrases from the document
- **Phrase**: Strings denoting the key talking points in the document text
