---
title: "Управление себестоимостью товаров | Документы Майкрософт"
description: "Процесс управления затратами, который также называют учетом себестоимости, связан с записью и отчетностью по текущим бизнес-расходам. Он включает в себя отчетность по себестоимости производства и запасов, то есть, по себестоимости товаров."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8da779426dfd06519507796c995adcedcd40ac81
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="managing-inventory-costs"></a><span data-ttu-id="ddaf7-104">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="ddaf7-104">Managing Inventory Costs</span></span>
<span data-ttu-id="ddaf7-105">Процесс управления затратами, который также называют учетом себестоимости, связан с записью и отчетностью по текущим бизнес-расходам.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-105">Cost management, also referred to as “costing”, is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="ddaf7-106">Он включает в себя отчетность по себестоимости производства и запасов, то есть, по себестоимости товаров.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>   

<span data-ttu-id="ddaf7-107">Необходимо понять такие главные принципы: от выбора метода учета себестоимости зависит, как определяется стоимость товаров, когда они покидают склад; в результате коррекции стоимости стоимость проданных товаров обновляется связанной стоимостью покупки, учтенной после продажи; стоимость товаров должна учитываться в соответствующих счетах ГК через равные интервалы.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>

<span data-ttu-id="ddaf7-108">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="ddaf7-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="ddaf7-109">**To**</span></span>|<span data-ttu-id="ddaf7-110">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="ddaf7-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="ddaf7-111">Ознакомление с разнообразными концептуальными сведениями, необходимыми для понимания принципов и определений, управляющих функцией учета стоимости запасов в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="ddaf7-111">Read various conceptual information to understand the principles and definitions that govern the inventory costing accounting functionality in [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)].</span></span>|[<span data-ttu-id="ddaf7-112">Об оценке себестоимости товаров</span><span class="sxs-lookup"><span data-stu-id="ddaf7-112">About Inventory Costing</span></span>](finance-learn-about-costing.md)|  
|<span data-ttu-id="ddaf7-113">Настройка периодов учета запасов, методов учета себестоимости и методов округления.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-113">Set up inventory periods, costing methods, and rounding methods.</span></span>|[<span data-ttu-id="ddaf7-114">Настройка оценки стоимости запасов и учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="ddaf7-114">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)|
|<span data-ttu-id="ddaf7-115">Повышение или понижение стоимости одного или нескольких товаров в запасах путем учета текущей вычисленной стоимости.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-115">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="ddaf7-116">Практическое руководство. Переоценка запасов</span><span class="sxs-lookup"><span data-stu-id="ddaf7-116">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="ddaf7-117">Скорректируйте себестоимость товаров, автоматически или вручную, чтобы перенести изменения себестоимости из входящих операций на соответствующие исходящие операции.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-117">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="ddaf7-118">Практическое руководство. Корректировка себестоимости товаров</span><span class="sxs-lookup"><span data-stu-id="ddaf7-118">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="ddaf7-119">Используйте специальные функции себестоимости для повседневных транзакций в операциях с товарами.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-119">Use special costing functions for every-day item transactions in the item operations.</span></span>|[<span data-ttu-id="ddaf7-120">Обработка запасов и себестоимость производства</span><span class="sxs-lookup"><span data-stu-id="ddaf7-120">Handling Inventory and Manufacturing Costs</span></span>](finance-handle-inventory-and-manufacturing-costs.md)|  
|<span data-ttu-id="ddaf7-121">Периодическое обновление стандартных затрат для компонентов в спецификациях сборки или производства и развертывание новых затрат вплоть до родительского товара.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-121">Periodically update the standard costs of components, in assembly or production BOMs, and roll the new costs up to the parent item.</span></span>|[<span data-ttu-id="ddaf7-122">Практическое руководство: обновление стандартных себестоимостей</span><span class="sxs-lookup"><span data-stu-id="ddaf7-122">How to: Update Standard Costs</span></span>](finance-how-to-update-standard-costs.md)|
|<span data-ttu-id="ddaf7-123">Выполнение задач управления завершением периода и задач отчетности, таких как расчет стоимости запасов и учет себестоимости в главной книге.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-123">Perform period-end control and reporting tasks, such calculate the value of inventory and post costs to the general ledger.</span></span>|[<span data-ttu-id="ddaf7-124">Отчет о затратах и выверка с главной книгой</span><span class="sxs-lookup"><span data-stu-id="ddaf7-124">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="ddaf7-125">Узнайте о всех механизмах в системе расчета себестоимости.</span><span class="sxs-lookup"><span data-stu-id="ddaf7-125">Learn about all mechanisms in the costing system.</span></span>|[<span data-ttu-id="ddaf7-126">Сведения о проектировании: себестоимость запасов</span><span class="sxs-lookup"><span data-stu-id="ddaf7-126">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|  

## <a name="see-also"></a><span data-ttu-id="ddaf7-127">См. также</span><span class="sxs-lookup"><span data-stu-id="ddaf7-127">See Also</span></span>  
 [<span data-ttu-id="ddaf7-128">Финансы</span><span class="sxs-lookup"><span data-stu-id="ddaf7-128">Finance</span></span>](finance.md)  
 <span data-ttu-id="ddaf7-129">[Наличие](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="ddaf7-129">[Inventory](inventory-manage-inventory.md) </span></span>  
 <span data-ttu-id="ddaf7-130">[Продажи](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="ddaf7-130">[Sales](sales-manage-sales.md) </span></span>  
 [<span data-ttu-id="ddaf7-131">Покупки</span><span class="sxs-lookup"><span data-stu-id="ddaf7-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="ddaf7-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ddaf7-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

