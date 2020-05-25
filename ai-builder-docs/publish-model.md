---
title: Publish a model in AI Builder - AI Builder | Microsoft Docs
description: Provides steps by step instructions about how to publish your model in AI Builder.
author: Dean-Haas
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 01/03/2020
ms.author: joshrenn
ms.reviewer: v-dehaas
---

# Publish model

After you successfully train your model, you have to publish it to make it available. All users in your current environment can use your published model when you publish it.

On the details page, under **Last trained version**, select **Publish**.

> [!div class="mx-imgBorder"]
> ![Publish model screen](media/publish-model.png "Publish model screen")

After you publish your last trained version, it appears as the published version. For certain AI model types, you might need to take additional steps to use your model in Power Apps or Common Data Service.

> [!NOTE]
>
> - Any previous published version is overwritten when you publish a new version.
> - If you have a published version and a last trained version, you'll lose the published version when you unpublish because the last trained version is more recent.

## When should I publish my model?

Publish your model when you want to make it available to users in your Power Apps environment. If you aren't satisfied with your model, you can create a new version to try to yield better results. For information about how to create a new version, see [Manage a model in AI Builder](manage-model.md).

If you're satisfied with your model, you can publish it to make it available. Because you can only have up to two trained versions available at a time, you might publish a version because you don't want it to be overwritten by a new version.

### Next step

[Use your AI Builder model](use-model.md)

### Related topics

[Use AI Builder in Power Automate](use-in-flow-overview.md)  
[Use AI Builder in Power Apps](use-in-powerapps-overview.md)
