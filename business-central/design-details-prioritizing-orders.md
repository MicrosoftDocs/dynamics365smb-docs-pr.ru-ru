---
title: "Сведения о проектировании — определение приоритета заказов | Документы Майкрософт"
description: "Узнайте, как задавать приоритеты для удовлетворения требований как спроса, так и предложения."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 6e09ad64750493f99210d47516410d8471a83011
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="d3dda-103">Сведения о проектировании: определение приоритета заказов</span><span class="sxs-lookup"><span data-stu-id="d3dda-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="d3dda-104">В пределах заданной единицы хранения запрошенная или доступная дата представляет наивысший приоритет; спрос сегодняшнего дня необходимо удовлетворить перед спросом следующей недели.</span><span class="sxs-lookup"><span data-stu-id="d3dda-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="d3dda-105">Но в дополнение к этому общему приоритету система планирования предложит тип спроса, который требуется удовлетворить до удовлетворения другого спроса.</span><span class="sxs-lookup"><span data-stu-id="d3dda-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="d3dda-106">Аналогично она укажет, какой источник поставки следует применить до применения других источников поставки.</span><span class="sxs-lookup"><span data-stu-id="d3dda-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="d3dda-107">Это осуществляется в соответствии с приоритетами заказов.</span><span class="sxs-lookup"><span data-stu-id="d3dda-107">This is done according to order priorities.</span></span>  
  
<span data-ttu-id="d3dda-108">Загруженный спрос и поставка влияют на профиль для прогнозируемых запасов в соответствии со следующими приоритетами:</span><span class="sxs-lookup"><span data-stu-id="d3dda-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  
  
## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="d3dda-109">Приоритеты на стороне спроса</span><span class="sxs-lookup"><span data-stu-id="d3dda-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="d3dda-110">Уже отгружено: операция книги товаров</span><span class="sxs-lookup"><span data-stu-id="d3dda-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="d3dda-111">Возврат покупки</span><span class="sxs-lookup"><span data-stu-id="d3dda-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="d3dda-112">Заказ на продажу</span><span class="sxs-lookup"><span data-stu-id="d3dda-112">Sales Order</span></span>  
4. <span data-ttu-id="d3dda-113">Сервисный заказ</span><span class="sxs-lookup"><span data-stu-id="d3dda-113">Service Order</span></span>  
5. <span data-ttu-id="d3dda-114">Требуемый производственный компонент</span><span class="sxs-lookup"><span data-stu-id="d3dda-114">Production Component Need</span></span>  
6. <span data-ttu-id="d3dda-115">Строка заказа на сборку</span><span class="sxs-lookup"><span data-stu-id="d3dda-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="d3dda-116">Заказ на исходящее перемещение</span><span class="sxs-lookup"><span data-stu-id="d3dda-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="d3dda-117">Общий заказ (еще не использованный в связанных заказах на продажу)</span><span class="sxs-lookup"><span data-stu-id="d3dda-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="d3dda-118">Прогноз (еще не использованный в других заказах на продажу)</span><span class="sxs-lookup"><span data-stu-id="d3dda-118">Forecast (that has not already been consumed by other sales orders)</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="d3dda-119">Возвраты покупок обычно не включаются в планирование поставок; они всегда должны резервироваться из партии, которая будет возвращена.</span><span class="sxs-lookup"><span data-stu-id="d3dda-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="d3dda-120">Если возвраты покупок не зарезервированы, они играют роль в наличии и имеют высокий приоритет, чтобы система планирования не предлагала заказ на поставку лишь для того, чтобы обслужить возврат покупки.</span><span class="sxs-lookup"><span data-stu-id="d3dda-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  
  
## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="d3dda-121">Приоритеты на стороне поставки</span><span class="sxs-lookup"><span data-stu-id="d3dda-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="d3dda-122">Уже существует на складе: операция книги товаров ("Гибкость планирования" = "Нет")</span><span class="sxs-lookup"><span data-stu-id="d3dda-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="d3dda-123">Возврат продажи ("Гибкость планирования" = "Нет")</span><span class="sxs-lookup"><span data-stu-id="d3dda-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="d3dda-124">Заказ на входящее перемещение</span><span class="sxs-lookup"><span data-stu-id="d3dda-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="d3dda-125">Производственный заказ</span><span class="sxs-lookup"><span data-stu-id="d3dda-125">Production Order</span></span>  
5. <span data-ttu-id="d3dda-126">Сборочный заказ</span><span class="sxs-lookup"><span data-stu-id="d3dda-126">Assembly Order</span></span>  
6. <span data-ttu-id="d3dda-127">Заказ на покупку</span><span class="sxs-lookup"><span data-stu-id="d3dda-127">Purchase Order</span></span>  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="d3dda-128">Приоритет, связанный с состоянием спрос и поставки</span><span class="sxs-lookup"><span data-stu-id="d3dda-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="d3dda-129">Помимо приоритетов, определяемых типом спроса и поставки, текущее состояние заказов в процессе выполнения также определяет приоритет.</span><span class="sxs-lookup"><span data-stu-id="d3dda-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="d3dda-130">Например, складские операции оказывают влияние, и учитывается статус заказов на продажу, покупку, перемещение и сборку:</span><span class="sxs-lookup"><span data-stu-id="d3dda-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  
  
1. <span data-ttu-id="d3dda-131">Частично скорректировано ("Гибкость планирования" = "Нет")</span><span class="sxs-lookup"><span data-stu-id="d3dda-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="d3dda-132">Уже обрабатывается на складе ("Гибкость планирования" = "Нет")</span><span class="sxs-lookup"><span data-stu-id="d3dda-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="d3dda-133">Выпущено — все типы заказов ("Гибкость планирования" = "Неограниченно")</span><span class="sxs-lookup"><span data-stu-id="d3dda-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="d3dda-134">Утвержденный производственный заказ ("Гибкость планирования" = "Неограниченно")</span><span class="sxs-lookup"><span data-stu-id="d3dda-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="d3dda-135">Запланировано/открыто — все типы заказов ("Гибкость планирования" = "Неограниченно")</span><span class="sxs-lookup"><span data-stu-id="d3dda-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="d3dda-136">См. также</span><span class="sxs-lookup"><span data-stu-id="d3dda-136">See Also</span></span>  
<span data-ttu-id="d3dda-137">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="d3dda-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="d3dda-138">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="d3dda-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="d3dda-139">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="d3dda-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
