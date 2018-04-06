---
title: "Сведения о проектировании — партия на партию | Документы Майкрософт"
description: "Узнайте, как использовать политику \"партия на партию\" для того, чтобы определять количество заказа на основе спроса."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 2e0d1d18685f3395c31071ca9a2495c0091c564d
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-lot-for-lot"></a><span data-ttu-id="d2c87-103">Сведения о проектировании: партия на партию</span><span class="sxs-lookup"><span data-stu-id="d2c87-103">Design Details: Lot-for-Lot</span></span>
<span data-ttu-id="d2c87-104">Политика работы с индивидуальными партиями является наиболее гибкой, потому что система реагирует только на фактический спрос, а также на предполагаемый спрос прогнозируемых и общих заказов, а затем сопоставляет количество заказа с учетом спроса.</span><span class="sxs-lookup"><span data-stu-id="d2c87-104">The lot-for-lot policy is the most flexible because the system only reacts on actual demand, plus it acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand.</span></span> <span data-ttu-id="d2c87-105">Политика обработки отдельных партий ориентирована на товары категории А и В, где запасы могут быть приняты, однако этого следует избегать.</span><span class="sxs-lookup"><span data-stu-id="d2c87-105">The lot-for-lot policy is aimed at A- and B-items where inventory can be accepted but should be avoided.</span></span>  
  
<span data-ttu-id="d2c87-106">В некоторой степени политика "Партия на партию" похожа на политику "Заказ", но имеет общий подход к товарам. В соответствии с ней можно принимать количества в запасах и связывать спрос с соответствующей поставкой в горизонтах планирования, определенных пользователем.</span><span class="sxs-lookup"><span data-stu-id="d2c87-106">In some ways, the lot-for-lot policy looks like the Order policy, but it has a generic approach to items; it can accept quantities in inventory, and it bundles demand and corresponding supply in time buckets defined by the user.</span></span>  
  
<span data-ttu-id="d2c87-107">Горизонт планирования определяется в поле **Горизонт планирования**.</span><span class="sxs-lookup"><span data-stu-id="d2c87-107">The time bucket is defined in the **Time Bucket** field.</span></span> <span data-ttu-id="d2c87-108">Система работает с минимальным горизонтом планирования 1 день, поскольку это минимальная единица измерения событий спроса и предложения в системе (хотя на практике единица измерения производственных заказов и потребности в компонентах может измеряться в секундах).</span><span class="sxs-lookup"><span data-stu-id="d2c87-108">The system works with a minimum time bucket of one day, since this is the smallest time unit of measure on demand and supply events in the system (although, in practice, the time unit of measure on production orders and component needs can be seconds).</span></span>  
  
<span data-ttu-id="d2c87-109">Горизонт планирования также устанавливает лимиты перепланирования существующего заказа на поставку с целью удовлетворения имеющегося требования.</span><span class="sxs-lookup"><span data-stu-id="d2c87-109">The time bucket also sets limits on when an existing supply order should be rescheduled to meet a given demand.</span></span> <span data-ttu-id="d2c87-110">Если поставка находится в пределах горизонта планирования, она будет перепланирована на более раннюю или позднюю дату, чтобы удовлетворить спрос.</span><span class="sxs-lookup"><span data-stu-id="d2c87-110">If the supply lies within the time bucket, it will be rescheduled in or out to meet the demand.</span></span> <span data-ttu-id="d2c87-111">В противном, если поставка находится до горизонта планирования, это приведет к ненужному накоплению запасов, и такую поставку следует отменить.</span><span class="sxs-lookup"><span data-stu-id="d2c87-111">Otherwise, if it lies earlier, it will cause unnecessary build-up of inventory and should be canceled.</span></span> <span data-ttu-id="d2c87-112">В противном случае будет создан новый заказ на поставку.</span><span class="sxs-lookup"><span data-stu-id="d2c87-112">If it lies later, a new supply order will be created instead.</span></span>  
  
<span data-ttu-id="d2c87-113">С этой политикой можно также определить страховой запас, чтобы компенсировать возможные колебания в поставках или удовлетворить неожиданный спрос.</span><span class="sxs-lookup"><span data-stu-id="d2c87-113">With this policy, it is also possible to define a safety stock in order to compensate for possible fluctuations in supply, or to meet sudden demand.</span></span>  
  
<span data-ttu-id="d2c87-114">Поскольку количество заказа на поставку основывается на фактическом спросе, может иметь смысл использовать модификаторы заказов: округление количества заказа с учетом указанного множителя заказа (или единицы измерения покупки), увеличение количества заказа до определенного минимального значения или уменьшение количества до определенного максимального значения (при этом создается две или больше поставок для достижения необходимого количества).</span><span class="sxs-lookup"><span data-stu-id="d2c87-114">Because the supply order quantity is based on the actual demand it can make sense to use the order modifiers: round the order quantity up to meet a specified order multiple (or purchase unit of measure), increase the order to a specified minimum order quantity, or decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d2c87-115">См. также</span><span class="sxs-lookup"><span data-stu-id="d2c87-115">See Also</span></span>  
<span data-ttu-id="d2c87-116">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d2c87-116">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="d2c87-117">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="d2c87-117">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="d2c87-118">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="d2c87-118">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="d2c87-119">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="d2c87-119">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
