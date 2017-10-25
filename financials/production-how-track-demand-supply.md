---
title: "Как отслеживать связи между спросом и предложением | Документы Майкрософт"
description: "Из любого документа по предложению или спросу в так называемой сети заказов можно отслеживать требования по заказу (трассируемое количество), прогноз, общий заказ продажи или параметры планирования (нетрассируемое количество), ставших причиной создания соответствующей строки планирования."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 511381e4f6d469ff16714a30fde60d3e238ad975
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-track-relations-between-demand-and-supply"></a><span data-ttu-id="97f62-103">Практическое руководство. Отслеживание связей между спросом и предложением</span><span class="sxs-lookup"><span data-stu-id="97f62-103">How to: Track Relations Between Demand and Supply</span></span>
<span data-ttu-id="97f62-104">Из любого документа по предложению или спросу в так называемой сети заказов можно отслеживать требования по заказу (трассируемое количество), прогноз, общий заказ продажи или параметры планирования (нетрассируемое количество), ставших причиной создания соответствующей строки планирования.</span><span class="sxs-lookup"><span data-stu-id="97f62-104">From any supply or demand document in the so-called order network, you can track the order demand (tracked quantity), forecast, blanket sales order, or planning parameter (untracked quantity) that has given rise to the planning line in question.</span></span>

<span data-ttu-id="97f62-105">В производственных планах также предлагаются такие вспомогательные сведения о планировании, как не связанные с заказом операции, помогающие планировщику составить оптимальный план поставки.</span><span class="sxs-lookup"><span data-stu-id="97f62-105">The planning worksheets also offers supporting planning information about non-order entities to help the planner obtain an optimal supply plan.</span></span> <span data-ttu-id="97f62-106">Дополнительные сведения см. в разделе "Нетрассируемые элементы планирования".</span><span class="sxs-lookup"><span data-stu-id="97f62-106">For more information, see the "Untracked Planning Elements" section.</span></span>

## <a name="to-track-linked-items"></a><span data-ttu-id="97f62-107">Трассировка связанных товаров</span><span class="sxs-lookup"><span data-stu-id="97f62-107">To track linked items</span></span>
<span data-ttu-id="97f62-108">Трассировка заказов отображает, как при помощи резервирования заказы продаж, производственные заказы и заказы покупки соотносятся с производственным заказом в системах планирования и резервирования.</span><span class="sxs-lookup"><span data-stu-id="97f62-108">Order tracking shows how sales orders, production orders, and purchase orders are related to the manufacturing order through the planning and reservation systems.</span></span>

<span data-ttu-id="97f62-109">Ниже описано, как отслеживать связанные товары в утвержденном производственном заказе.</span><span class="sxs-lookup"><span data-stu-id="97f62-109">The following describes how to track linked items on a firm planned production order.</span></span> <span data-ttu-id="97f62-110">Шаги аналогичны для всех типов заказов, а также из строк журнала планирования.</span><span class="sxs-lookup"><span data-stu-id="97f62-110">The steps are similar for all other order types, and from planning worksheet lines.</span></span>

1. <span data-ttu-id="97f62-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Утвержд. произ. заказ**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="97f62-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="97f62-112">Откройте соответствующий утвержденный производственный заказ из списка.</span><span class="sxs-lookup"><span data-stu-id="97f62-112">Open the relevant firm planned production order from the list.</span></span>
3. <span data-ttu-id="97f62-113">На экспресс-вкладке **Строки** выберите действие **Функции**, затем действие **Трассировка заказа**.</span><span class="sxs-lookup"><span data-stu-id="97f62-113">On the **Lines** FastTab, choose the **Functions** action, and then choose the **Order Tracking** action.</span></span>

<span data-ttu-id="97f62-114">В окне **Трассировка заказов** перечислены документы, которые имеют отношение к текущей строке производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="97f62-114">The lines in the **Order Tracking** display the documents that are related to the current production order line.</span></span>

## <a name="untracked-planning-elements"></a><span data-ttu-id="97f62-115">Нетрассируемые элементы планирования</span><span class="sxs-lookup"><span data-stu-id="97f62-115">Untracked Planning Elements</span></span>
<span data-ttu-id="97f62-116">Окно **Нетрассируемые элементы планирования** открывается при выборе поля **Нетрассированное колич.** в окне **Планирование заказов**.</span><span class="sxs-lookup"><span data-stu-id="97f62-116">The **Untracked Planning Elements** window opens when you choose the **Untracked Qty.** field in the **order Planning** window.</span></span> <span data-ttu-id="97f62-117">Оно служит для двух целей:</span><span class="sxs-lookup"><span data-stu-id="97f62-117">It serves two purposes:</span></span>

1. <span data-ttu-id="97f62-118">для хранения сведений о нетрассированных количествах, которые отображаются, когда пользователь выполняет поиск из окна «Трассировка заказов», чтобы просмотреть нетрассированные количества;</span><span class="sxs-lookup"><span data-stu-id="97f62-118">To hold information about untracked quantities displayed when the user looks up from the Order Tracking window to see untracked quantities.</span></span>
2. <span data-ttu-id="97f62-119">для хранения предупреждений, которые отображаются, когда пользователь выбирает значок **Предупреждение** в окне **Журнал планирования**.</span><span class="sxs-lookup"><span data-stu-id="97f62-119">To hold warning messages displayed when the user chooses the **Warning** icon in the **Planning Worksheet** window.</span></span>

<span data-ttu-id="97f62-120">Окно содержит записи для учета нетрассированного избыточного количества в сети трассировки заказов.</span><span class="sxs-lookup"><span data-stu-id="97f62-120">The window contains entries which account for an untracked surplus quantity in order tracking network.</span></span> <span data-ttu-id="97f62-121">Эти записи создаются в ходе планирования и поясняют, откуда появилось нетрассированное избыточное количество в строке трассировки заказов.</span><span class="sxs-lookup"><span data-stu-id="97f62-121">These entries are generated during the planning run and explain where the untracked surplus quantity in the order tracking lines came from.</span></span> <span data-ttu-id="97f62-122">Этот нетрассированный излишек может появляться из следующих источников:</span><span class="sxs-lookup"><span data-stu-id="97f62-122">This untracked surplus can come from:</span></span>

- <span data-ttu-id="97f62-123">«Прогноз производства»;</span><span class="sxs-lookup"><span data-stu-id="97f62-123">Production forecast</span></span>
- <span data-ttu-id="97f62-124">«Общие заказы»;</span><span class="sxs-lookup"><span data-stu-id="97f62-124">Blanket orders</span></span>
- <span data-ttu-id="97f62-125">«Кол-во страхового запаса»;</span><span class="sxs-lookup"><span data-stu-id="97f62-125">Safety stock quantity</span></span>
- <span data-ttu-id="97f62-126">«Точка повтора заказа»;</span><span class="sxs-lookup"><span data-stu-id="97f62-126">Reorder point</span></span>
- <span data-ttu-id="97f62-127">«Максимальный запас»;</span><span class="sxs-lookup"><span data-stu-id="97f62-127">Maximum inventory</span></span>
- <span data-ttu-id="97f62-128">«Кол-во для повторного заказа»;</span><span class="sxs-lookup"><span data-stu-id="97f62-128">Reorder quantity</span></span>
- <span data-ttu-id="97f62-129">«Максимальное кол-во заказа»;</span><span class="sxs-lookup"><span data-stu-id="97f62-129">Maximum order quantity</span></span>
- <span data-ttu-id="97f62-130">«Минимальное кол-во заказа»;</span><span class="sxs-lookup"><span data-stu-id="97f62-130">Minimum order quantity</span></span>
- <span data-ttu-id="97f62-131">«Заказать несколько»;</span><span class="sxs-lookup"><span data-stu-id="97f62-131">Order multiple</span></span>
- <span data-ttu-id="97f62-132">«Демпфер (% от размера партии)».</span><span class="sxs-lookup"><span data-stu-id="97f62-132">Dampener (% of lot size)</span></span>

## <a name="see-also"></a><span data-ttu-id="97f62-133">См. также</span><span class="sxs-lookup"><span data-stu-id="97f62-133">See Also</span></span>  
<span data-ttu-id="97f62-134">[Планирование](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="97f62-134">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="97f62-135">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="97f62-135">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="97f62-136">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="97f62-136">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="97f62-137">Наличие</span><span class="sxs-lookup"><span data-stu-id="97f62-137">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="97f62-138">Покупки</span><span class="sxs-lookup"><span data-stu-id="97f62-138">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="97f62-139">Сведения о проектировании. Резервирование, трассировка и отправка сообщений о действиях</span><span class="sxs-lookup"><span data-stu-id="97f62-139">Design Details: Reservation, Tracking, and Action Messaging</span></span>](design-details-reservation-order-tracking-and-action-messaging.md)  
<span data-ttu-id="97f62-140">[Сведения о проектировании: планирование поставок](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="97f62-140">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="97f62-141">Рекомендации по настройке. Планирование поставок</span><span class="sxs-lookup"><span data-stu-id="97f62-141">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="97f62-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="97f62-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

