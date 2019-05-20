---
title: Сведения о проектировании — роль горизонта планирования | Документы Майкрософт
description: Цель горизонта планирования — сбор событий спроса на странице времени с целью составления совместного заказа на поставку.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 54d4a4aed94b562b82d94d6a5a75a3050c054fc3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1239318"
---
# <a name="design-details-the-role-of-the-time-bucket"></a><span data-ttu-id="2a167-103">Сведения о проектировании: роль горизонта планирования</span><span class="sxs-lookup"><span data-stu-id="2a167-103">Design Details: The Role of the Time Bucket</span></span>
<span data-ttu-id="2a167-104">Цель горизонта планирования — сбор событий спроса на странице времени с целью составления совместного заказа на поставку.</span><span class="sxs-lookup"><span data-stu-id="2a167-104">The purpose of the time bucket is to collect demand events within the time page in order to make a joint supply order.</span></span>  

 <span data-ttu-id="2a167-105">Для политик дозаказа, в которых используется точка дозаказа, можно определить горизонт планирования.</span><span class="sxs-lookup"><span data-stu-id="2a167-105">For reordering policies that use a reorder point, you can define a time bucket.</span></span> <span data-ttu-id="2a167-106">Это обеспечивает аккумуляцию спроса в одном временном периоде до проверки влияния на прогнозируемые запасы и проверки прохождения точки повторного заказа.</span><span class="sxs-lookup"><span data-stu-id="2a167-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span></span> <span data-ttu-id="2a167-107">Если точка дозаказа пройдена, планируется новый заказ на поставку на дату после даты конца периода, указанного в горизонте планирования.</span><span class="sxs-lookup"><span data-stu-id="2a167-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span></span> <span data-ttu-id="2a167-108">Горизонты планирования начинаются в начальную дату планирования.</span><span class="sxs-lookup"><span data-stu-id="2a167-108">The time buckets begin on the planning starting date.</span></span>  

 <span data-ttu-id="2a167-109">Концепция горизонтов планирования отражает осуществляемый вручную процесс проверки уровня запасов на регулярной основе, а не для каждой транзакции.</span><span class="sxs-lookup"><span data-stu-id="2a167-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span></span> <span data-ttu-id="2a167-110">Пользователю требуется определить периодичность (горизонт планирования).</span><span class="sxs-lookup"><span data-stu-id="2a167-110">The user needs to define the frequency (the time bucket).</span></span> <span data-ttu-id="2a167-111">Например, пользователь объединяет все потребности в товарах для одного поставщика для размещения еженедельного заказа.</span><span class="sxs-lookup"><span data-stu-id="2a167-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span></span>  

 <span data-ttu-id="2a167-112">![Пример горизонта планирования](media/nav_app_supply_planning_2_reorder_cycle.png "Пример горизонта планирования")</span><span class="sxs-lookup"><span data-stu-id="2a167-112">![Example of time bucket in planning](media/nav_app_supply_planning_2_reorder_cycle.png "Example of time bucket in planning")</span></span>  

 <span data-ttu-id="2a167-113">Горизонт планирования, как правило, используется для того, чтобы избежать каскадного эффекта.</span><span class="sxs-lookup"><span data-stu-id="2a167-113">The time bucket is generally used to avoid a cascade effect.</span></span> <span data-ttu-id="2a167-114">Например, создается сбалансированная строка спроса и поставки, в которой отменяется преждевременный спрос.</span><span class="sxs-lookup"><span data-stu-id="2a167-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span></span> <span data-ttu-id="2a167-115">Результатом будет перепланирование всех заказов на поставку (кроме последнего).</span><span class="sxs-lookup"><span data-stu-id="2a167-115">The result would be that every supply order (except the last one) is rescheduled.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2a167-116">См. также</span><span class="sxs-lookup"><span data-stu-id="2a167-116">See Also</span></span>  
 <span data-ttu-id="2a167-117">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="2a167-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="2a167-118">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="2a167-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="2a167-119">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="2a167-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="2a167-120">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="2a167-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
