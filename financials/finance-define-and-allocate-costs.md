---
title: "Определение и распределение затрат | Документы Майкрософт"
description: "Распределения затрат перемещают затраты и доходы между типами затрат, местами возникновения затрат и объектами затрат. Можно определить любое необходимое число распределений."
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
ms.openlocfilehash: 050b0bd997629ca189cfbe035e361de7a252d079
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="aecc0-104">Определение и распределение затрат</span><span class="sxs-lookup"><span data-stu-id="aecc0-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="aecc0-105">Распределения затрат перемещают затраты и доходы между типами затрат, местами возникновения затрат и объектами затрат.</span><span class="sxs-lookup"><span data-stu-id="aecc0-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="aecc0-106">Можно определить любое необходимое число распределений.</span><span class="sxs-lookup"><span data-stu-id="aecc0-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="aecc0-107">Каждое распределение состоит из:</span><span class="sxs-lookup"><span data-stu-id="aecc0-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="aecc0-108">Источник распределения.</span><span class="sxs-lookup"><span data-stu-id="aecc0-108">An allocation source.</span></span>  
-   <span data-ttu-id="aecc0-109">Одно или несколько назначений распределения.</span><span class="sxs-lookup"><span data-stu-id="aecc0-109">One or more allocation targets.</span></span>  

<span data-ttu-id="aecc0-110">Источник распределения задает затраты, которые должны быть распределены, а цели распределения определяют, куда затраты должны быть распределены.</span><span class="sxs-lookup"><span data-stu-id="aecc0-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="aecc0-111">Например, источником распределения затрат могут быть расходы за электричество и отопление.</span><span class="sxs-lookup"><span data-stu-id="aecc0-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="aecc0-112">Вы назначаете все расходы на электричество и отопление трем местам возникновения затрат: мастерской, производству и продажам.</span><span class="sxs-lookup"><span data-stu-id="aecc0-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="aecc0-113">Эти места возникновения затрат являются целями распределения.</span><span class="sxs-lookup"><span data-stu-id="aecc0-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="aecc0-114">Для каждого источника распределения указываются уровень распределения, период действия и вариант в качестве идентификатора группировки.</span><span class="sxs-lookup"><span data-stu-id="aecc0-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="aecc0-115">Можно использовать пакетное задание для установки фильтров и выбора определений распределения и последующего автоматического распределения затрат.</span><span class="sxs-lookup"><span data-stu-id="aecc0-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="aecc0-116">Для каждой цели распределения определяется база распределения.</span><span class="sxs-lookup"><span data-stu-id="aecc0-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="aecc0-117">База распределения может быть статической или динамической.</span><span class="sxs-lookup"><span data-stu-id="aecc0-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="aecc0-118">Статическое распределение основано на конкретном значении, таком как площадь в квадратных метрах или заданное соотношение распределения (например, 5:2: 4).</span><span class="sxs-lookup"><span data-stu-id="aecc0-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="aecc0-119">Базы динамического распределения зависят от изменяемых значений, таких как количество сотрудников в месте возникновения затрат или доход от продажи объекта затрат за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="aecc0-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="aecc0-120">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="aecc0-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="aecc0-121">По</span><span class="sxs-lookup"><span data-stu-id="aecc0-121">To</span></span>|<span data-ttu-id="aecc0-122">Ссылка</span><span class="sxs-lookup"><span data-stu-id="aecc0-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="aecc0-123">Настройте источник распределения и его целевые объекты.</span><span class="sxs-lookup"><span data-stu-id="aecc0-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="aecc0-124">Практическое руководство. Настройка источника и целей распределения</span><span class="sxs-lookup"><span data-stu-id="aecc0-124">How to: Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="aecc0-125">Настройте различные фильтры для базы динамического распределения.</span><span class="sxs-lookup"><span data-stu-id="aecc0-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="aecc0-126">Настройка фильтров для базы динамического распределения</span><span class="sxs-lookup"><span data-stu-id="aecc0-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="aecc0-127">См. пример того, как определять статическое распределение.</span><span class="sxs-lookup"><span data-stu-id="aecc0-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="aecc0-128">Пример сценария. Определение статических распределений на основе отношения распределений</span><span class="sxs-lookup"><span data-stu-id="aecc0-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="aecc0-129">См. пример того, как определять динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="aecc0-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="aecc0-130">Пример сценария. Определение динамических распределений на основе проданных товаров</span><span class="sxs-lookup"><span data-stu-id="aecc0-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="aecc0-131">См. также</span><span class="sxs-lookup"><span data-stu-id="aecc0-131">See Also</span></span>  
 <span data-ttu-id="aecc0-132">[Настройка учета затрат](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="aecc0-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="aecc0-133">[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="aecc0-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="aecc0-134">[Учет по затратам](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="aecc0-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="aecc0-135">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="aecc0-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="aecc0-136">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="aecc0-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

