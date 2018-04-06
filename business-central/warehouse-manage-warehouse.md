---
title: "Складские операции | Документы Майкрософт"
description: "После получения товаров и перед их отгрузкой выполняется ряд внутренних складских действий, чтобы обеспечить эффективный поток через склад, а также упорядочить и обработать складские запасы организации."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 604f7e55067efaebed412683ed51ce8717562688
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="warehouse-management"></a><span data-ttu-id="9b123-103">Управление складом</span><span class="sxs-lookup"><span data-stu-id="9b123-103">Warehouse Management</span></span>
<span data-ttu-id="9b123-104">После получения товаров и перед их отгрузкой выполняется ряд внутренних складских действий, чтобы обеспечить эффективный поток через склад, а также упорядочить и обработать складские запасы организации.</span><span class="sxs-lookup"><span data-stu-id="9b123-104">After goods are received and before goods are shipped, a series of internal warehouse activities take place to ensure an effective flow through the warehouse and to organize and maintain company inventories.</span></span>

<span data-ttu-id="9b123-105">Типичные складские действия включают размещение товаров, перемещение товаров в пределах склада и между складами, а также подбор товаров для сборки, производства или отгрузки.</span><span class="sxs-lookup"><span data-stu-id="9b123-105">Typical warehouse activities include putting items away, moving items inside or between warehouses, and picking items for assembly, production, or shipment.</span></span> <span data-ttu-id="9b123-106">Сборка товаров для продажи или в запасы также может рассматриваться как складские операции, но здесь они не рассматриваются.</span><span class="sxs-lookup"><span data-stu-id="9b123-106">Assembling items for sale or inventory may also be considered warehouse activities, but these are covered elsewhere.</span></span> <span data-ttu-id="9b123-107">Дополнительные сведения см. в разделе [Управление сборкой](assembly-assemble-items.md).</span><span class="sxs-lookup"><span data-stu-id="9b123-107">For more information, see [Assembly Management](assembly-assemble-items.md).</span></span>  

<span data-ttu-id="9b123-108">На крупных складах эти различные задачи обработки могут распределяться по отделам, а управление их интеграцией осуществляется с помощью расширенного рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="9b123-108">In large warehouses, these different handling tasks can be separated by departments and the integration managed by a directed workflow.</span></span> <span data-ttu-id="9b123-109">В более простых структурах процесс менее формализован, а складские операции выполняются с использованием т. н. операций размещения запасов и подбора запасов.</span><span class="sxs-lookup"><span data-stu-id="9b123-109">In simpler installations, the flow is less formalized and the warehouse activities are performed with so-called inventory put-aways and inventory picks.</span></span> <span data-ttu-id="9b123-110">Дополнительные сведения о сравнении базовых и расширенных конфигурациях складов см. в разделах [Сведения о проектировании: обзор склада](design-details-warehouse-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9b123-110">For more information about basic versus advanced warehouse configurations, see [Design Details: Warehouse Overview](design-details-warehouse-overview.md).</span></span>

<span data-ttu-id="9b123-111">Прежде чем можно будет осуществлять складские операции, необходимо настроить систему для соответствующей сложности складской обработки.</span><span class="sxs-lookup"><span data-stu-id="9b123-111">Before you can perform warehouse activities, you must set the system up for the relevant complexity of warehouse processing.</span></span> <span data-ttu-id="9b123-112">Дополнительные сведения см. в разделе [Настройка управления складом](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="9b123-112">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>

 <span data-ttu-id="9b123-113">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="9b123-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="9b123-114">**Задача**</span><span class="sxs-lookup"><span data-stu-id="9b123-114">**To**</span></span>|<span data-ttu-id="9b123-115">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="9b123-115">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="9b123-116">Регистрация приемки товаров на складе, либо только с заказом на покупку, при простых настройках склада, либо со складской приходной накладной, в случае полуавтоматической или полностью автоматической обработки на складе.</span><span class="sxs-lookup"><span data-stu-id="9b123-116">Record the receipt of items at warehouse locations, either with a purchase order only, in simple location setups, or with a warehouse receipt, in case of semi or fully automated warehouse processing at the location.</span></span>|[<span data-ttu-id="9b123-117">Приемка товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-117">Receive Items</span></span>](warehouse-how-receive-items.md)|
|<span data-ttu-id="9b123-118">Обход процессов размещения и подборки, чтобы ускорить передачу товара прямо с приемки или производства на отгрузку.</span><span class="sxs-lookup"><span data-stu-id="9b123-118">Bypass the put-away and pick processes to expedite an item straight from receiving or production to shipping.</span></span>|[<span data-ttu-id="9b123-119">Переброска товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-119">Cross-Dock Items</span></span>](warehouse-how-to-cross-dock-items.md)|    
|<span data-ttu-id="9b123-120">Разместить товары, полученные в результате покупок, возвратов продаж, перемещений или выхода продукции в соответствии с настроенным процессом склада.</span><span class="sxs-lookup"><span data-stu-id="9b123-120">Put away items received from purchases, sales returns, transfers, or production output according to the configured warehouse process.</span></span>|[<span data-ttu-id="9b123-121">Размещение товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-121">Putting Items Away</span></span>](warehouse-put-away-items.md)|
|<span data-ttu-id="9b123-122">Перемещение товаров между ячейками на складе.</span><span class="sxs-lookup"><span data-stu-id="9b123-122">Move items between bins in the warehouse.</span></span>|[<span data-ttu-id="9b123-123">Перемещение товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-123">Moving Items</span></span>](warehouse-move-items.md)|
|<span data-ttu-id="9b123-124">Выполнить подбор товаров для отгрузки, перемещения или потребления при сборке или производстве в соответствии с настроенным процессом склада.</span><span class="sxs-lookup"><span data-stu-id="9b123-124">Pick items to be shipped, transferred, or consumed in assembly or production, according to the configured warehouse process.</span></span>|[<span data-ttu-id="9b123-125">Подбор товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-125">Picking Items</span></span>](warehouse-pick-items.md)|
|<span data-ttu-id="9b123-126">Регистрация отгрузки товаров со склада, либо только с заказом на продажу, при простых настройках склада, либо со складской расходной накладной, в случае полуавтоматических или полностью автоматических складских процессов на складе.</span><span class="sxs-lookup"><span data-stu-id="9b123-126">Record the shipment of items from warehouse locations, either with a sales order only, in simple location setups, or with a warehouse shipment, in case of semi or fully automated warehouse processes at the location.</span></span>|[<span data-ttu-id="9b123-127">Отгрузка товаров</span><span class="sxs-lookup"><span data-stu-id="9b123-127">Ship Items</span></span>](warehouse-how-ship-items.md)|  

## <a name="see-also"></a><span data-ttu-id="9b123-128">См. также</span><span class="sxs-lookup"><span data-stu-id="9b123-128">See Also</span></span>  
[<span data-ttu-id="9b123-129">Наличие</span><span class="sxs-lookup"><span data-stu-id="9b123-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="9b123-130">[Настройка управления складом](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="9b123-130">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="9b123-131">[Управление сборкой](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="9b123-131">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="9b123-132">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="9b123-132">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="9b123-133">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9b123-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]

