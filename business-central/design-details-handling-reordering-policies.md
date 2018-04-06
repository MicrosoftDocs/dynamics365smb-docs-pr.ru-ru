---
title: "Сведения о проектировании — обработка политик дозаказа | Документы Майкрософт"
description: "Обзор задач для определения политики повтора заказа при планировании поставок."
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
ms.openlocfilehash: b273dedd269d8b86ba4fa7a9d9540c44b701a97e
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-handling-reordering-policies"></a><span data-ttu-id="9004d-103">Сведения о проектировании: обработка политик дозаказа</span><span class="sxs-lookup"><span data-stu-id="9004d-103">Design Details: Handling Reordering Policies</span></span>
<span data-ttu-id="9004d-104">Чтобы товар мог участвовать в планировании поставок, должна быть определена политика дозаказа.</span><span class="sxs-lookup"><span data-stu-id="9004d-104">For an item to participate in supply planning, a reorder policy must be defined.</span></span> <span data-ttu-id="9004d-105">Существует четыре следующих политики повторного заказа.</span><span class="sxs-lookup"><span data-stu-id="9004d-105">The following four reordering policies exist:</span></span>  
  
* <span data-ttu-id="9004d-106">Фикс. кол-во повтора заказа</span><span class="sxs-lookup"><span data-stu-id="9004d-106">Fixed Reorder Qty.</span></span>  
* <span data-ttu-id="9004d-107">Максимальное кол-во</span><span class="sxs-lookup"><span data-stu-id="9004d-107">Maximum Qty.</span></span>  
* <span data-ttu-id="9004d-108">Заказ</span><span class="sxs-lookup"><span data-stu-id="9004d-108">Order</span></span>  
* <span data-ttu-id="9004d-109">Партия на партию</span><span class="sxs-lookup"><span data-stu-id="9004d-109">Lot-for-Lot</span></span>  
  
<span data-ttu-id="9004d-110">Политики "Фикс. кол-во дозаказа" и "Максимальное кол-во" относятся к планированию запасов.</span><span class="sxs-lookup"><span data-stu-id="9004d-110">Fixed Reorder Qty. and Maximum Qty. policies relate to inventory planning.</span></span> <span data-ttu-id="9004d-111">Хотя планирование запасов технически проще процедуры балансировки, эти политики должны сосуществовать с поэтапной балансировкой поставок и трассировкой заказов.</span><span class="sxs-lookup"><span data-stu-id="9004d-111">Although inventory planning is technically simpler than the balancing procedure, these policies must coexist with the step-by-step balancing of supply and order tracking.</span></span> <span data-ttu-id="9004d-112">Для контроля интеграции между этими двумя сущностями и обеспечения обзорности соответствующей логики планирования, строгие принципы регулируют работу с политиками повторных заказов.</span><span class="sxs-lookup"><span data-stu-id="9004d-112">To control the integration between the two, and to provide visibility into the involved planning logic, strict principles govern how reordering policies are handled.</span></span>  
  
## <a name="in-this-section"></a><span data-ttu-id="9004d-113">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="9004d-113">In This Section</span></span>  
[<span data-ttu-id="9004d-114">Сведения о проектировании: роль точки дозаказа</span><span class="sxs-lookup"><span data-stu-id="9004d-114">Design Details: The Role of the Reorder Point</span></span>](design-details-the-role-of-the-reorder-point.md)  
[<span data-ttu-id="9004d-115">Сведения о проектировании: отслеживание уровня прогнозируемых запасов и точки дозаказа</span><span class="sxs-lookup"><span data-stu-id="9004d-115">Design Details: Monitoring the Projected Inventory Level and the Reorder Point</span></span>](design-details-monitoring-the-projected-inventory-level-and-the-reorder-point.md)  
[<span data-ttu-id="9004d-116">Сведения о проектировании: роль горизонта планирования</span><span class="sxs-lookup"><span data-stu-id="9004d-116">Design Details: The Role of the Time Bucket</span></span>](design-details-the-role-of-the-time-bucket.md)  
[<span data-ttu-id="9004d-117">Сведения о проектировании: нахождение ниже уровня допустимого избытка</span><span class="sxs-lookup"><span data-stu-id="9004d-117">Design Details: Staying under the Overflow Level</span></span>](design-details-staying-under-the-overflow-level.md)  
[<span data-ttu-id="9004d-118">Сведения о проектировании: обработка прогнозируемых отрицательных остатков</span><span class="sxs-lookup"><span data-stu-id="9004d-118">Design Details: Handling Projected Negative Inventory</span></span>](design-details-handling-projected-negative-inventory.md)  
[<span data-ttu-id="9004d-119">Сведения о проектировании: политики дозаказа</span><span class="sxs-lookup"><span data-stu-id="9004d-119">Design Details: Reordering Policies</span></span>](design-details-reordering-policies.md)  
  
## <a name="see-also"></a><span data-ttu-id="9004d-120">См. также</span><span class="sxs-lookup"><span data-stu-id="9004d-120">See Also</span></span>  
<span data-ttu-id="9004d-121">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="9004d-121">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="9004d-122">[Сведения о проектировании: таблица "Назначение произ. плана"](design-details-planning-assignment-table.md) </span><span class="sxs-lookup"><span data-stu-id="9004d-122">[Design Details: Planning Assignment Table](design-details-planning-assignment-table.md) </span></span>  
<span data-ttu-id="9004d-123">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="9004d-123">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
<span data-ttu-id="9004d-124">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="9004d-124">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
[<span data-ttu-id="9004d-125">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="9004d-125">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
