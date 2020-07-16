---
title: Расширения интеллектуального облака Business Central для миграции в облако | Microsoft Docs
description: Используйте расширения облачной миграции для переноса локальных данных в сетевую версию Business Central. Эти расширения перемещают ваши локальные данные в облако, чтобы вы могли использовать сетевую версию Business Central с вашими существующими данными.
author: jenolson
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.reviewer: edupont
ms.date: 06/22/2020
ms.author: jenolson
ms.openlocfilehash: 5b1ed470b4150c49fd20776718ab7429e7fbf3b8
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528542"
---
# <a name="intelligent-cloud-extensions-for-cloud-migration"></a><span data-ttu-id="43885-104">Расширение интеллектуального облака для миграции в облако</span><span class="sxs-lookup"><span data-stu-id="43885-104">Intelligent Cloud Extensions for Cloud Migration</span></span>

<span data-ttu-id="43885-105">Это расширение соединит ваши данные локальной версии [!INCLUDE[prodshort](includes/prodshort.md)] с сетевой версией [!INCLUDE[prodshort](includes/prodshort.md)] для целей миграции вашего решения в облако.</span><span class="sxs-lookup"><span data-stu-id="43885-105">This extension will connect your data from [!INCLUDE[prodshort](includes/prodshort.md)] on-premises with [!INCLUDE[prodshort](includes/prodshort.md)] online for purposes of migrating your solution to the cloud.</span></span>  

<span data-ttu-id="43885-106">Если используется локальная версия одного из поддерживаемых продуктов, можно настроить среду облака на основе специального расширения для этого продукта.</span><span class="sxs-lookup"><span data-stu-id="43885-106">If you are using one of the supported on-premises products, you can configure your cloud environment based on a product-specific extension.</span></span><span data-ttu-id="43885-107"> После настройки вашей среды облака можно будет перенести данные из вашего локального решения в [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="43885-107"> Once your cloud environment is configured, you will be able to migrate data from your on-premises solution to [!INCLUDE[prodshort](includes/prodshort.md)].</span></span> <span data-ttu-id="43885-108">Это позволит вам полностью использовать преимущества облака для вашего бизнеса, такие как улучшенный анализ бизнеса, искусственный интеллект, доступ с нескольких устройств и доступ в любой момент из любого места.</span><span class="sxs-lookup"><span data-stu-id="43885-108">This will enable you to take full advantage of what the cloud has to offer your business such as, enhanced insights into your business, artificial intelligence, multiple device access, and anytime, anywhere access.</span></span>  

<span data-ttu-id="43885-109">Для получения дополнительной информации см. раздел [Миграция локальных данных в Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data) в материалах для администраторов [!INCLUDE[prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="43885-109">For more information, see [Migrating On-Premises Data to Business Central Online](/dynamics365/business-central/dev-itpro/administration/migrate-data) in the administration content for [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>  

## <a name="business-central-on-premises"></a><span data-ttu-id="43885-110">Локальная версия Business Central</span><span class="sxs-lookup"><span data-stu-id="43885-110">Business Central on-premises</span></span>
<span data-ttu-id="43885-111">Если используется локальное развертывание [!INCLUDE[prodshort](includes/prodshort.md)], получите расширения **Основа интеллектуального облака** и **Интеллектуальное облако Business Central**, затем выполните мастер настройки **Настройка миграции в облако**.</span><span class="sxs-lookup"><span data-stu-id="43885-111">If you are using an on-premises deployment of [!INCLUDE[prodshort](includes/prodshort.md)], get the **Intelligent Cloud Base** extension and the **Business Central Intelligent Cloud** extension, and then run the **Cloud Migration Setup** assisted setup guide.</span></span>  

## <a name="dynamics-gp"></a><span data-ttu-id="43885-112">Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="43885-112">Dynamics GP</span></span>
<span data-ttu-id="43885-113">Если используется Dynamics GP, получите расширения **Базовое расширение интеллектуального облака** и **Интеллектуальное облако Dynamics GP**, затем запустите мастер настройки **Настройка миграции в облако**.</span><span class="sxs-lookup"><span data-stu-id="43885-113">If you are using Dynamics GP,  get the **Intelligent Cloud Base Extension** extension and the **Dynamics GP Intelligent Cloud** extension, and then run the **Cloud Migration Setup** assisted setup guide.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="43885-114">Миграция из Dynamics GP с использованием мастер настройки **Настройка миграции в облако** в настоящее время поддерживается только для следующих рынков: США, Канада, Великобритания.</span><span class="sxs-lookup"><span data-stu-id="43885-114">Migrating from Dynamics GP using the **Cloud Migration Setup** assisted setup guide is currently only supported for the following markets: United States, Canada, United Kingdom.</span></span>

## <a name="dynamics-sl"></a><span data-ttu-id="43885-115">Dynamics SL</span><span class="sxs-lookup"><span data-stu-id="43885-115">Dynamics SL</span></span>
<span data-ttu-id="43885-116">Если используется Dynamics SL, получите расширения **Базовое расширение интеллектуального облака**, **Интеллектуальное облако Microsoft Dynamics SL** и **Смарт-листы истории Microsoft Dynamics SL**, затем запустите мастер настройки **Настройка миграции в облако**.</span><span class="sxs-lookup"><span data-stu-id="43885-116">If you are using Dynamics SL, get the **Intelligent Cloud Base Extension** extension, the **Microsoft Dynamics SL Intelligent Cloud** extension and the **Microsoft Dynamics SL History Smartlists** extension, and then run the **Cloud Migration Setup** assisted setup guide.</span></span>  

## <a name="see-also"></a><span data-ttu-id="43885-117">См. также</span><span class="sxs-lookup"><span data-stu-id="43885-117">See Also</span></span>

[<span data-ttu-id="43885-118">Интеллектуальная аналитика</span><span class="sxs-lookup"><span data-stu-id="43885-118">Intelligent Insights</span></span>](about-intelligent-cloud.md)  
[<span data-ttu-id="43885-119">Базовое расширение интеллектуального облака</span><span class="sxs-lookup"><span data-stu-id="43885-119">Intelligent Cloud Base Extension</span></span>](ui-extensions-intelligent-cloud.md)  
