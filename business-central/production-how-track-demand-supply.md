---
title: Как отслеживать связи между спросом и предложением | Документы Майкрософт
description: Из любого документа по предложению или спросу в так называемой сети заказов можно отслеживать требования по заказу (трассируемое количество), прогноз, общий заказ продажи или параметры планирования (нетрассируемое количество), ставших причиной создания соответствующей строки планирования.
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
ms.openlocfilehash: beb438be379cfc6e3f239ebb0ae270a2e957651c
ms.sourcegitcommit: addfb47612cc2e4e98dfd7e338b6f41cde405d5c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2019
ms.locfileid: "938494"
---
# <a name="track-relations-between-demand-and-supply"></a><span data-ttu-id="aa80e-103">Отслеживание связей между спросом и предложением</span><span class="sxs-lookup"><span data-stu-id="aa80e-103">Track Relations Between Demand and Supply</span></span>
<span data-ttu-id="aa80e-104">Из любого документа по предложению или спросу в так называемой сети заказов можно отслеживать требования по заказу (трассируемое количество), прогноз, общий заказ продажи или параметры планирования (нетрассируемое количество), ставших причиной создания соответствующей строки планирования.</span><span class="sxs-lookup"><span data-stu-id="aa80e-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span></span>

<span data-ttu-id="aa80e-105">В производственных планах также предлагаются такие вспомогательные сведения о планировании, как не связанные с заказом операции, помогающие планировщику составить оптимальный план поставки.</span><span class="sxs-lookup"><span data-stu-id="aa80e-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span></span> <span data-ttu-id="aa80e-106">Дополнительные сведения см. в разделе [Нетрассируемые элементы планирования](production-how-track-demand-supply.md#untracked-planning-elements).</span><span class="sxs-lookup"><span data-stu-id="aa80e-106">For more information, see [Untracked Planning Elements](production-how-track-demand-supply.md#untracked-planning-elements).</span></span>

## <a name="to-track-linked-items"></a><span data-ttu-id="aa80e-107">Трассировка связанных товаров</span><span class="sxs-lookup"><span data-stu-id="aa80e-107">To track linked items</span></span>
<span data-ttu-id="aa80e-108">Трассировка заказов отображает, как при помощи резервирования заказы продаж, производственные заказы и заказы покупки соотносятся с производственным заказом в системах планирования и резервирования.</span><span class="sxs-lookup"><span data-stu-id="aa80e-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span></span>

<span data-ttu-id="aa80e-109">Ниже описано, как отслеживать связанные товары в утвержденном производственном заказе.</span><span class="sxs-lookup"><span data-stu-id="aa80e-109">The following describes how to track linked items on a firm planned production order.</span></span> <span data-ttu-id="aa80e-110">Шаги аналогичны для всех типов заказов, а также из строк журнала планирования.</span><span class="sxs-lookup"><span data-stu-id="aa80e-110">The steps are similar for all other order types, and from planning worksheet lines.</span></span>

1. <span data-ttu-id="aa80e-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Утвержд. произ. заказ**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="aa80e-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="aa80e-112">Откройте соответствующий утвержденный производственный заказ из списка.</span><span class="sxs-lookup"><span data-stu-id="aa80e-112">Open the relevant firm planned production order from the list.</span></span>
3. <span data-ttu-id="aa80e-113">На экспресс-вкладке **Строки** выберите действие **Функции**, затем действие **Трассировка заказа**.</span><span class="sxs-lookup"><span data-stu-id="aa80e-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span></span>

<span data-ttu-id="aa80e-114">В окне **Трассировка заказов** перечислены документы, которые имеют отношение к текущей строке производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="aa80e-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span></span>

## <a name="untracked-planning-elements"></a><span data-ttu-id="aa80e-115">Нетрассируемые элементы планирования</span><span class="sxs-lookup"><span data-stu-id="aa80e-115">Untracked Planning Elements</span></span>
<span data-ttu-id="aa80e-116">Страница **Нетрассируемые элементы планирования** открывается при выборе поля **Нетрассированное колич.** на странице **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="aa80e-116">The **Untracked Planning Elements** page opens when you choose the **Untracked Qty.** field on the **order Planning** page.</span></span> <span data-ttu-id="aa80e-117">Оно служит для двух целей:</span><span class="sxs-lookup"><span data-stu-id="aa80e-117">It serves two purposes:</span></span>

1. <span data-ttu-id="aa80e-118">для хранения сведений о нетрассированных количествах, которые отображаются, когда пользователь выполняет поиск со страницы «Трассировка заказов», чтобы просмотреть нетрассированные количества;</span><span class="sxs-lookup"><span data-stu-id="aa80e-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking page to see untracked quantities.</span></span>
2. <span data-ttu-id="aa80e-119">для хранения предупреждений, которые отображаются, когда пользователь выбирает значок **Предупреждение** на странице **Журнал планирования**.</span><span class="sxs-lookup"><span data-stu-id="aa80e-119">To hold warning messages displayed when the user chooses the **Warning** icon on the **Planning Worksheet** page.</span></span>

<span data-ttu-id="aa80e-120">Страница содержит записи для учета нетрассированного избыточного количества в сети трассировки заказов.</span><span class="sxs-lookup"><span data-stu-id="aa80e-120">The page contains entries which account for an untracked surplus quantity in order tracking network.</span></span> <span data-ttu-id="aa80e-121">Эти записи создаются в ходе планирования и поясняют, откуда появилось нетрассированное избыточное количество в строке трассировки заказов.</span><span class="sxs-lookup"><span data-stu-id="aa80e-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span></span> <span data-ttu-id="aa80e-122">Этот нетрассированный излишек может появляться из следующих источников:</span><span class="sxs-lookup"><span data-stu-id="aa80e-122">This untracked surplus can come from:</span></span>

- <span data-ttu-id="aa80e-123">«Прогноз производства»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-123">Production forecast</span></span>
- <span data-ttu-id="aa80e-124">«Общие заказы»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-124">Blanket orders</span></span>
- <span data-ttu-id="aa80e-125">«Кол-во страхового запаса»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-125">Safety stock quantity</span></span>
- <span data-ttu-id="aa80e-126">«Точка повтора заказа»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-126">Reorder point</span></span>
- <span data-ttu-id="aa80e-127">«Максимальный запас»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-127">Maximum inventory</span></span>
- <span data-ttu-id="aa80e-128">«Кол-во для повторного заказа»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-128">Reorder quantity</span></span>
- <span data-ttu-id="aa80e-129">«Максимальное кол-во заказа»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-129">Maximum order quantity</span></span>
- <span data-ttu-id="aa80e-130">«Минимальное кол-во заказа»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-130">Minimum order quantity</span></span>
- <span data-ttu-id="aa80e-131">«Заказать несколько»;</span><span class="sxs-lookup"><span data-stu-id="aa80e-131">Order multiple</span></span>
- <span data-ttu-id="aa80e-132">«Демпфер (% от размера партии)».</span><span class="sxs-lookup"><span data-stu-id="aa80e-132">Dampener (% of lot size)</span></span>

## <a name="see-also"></a><span data-ttu-id="aa80e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="aa80e-133">See Also</span></span>  
<span data-ttu-id="aa80e-134">[Планирование](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="aa80e-134">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="aa80e-135">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="aa80e-135">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="aa80e-136">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="aa80e-136">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="aa80e-137">Наличие</span><span class="sxs-lookup"><span data-stu-id="aa80e-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="aa80e-138">Покупки</span><span class="sxs-lookup"><span data-stu-id="aa80e-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="aa80e-139">Сведения о проектировании. Резервирование, трассировка и отправка сообщений о действиях</span><span class="sxs-lookup"><span data-stu-id="aa80e-139">Design Details: Reservation, Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="aa80e-140">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="aa80e-140">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="aa80e-141">Рекомендации по настройке. Планирование поставок</span><span class="sxs-lookup"><span data-stu-id="aa80e-141">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="aa80e-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aa80e-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
