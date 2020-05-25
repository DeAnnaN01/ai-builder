---
title: Business card prebuilt AI model- AI Builder | Microsoft Docs
description: Describes the business card prebuilt AI Builder model.
author: alanabrito

ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 10/04/2019
ms.author: alanab
ms.reviewer: v-dehaas
---

# Business card model

The business card prebuilt AI model allows you to extract information from business card images. If it detects a business card in the image, the AI model extracts the information such as name, job title, address, email, company, and phone numbers.

> [!NOTE]
> The design and format of business cards varies widely. AI Builder is constantly improving the accuracy of the business card AI model, but it's possible there could be inaccurate or missing information in some cases. It's a good idea to verify that the output is as you expect!

## Licensing requirements

AI Builder is licensed as an add-on to your Power Apps or Power Automate licenses. For information about license capacity, pricing, and restrictions, see [AI Builder licensing](administer-licensing.md).

## Role requirements

Users need to have the Common Data Service user role to consume the business card reader.

## Use in Power Apps

If you want to use this prebuilt model in Power Apps using the Business card reader component. You can find more information in [Use business card reader component in Power Apps](business-card-reader-component-in-powerapps.md).

## Use in Power Automate

If you want to use this prebuilt model in Power Automate, you can find more information in [Use business card model in Power Automate](flow-business-card-reader.md).

## Supported language, format, and size

The images you can process with the business card model need these characteristics:

- Language: English.
- Format:
  - JPG
  - PNG
  - BMP
- Size: 6 MB maximum

## Model output

If a business card is detected, the business card model will try to locate and extract the following properties:

|Property |Definition  |
|---------|---------|
| **AddressCity**| The city address|
| **AddressCountry**| The country address|
| **AddressPostalCode**| The postal code address|
| **AddressPostOfficeBox**| The post office box address|
| **AddressState**| The state address|
| **AddressStreet**| The street address|
| **BusinessPhone**| The first phone or fax number|
| **CleanedImage**| The image after processing where the business card appears cropped and enhanced from the original image|
| **CompanyName**| The company name|
| **Department**| The organization department found|
| **Email**| The contact email found in the business card, if any|
| **Fax**| The third phone or fax number|
| **FirstName**| The contact first name|
| **FullAddress**| The contact full address|
| **FullName**| The contact full name|
| **JobTitle**| The contact job title|
| **LastName**| The contact last name|
| **MobilePhone**| The second phone or fax number|
| **OriginalImage**| The original image before processing|
| **Website**| The website|
