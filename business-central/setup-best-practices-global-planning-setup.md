---
title: Рекомендации по настройке глобального планирования | Документация Майкрософт
description: На экспресс-вкладке "Планирование" на странице "Производство - настройка" приводится несколько полей, которые определяют глобальные правила для планирования поставок.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: c91bde42378992ef1c1e9613fb94d9bac2d4f57c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785352"
---
# <a name="setup-best-practices-global-planning-setup"></a><span data-ttu-id="af9c1-103">Рекомендации по настройке. Глобальная настройка планирования</span><span class="sxs-lookup"><span data-stu-id="af9c1-103">Setup Best Practices: Global Planning Setup</span></span>
<span data-ttu-id="af9c1-104">На экспресс-вкладке **Планирование** на странице **Производство - настройка** приводится несколько полей, которые определяют глобальные правила для планирования поставок.</span><span class="sxs-lookup"><span data-stu-id="af9c1-104">The **Planning** FastTab on the **Manufacturing Setup** page contains several fields that define global rules for supply planning.</span></span>  

 <span data-ttu-id="af9c1-105">В следующей таблице приведены рекомендации по настройке выбранных глобальных полей параметров планирования.</span><span class="sxs-lookup"><span data-stu-id="af9c1-105">The following table provides best practices on how to set up selected global planning parameter fields.</span></span> <span data-ttu-id="af9c1-106">Для получения дополнительных сведений о полях выберите ссылку в столбце **Поле настройки**.</span><span class="sxs-lookup"><span data-stu-id="af9c1-106">For more information about a field, choose the link in the **Setup field** column.</span></span>  

|<span data-ttu-id="af9c1-107">Настройка поля</span><span class="sxs-lookup"><span data-stu-id="af9c1-107">Setup field</span></span>|<span data-ttu-id="af9c1-108">Рекомендация</span><span class="sxs-lookup"><span data-stu-id="af9c1-108">Best practice</span></span>|<span data-ttu-id="af9c1-109">Комментарий</span><span class="sxs-lookup"><span data-stu-id="af9c1-109">Comment</span></span>|  
|-----------------|-------------------|-------------|  
|<span data-ttu-id="af9c1-110">Использовать прогноз по складам</span><span class="sxs-lookup"><span data-stu-id="af9c1-110">Use Forecast on Locations</span></span>|<span data-ttu-id="af9c1-111">Выберите, если есть прогнозы для определенных складов.</span><span class="sxs-lookup"><span data-stu-id="af9c1-111">Select if you have forecasts for specific locations.</span></span>||  
|<span data-ttu-id="af9c1-112">Компоненты по складам</span><span class="sxs-lookup"><span data-stu-id="af9c1-112">Components at Location</span></span>|<span data-ttu-id="af9c1-113">Если товары не определены как единицы хранения, выберите код склада в главном складе.</span><span class="sxs-lookup"><span data-stu-id="af9c1-113">If items are not defined as SKUs, select the location code of your main warehouse.</span></span>|<span data-ttu-id="af9c1-114">Это также верно, если используется только журнал заявок.</span><span class="sxs-lookup"><span data-stu-id="af9c1-114">This also applies if you only use the requisition worksheet.</span></span>|  
|<span data-ttu-id="af9c1-115">Общий допустимый избыток</span><span class="sxs-lookup"><span data-stu-id="af9c1-115">Blank Overflow Level</span></span>|<span data-ttu-id="af9c1-116">Выберите **Разрешать расчет по умолчанию** при переходе с Microsoft Dynamics NAV 5.0 или ранее.</span><span class="sxs-lookup"><span data-stu-id="af9c1-116">Select **Allow Default Calculation** if you are migrating from Microsoft Dynamics NAV 5.0 or earlier.</span></span>|<span data-ttu-id="af9c1-117">Используйте, только если нужно разрешить всем или некоторым товарам переполнять точку дозаказа.</span><span class="sxs-lookup"><span data-stu-id="af9c1-117">Use only if you want to allow all or some of your items to overflow the reorder point.</span></span>|  
|<span data-ttu-id="af9c1-118">Буферный период по умолчанию</span><span class="sxs-lookup"><span data-stu-id="af9c1-118">Default Dampener Period</span></span>|<span data-ttu-id="af9c1-119">Выберите значение между 1D и 5D.</span><span class="sxs-lookup"><span data-stu-id="af9c1-119">Set between 1D and 5D.</span></span><br /><br /> <span data-ttu-id="af9c1-120">Если вы впервые выполняете планирование в [!INCLUDE[prod_short](includes/prod_short.md)], укажите больший период.</span><span class="sxs-lookup"><span data-stu-id="af9c1-120">If new to planning in [!INCLUDE[prod_short](includes/prod_short.md)], then set a longer period.</span></span>|<span data-ttu-id="af9c1-121">Если пользователи лучше знакомы с различными причинами отображения сообщений о действиях, сократите буферный период, чтобы разрешить дополнительные предложения об изменениях.</span><span class="sxs-lookup"><span data-stu-id="af9c1-121">When users are more familiar with the different reasons for action messages, then shorten the dampener period to allow more change suggestions.</span></span>|  
|<span data-ttu-id="af9c1-122">Буферное количество по умолчанию в %</span><span class="sxs-lookup"><span data-stu-id="af9c1-122">Default Dampener Quantity %</span></span>|<span data-ttu-id="af9c1-123">Установите значение между 5 и 20 процентами от размера партии данного товара.</span><span class="sxs-lookup"><span data-stu-id="af9c1-123">Set between 5 and 20 percent of the item’s lot size.</span></span>||  

## <a name="see-also"></a><span data-ttu-id="af9c1-124">См. также</span><span class="sxs-lookup"><span data-stu-id="af9c1-124">See Also</span></span>  
 <span data-ttu-id="af9c1-125">[Рекомендации по настройке. Планирование поставок](setup-best-practices-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="af9c1-125">[Setup Best Practices: Supply Planning](setup-best-practices-supply-planning.md) </span></span>  
 <span data-ttu-id="af9c1-126">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="af9c1-126">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
 [<span data-ttu-id="af9c1-127">Настройка сложных областей приложения с помощью рекомендаций</span><span class="sxs-lookup"><span data-stu-id="af9c1-127">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)  
 <span data-ttu-id="af9c1-128">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="af9c1-128">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]