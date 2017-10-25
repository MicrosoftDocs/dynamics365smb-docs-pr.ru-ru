---
title: "Настройка циклов продаж и этапов циклов | Документы Майкрософт"
description: "Описывается, как определять этапы продаж от первого контакта до закрытия, чтобы создавать циклы и назначать их возможным сделкам в Financials."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 29f9caa8f01fe8e4cfd0f65cc290d82a49fb36bb
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="0f4f7-103">Практическое руководство. Настройка циклов продаж и этапов циклов</span><span class="sxs-lookup"><span data-stu-id="0f4f7-103">How to: Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="0f4f7-104">Прежде чем начать использовать возможностей продаж, необходимо настроить циклы продаж и их этапы.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-104">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="0f4f7-105">Цикл продаж состоит из последовательности этапов от первого контакта до закрытия продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-105">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="0f4f7-106">Каждый этап может содержать определенные требования, которые должны быть соблюдены, такие как обязательное наличие предложения по продаже перед переходом к следующей стадии.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-106">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="0f4f7-107">Можно также указать, можно ли пропустить этап.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-107">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="0f4f7-108">Можно настроить столько циклов продаж, сколько требуется, а также необходимое количество этапов цикла продаж в каждом цикле.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-108">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="0f4f7-109">Реализация циклов продаж включает настройку цикла продаж, определение различных этапов цикла и назначение циклов возможностям.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-109">Implementing opportunity sales cycles involves setting up the sales cycle, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span> <span data-ttu-id="0f4f7-110">Назначение соответствующих действий или задач возможностям также может быть частью настройки цикла продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-110">Assigning the relevant activity or tasks to the opportunity may also be part of setting up a sales cycle.</span></span>

<span data-ttu-id="0f4f7-111">Также в этом разделе описывается, как настроить задачи и действия и как назначить задачи действиям.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-111">This topic also describes how to set up tasks and activities, and how to assign tasks to activities.</span></span> <span data-ttu-id="0f4f7-112">Дополнительные сведения см. в подразделе "Настройка действий с задачами".</span><span class="sxs-lookup"><span data-stu-id="0f4f7-112">For more information, see the "To set up activities with tasks" section.</span></span>

## <a name="to-set-up-opportunity-sales-cycle-codes"></a><span data-ttu-id="0f4f7-113">Настройка кодов циклов продаж для возможностей</span><span class="sxs-lookup"><span data-stu-id="0f4f7-113">To set up opportunity sales cycle codes</span></span>
1. <span data-ttu-id="0f4f7-114">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Циклы продаж**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="0f4f7-115">Откроется окно **Циклы продаж**, содержащее все существующие циклы продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-115">The **Sales Cycles** window opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="0f4f7-116">Выберите действие **Создать** и введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-116">Choose the **New** action, and fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="0f4f7-117">Повторите эти шаги, чтобы настроить необходимое количество циклов продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-117">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="0f4f7-118">После настройки циклов продаж может понадобиться настроить различные этапы внутри каждого цикла.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-118">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="0f4f7-119">Определение этапов цикла продаж</span><span class="sxs-lookup"><span data-stu-id="0f4f7-119">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="0f4f7-120">В окне **Циклы продаж** выберите цикл продаж, для которого требуется настроить этапы, и выберите действие **Этапы**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-120">In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="0f4f7-121">Откроется окно **Этапы цикла продажи**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-121">The **Sales Cycle Stages** window opens.</span></span>
2. <span data-ttu-id="0f4f7-122">Выберите действие **Создать**, чтобы создать новый этап цикла продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-122">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="0f4f7-123">Повторите эти шаги для настройки нужного количества стадий цикла продаж.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-123">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycles-to-opportunities"></a><span data-ttu-id="0f4f7-124">Назначение циклов стадий возможностям</span><span class="sxs-lookup"><span data-stu-id="0f4f7-124">To assign stage cycles to opportunities</span></span>
<span data-ttu-id="0f4f7-125">После добавления цикла продаж вы можете добавлять возможности продаж и назначать цикл продаж возможностям, устанавливая поле **Код цикла продаж**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-125">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="0f4f7-126">Дополнительные сведения см. в разделе [Практическое руководство. Создание возможностей продаж](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="0f4f7-126">For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

## <a name="to-set-up-activities-with-tasks"></a><span data-ttu-id="0f4f7-127">Настройка действий с задачами</span><span class="sxs-lookup"><span data-stu-id="0f4f7-127">To set up activities with tasks</span></span>
<span data-ttu-id="0f4f7-128">Вы можете объединять задачи, например отдельные шаги, в действия.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-128">You can combine multiple task, for example tasks that each represent a step, in activities.</span></span> <span data-ttu-id="0f4f7-129">Задачи действий связаны друг с другом с помощью формулы даты.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-129">Activity tasks are related to each other by a date formula.</span></span> <span data-ttu-id="0f4f7-130">Вы можете назначить действия возможностям, менеджерам по продажам или контактам.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-130">You can assign activities to opportunities, salespeople, or contacts.</span></span>

1. <span data-ttu-id="0f4f7-131">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Циклы продаж**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-131">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Activities**, and then choose the related link.</span></span>
2. <span data-ttu-id="0f4f7-132">Выберите действие **Создать** и введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-132">Choose the **New** action, and fill in the fields as necessary.</span></span>
3. <span data-ttu-id="0f4f7-133">На экспресс-вкладке **Строки** заполните поля соответствующим образом, чтобы определить одну или несколько задач в действии.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-133">On the **Lines** FastTab, fill in the fields as necessary to define one or more tasks in the activity.</span></span>

## <a name="to-assign-tasks-or-activities-of-tasks-to-opportunities"></a><span data-ttu-id="0f4f7-134">Назначение задач или действий задач возможностям</span><span class="sxs-lookup"><span data-stu-id="0f4f7-134">To assign tasks or activities of tasks to opportunities</span></span>
<span data-ttu-id="0f4f7-135">После настройки задачи вы можете назначить ее возможности продажи и таким образом назначить действие, к которому относится задача.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-135">When you have set up a task, you can assign it to a sales opportunity and thereby assign the activity that the task belongs to.</span></span>

> [!NOTE]  
>   <span data-ttu-id="0f4f7-136">В этой процедуре описано, как назначать задачи действий возможностям.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-136">This procedure describes how to assign activity tasks to opportunities.</span></span> <span data-ttu-id="0f4f7-137">Шаги похожи на процедуру назначения задач менеджерам по продажам и контактам.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-137">the steps are similar when you assign tasks to salespeople and contacts.</span></span>

1. <span data-ttu-id="0f4f7-138">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Возможности**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-138">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Opportunities**, and then choose the related link.</span></span>
2. <span data-ttu-id="0f4f7-139">Выберите возможность, затем выберите действие **Задачи**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-139">Select an opportunity, and then choose the **Tasks** action.</span></span>
3. <span data-ttu-id="0f4f7-140">В окне **Список задач** выберите действие **Создать задачу**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-140">In the **Task List** window, choose the **Create Task** action.</span></span>
4.  <span data-ttu-id="0f4f7-141">В окне **Создать задачу** заполните поля по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-141">The **Create Task** window, fill in the fields as necessary.</span></span>

    <span data-ttu-id="0f4f7-142">Обратите внимание на поле **Возможность**, в которое автоматически подставляется текущая возможность.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-142">Notice in the **Opportunity** field, that it is automatically assigned to the opportunity in question.</span></span>
5. <span data-ttu-id="0f4f7-143">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-143">Choose the **OK** button.</span></span>
6. <span data-ttu-id="0f4f7-144">В окне **Список задач** выберите новую задачу, а затем выберите действие **Назначить действия**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-144">In the **Task List** window, select the new task, and then choose the **Assign Activities** action.</span></span>
7. <span data-ttu-id="0f4f7-145">В окне **Назначить действия** заполните поля по мере необходимости, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="0f4f7-145">In the **Assign Activity** window, fill in the fields as necessary, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="0f4f7-146">См. также</span><span class="sxs-lookup"><span data-stu-id="0f4f7-146">See Also</span></span>
[<span data-ttu-id="0f4f7-147">Обработка возможностей продаж</span><span class="sxs-lookup"><span data-stu-id="0f4f7-147">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="0f4f7-148">Продажи</span><span class="sxs-lookup"><span data-stu-id="0f4f7-148">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="0f4f7-149">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0f4f7-149">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

