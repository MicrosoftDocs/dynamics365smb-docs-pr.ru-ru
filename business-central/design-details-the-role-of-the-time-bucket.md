---
title: "Сведения о проектировании — роль горизонта планирования | Документы Майкрософт"
description: "Цель горизонта планирования — сбор событий спроса в окне времени с целью составления совместного заказа на поставку."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 099465f0ef7bdafa3df80c377cd83b177bb68072
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-the-role-of-the-time-bucket"></a><span data-ttu-id="f9e3e-103">Сведения о проектировании: роль горизонта планирования</span><span class="sxs-lookup"><span data-stu-id="f9e3e-103">Design Details: The Role of the Time Bucket</span></span>
<span data-ttu-id="f9e3e-104">Цель горизонта планирования — сбор событий спроса в окне времени с целью составления совместного заказа на поставку.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-104">The purpose of the time bucket is to collect demand events within the time window in order to make a joint supply order.</span></span>  
  
 <span data-ttu-id="f9e3e-105">Для политик дозаказа, в которых используется точка дозаказа, можно определить горизонт планирования.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-105">For reordering policies that use a reorder point, you can define a time bucket.</span></span> <span data-ttu-id="f9e3e-106">Это обеспечивает аккумуляцию спроса в одном временном периоде до проверки влияния на прогнозируемые запасы и проверки прохождения точки повторного заказа.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-106">This ensures that demand within the same time period is accumulated before checking the impact on the projected inventory and whether the reorder point has been passed.</span></span> <span data-ttu-id="f9e3e-107">Если точка дозаказа пройдена, планируется новый заказ на поставку на дату после даты конца периода, указанного в горизонте планирования.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-107">If the reorder point is passed, a new supply order is scheduled forward from the end of the period defined by the time bucket.</span></span> <span data-ttu-id="f9e3e-108">Горизонты планирования начинаются в начальную дату планирования.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-108">The time buckets begin on the planning starting date.</span></span>  
  
 <span data-ttu-id="f9e3e-109">Концепция горизонтов планирования отражает осуществляемый вручную процесс проверки уровня запасов на регулярной основе, а не для каждой транзакции.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-109">The time-bucketed concept reflects the manual process of checking the inventory level on a frequent basis rather than for each transaction.</span></span> <span data-ttu-id="f9e3e-110">Пользователю требуется определить периодичность (горизонт планирования).</span><span class="sxs-lookup"><span data-stu-id="f9e3e-110">The user needs to define the frequency (the time bucket).</span></span> <span data-ttu-id="f9e3e-111">Например, пользователь объединяет все потребности в товарах для одного поставщика для размещения еженедельного заказа.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-111">For example, the user gathers all item needs from one vendor to place a weekly order.</span></span>  
  
 <span data-ttu-id="f9e3e-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span><span class="sxs-lookup"><span data-stu-id="f9e3e-112">![](media/nav_app_supply_planning_2_reorder_cycle.png "NAV_APP_supply_planning_2_reorder_cycle")</span></span>  
  
 <span data-ttu-id="f9e3e-113">Горизонт планирования, как правило, используется для того, чтобы избежать каскадного эффекта.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-113">The time bucket is generally used to avoid a cascade effect.</span></span> <span data-ttu-id="f9e3e-114">Например, создается сбалансированная строка спроса и поставки, в которой отменяется преждевременный спрос.</span><span class="sxs-lookup"><span data-stu-id="f9e3e-114">For example, a balanced row of demand and supply where an early demand is canceled, or a new one is created.</span></span> <span data-ttu-id="f9e3e-115">Результатом будет перепланирование всех заказов на поставку (кроме последнего).</span><span class="sxs-lookup"><span data-stu-id="f9e3e-115">The result would be that every supply order (except the last one) is rescheduled.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f9e3e-116">См. также</span><span class="sxs-lookup"><span data-stu-id="f9e3e-116">See Also</span></span>  
 <span data-ttu-id="f9e3e-117">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="f9e3e-117">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
 <span data-ttu-id="f9e3e-118">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="f9e3e-118">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
 <span data-ttu-id="f9e3e-119">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="f9e3e-119">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
 [<span data-ttu-id="f9e3e-120">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="f9e3e-120">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
