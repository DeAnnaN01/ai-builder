---
title: Sentiment analysis prebuilt AI model - AI Builder | Microsoft Docs
description: Describes the prebuilt sentiment analysis AI model in AI Builder.
author: alanabrito
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 12/12/2019
ms.author: alanab
ms.reviewer: v-dehaas
---

# Sentiment analysis model

The sentiment analysis prebuilt model detects positive or negative sentiment in text data. You could use it to analyze social media, customer reviews, or any text data you want to analyze. Sentiment analysis evaluates text input, and gives scores and labels at a sentence and document level. The scores and labels can be positive, negative, and neutral. At the document level, there can also be a mixed sentiment label, which has no score. The sentiment of the document is determined by aggregating the sentence scores.

## Use in Power Apps

### Explore sentiment analysis

You can try out the sentiment analysis model before you decide to import it into your flow by using the 'try it out' feature.

1. Sign in to [Power Apps](https://make.powerapps.com).
1. In the left navigation pane, select **AI Builder** > **Build**.
1. Under **Get straight to productivity**, select **Sentiment Analysis**.
1. In the **Sentiment Analysis** window, select **Try it out**.
1. Select predefined text samples to analyze, or add your own text in the **Add your own here** box to see how the model analyzes your text.

### Use the formula bar

You can integrate your AI Builder sentiment analysis models in Power Apps maker studio by using the formula bar. More information: [Use formulas for text AI models (Preview)](use-model.md#use-formulas-for-text-ai-models-preview)

## Use in Power Automate

If you want to use this prebuilt model in Power Automate, you can find more information in [Use sentiment analysis model in Power Automate](flow-sentiment-analysis.md).
  
## Supported language and data format

- Documents can't exceed 5,120 characters.
- For information on language support, see [Language and region support for the text analytics API](/azure/cognitive-services/text-analytics/language-support?#sentiment-analysis-key-phrase-extraction-and-named-entity-recognition).

## Model output

If text is detected, the sentiment analysis model will output the following information: 
- **Sentiment**: 
    - Positive
    - Negative
    - Neutral
    - Mixed
- **DocumentScores**: Value in the range of 0 to 1. Values close to 1 indicate greater confidence that the identified sentiment is accurate.
- **Sentences**: List of sentences from the input text with analysis of its sentiments.
    - **Sentiment**:
        - Positive
        - Negative
        - Neutral
        - Mixed
    - **SentenceScores**: Value in the range of 0 to 1. Values close to 1 indicate greater confidence that the sentiment is accurate.
