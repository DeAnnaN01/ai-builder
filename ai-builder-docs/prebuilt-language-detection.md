---
title: Language detection prebuilt AI model - AI Builder | Microsoft Docs
description: Describes the prebuilt language detection AI Builder model.
author: alanabrito
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 05/11/2020
ms.author: alanab
ms.reviewer: v-dehaas
---

# Language detection model

The prebuilt language detection model identifies the predominant language of a text document. The model analyses the text and returns the detected language and a numeric score between 0 and 1. Scores close to 1 indicate higher confidence in the result. The detected language is returned as the "script" of the language. For instance, for the phrase "I have a dog" it will return "en" instead of "en-US". The response for languages that can't be detected is **unknown**.

## Use in Power Apps

### Use the formula bar

You can integrate your AI Builder language detection models by using the formula bar. More information: [Use formulas for text AI models (Preview)](use-model.md#use-formulas-for-text-ai-models-preview)

## Use in Power Automate

If you want to use this prebuilt model in Power Automate, you can find more information in [Use language detection model in Power Automate](flow-language-detection.md).

## Supported language and data format

- Documents can't exceed 5,120 characters.
- For information on language support, see [Language and region support for the text analytics API](/azure/cognitive-services/text-analytics/language-support?#language-detection).


## Model output

If text is detected, the language detection model will output the following information:

- **Results**: A list of languages detected in the input text.
- **Language**: Script version of the language code (ex.: "en", "fr", "zh_chs", "ru")
- **Score**: Numeric value from 0 to 1 where values close to 1 indicate 100% confidence that the identified language is true
