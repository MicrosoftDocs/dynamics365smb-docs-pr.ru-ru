---
title: "Практическое руководство. Настройка центров затрат | Документы Майкрософт"
description: "Места возникновения затрат — это подразделения, которые отвечают за затраты и доход. Диаграмма мест возникновения затрат аналогична информации об измерениях для главной книги."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 38b6ce01e48f1b32c28b1883875a566d19f02ea3
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-cost-centers"></a><span data-ttu-id="19ac0-104">Настройка центров затрат</span><span class="sxs-lookup"><span data-stu-id="19ac0-104">Set Up Cost Centers</span></span>
<span data-ttu-id="19ac0-105">Места возникновения затрат — это подразделения, которые отвечают за затраты и доход.</span><span class="sxs-lookup"><span data-stu-id="19ac0-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="19ac0-106">Диаграмма мест возникновения затрат аналогична информации об измерениях для главной книги.</span><span class="sxs-lookup"><span data-stu-id="19ac0-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="19ac0-107">Диаграмму мест возникновения затрат можно настроить одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="19ac0-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="19ac0-108">Перенос значений измерений главной книги в план мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="19ac0-109">Все необходимые изменения можно внести после перевода.</span><span class="sxs-lookup"><span data-stu-id="19ac0-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="19ac0-110">Создайте новую диаграмму мест возникновения затрат, которая не зависит от Главной книги, или добавьте новое место возникновения затрат в существующую диаграмму мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="19ac0-111">Необходимо создать каждое место возникновения затрат по отдельности.</span><span class="sxs-lookup"><span data-stu-id="19ac0-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="19ac0-112">Перенос значений измерений главной книги в план мест возникновения затрат</span><span class="sxs-lookup"><span data-stu-id="19ac0-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="19ac0-113">Установите измерение, которое должно быть измерением центра затрат, в окне **Обновить измерения учета затрат**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-113">Set up a dimension to be the cost center dimension in the **Update Cost Acctg. Dimensions** window.</span></span> <span data-ttu-id="19ac0-114">Передаются только значения данного измерения.</span><span class="sxs-lookup"><span data-stu-id="19ac0-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="19ac0-115">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Центры затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="19ac0-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="19ac0-116">На вкладке **Действия** в группе **Функции** выберите **Получить места возникновения затрат из измерения** для возвращения значений измерений в диаграмму мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="19ac0-117">Функция перемещает значения измерений, заданные на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="19ac0-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="19ac0-118">Можно настроить поле **Выровнять измерение центра затрат** для односторонней синхронизации значений измерений из главной книги в диаграмму центров затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="19ac0-119">Нельзя определить синхронизацию диаграммы мест возникновения затрат со значениями измерений из главной книги.</span><span class="sxs-lookup"><span data-stu-id="19ac0-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="19ac0-120">Диаграмма мест возникновения затрат теперь содержит все заданные значения измерений из главной книги и включает должности и подытоги.</span><span class="sxs-lookup"><span data-stu-id="19ac0-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-window"></a><span data-ttu-id="19ac0-121">Создание новых центров затрат в окне "Диаграмма центров затрат"</span><span class="sxs-lookup"><span data-stu-id="19ac0-121">To create new cost centers in the Chart of Cost Centers window</span></span>  
<span data-ttu-id="19ac0-122">Можно настроить и обслуживать центры затрат в карточке **Карта центров затрат** или в окне **Диаграмма центров затрат**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-122">You can set up and maintain cost centers in either the **Cost Center Card** card or in the **Chart of Cost Centers** window.</span></span> <span data-ttu-id="19ac0-123">В рамках этой процедуры настраиваются центры затрат в окне **Диаграмма центров затрат**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-123">In this procedure, you set up cost centers in the **Chart of Cost Centers** window.</span></span>  

1. <span data-ttu-id="19ac0-124">Откройте окно **Диаграмма центров затрат** в режиме редактирования.</span><span class="sxs-lookup"><span data-stu-id="19ac0-124">Open the **Chart of Cost Centers** window in edit mode.</span></span>  
2. <span data-ttu-id="19ac0-125">В поле **Код** введите код центра затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="19ac0-126">У всех мест возникновения затрат должен быть код.</span><span class="sxs-lookup"><span data-stu-id="19ac0-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="19ac0-127">В поле **Имя** введите название центра затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="19ac0-128">Выберите стрелку раскрывающегося списка в поле **Тип строки**, чтобы указать назначение центра затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="19ac0-129">Для центров затрат, принадлежащих к типу счетов **Итог**, нужно заполнить поле **Группировка**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="19ac0-130">Используйте оператор **или**, который представлен вертикальной чертой (**&#124;**), чтобы установить диапазоны центров затрат.</span><span class="sxs-lookup"><span data-stu-id="19ac0-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="19ac0-131">Для мест возникновения затрат с типом строки **Сумма (до)** это поле заполняется автоматически при использовании функции отступа.</span><span class="sxs-lookup"><span data-stu-id="19ac0-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="19ac0-132">Заполните поля **Порядок сортировки** и **Подтип затрат**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="19ac0-133">Выберите следующую пустую строку, чтобы создать новое место возникновения затрат, затем повторите шаги с 2 по 5.</span><span class="sxs-lookup"><span data-stu-id="19ac0-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="19ac0-134">После настройки всех центров затрат выберите действие **Сдвинуть центры затрат**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="19ac0-135">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="19ac0-136">Если введены определения в полях **Группировка** для центров затрат **Сумма (до)**, то перед запуском этой функции необходимо снова ввести определения.</span><span class="sxs-lookup"><span data-stu-id="19ac0-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="19ac0-137">Функция переопределяет значения во всех полях **Сумма (до)**.</span><span class="sxs-lookup"><span data-stu-id="19ac0-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="19ac0-138">См. также</span><span class="sxs-lookup"><span data-stu-id="19ac0-138">See Also</span></span>  
[<span data-ttu-id="19ac0-139">Учет по затратам</span><span class="sxs-lookup"><span data-stu-id="19ac0-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="19ac0-140">[Настройка учета затрат](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="19ac0-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="19ac0-141">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="19ac0-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="19ac0-142">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="19ac0-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="19ac0-143">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="19ac0-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

