---
title: Практическое руководство. Настройка центров затрат | Документы Майкрософт
description: Места возникновения затрат — это подразделения, которые отвечают за затраты и доход. Диаграмма мест возникновения затрат аналогична информации об измерениях для главной книги.
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
redirect_url: finance-set-up-cost-accounting
ms.openlocfilehash: 48c1b9800c1e89246ba84122b4af56d75fdf6f9f
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1243530"
---
# <a name="set-up-cost-centers"></a><span data-ttu-id="7a277-104">Настройка центров затрат</span><span class="sxs-lookup"><span data-stu-id="7a277-104">Set Up Cost Centers</span></span>
<span data-ttu-id="7a277-105">Места возникновения затрат — это подразделения, которые отвечают за затраты и доход.</span><span class="sxs-lookup"><span data-stu-id="7a277-105">Cost centers are departments that are responsible for costs and income.</span></span> <span data-ttu-id="7a277-106">Диаграмма мест возникновения затрат аналогична информации об измерениях для главной книги.</span><span class="sxs-lookup"><span data-stu-id="7a277-106">The chart of cost centers is similar to the dimension information for the general ledger.</span></span> <span data-ttu-id="7a277-107">Диаграмму мест возникновения затрат можно настроить одним из следующих способов:</span><span class="sxs-lookup"><span data-stu-id="7a277-107">You can set up the chart of cost centers in the following ways:</span></span>  

-   <span data-ttu-id="7a277-108">Перенос значений измерений главной книги в план мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-108">Transfer dimension values in the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="7a277-109">Все необходимые изменения можно внести после перевода.</span><span class="sxs-lookup"><span data-stu-id="7a277-109">You can make any necessary adjustments after the transfer.</span></span>  
-   <span data-ttu-id="7a277-110">Создайте новую диаграмму мест возникновения затрат, которая не зависит от Главной книги, или добавьте новое место возникновения затрат в существующую диаграмму мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-110">Create a new chart of cost center that is independent of the general ledger or add a new cost center to an existing chart of cost center.</span></span> <span data-ttu-id="7a277-111">Необходимо создать каждое место возникновения затрат по отдельности.</span><span class="sxs-lookup"><span data-stu-id="7a277-111">You must create each cost center individually.</span></span>  

## <a name="to-transfer-dimension-values-in-the-general-ledger-to-the-chart-of-cost-centers"></a><span data-ttu-id="7a277-112">Перенос значений измерений главной книги в план мест возникновения затрат</span><span class="sxs-lookup"><span data-stu-id="7a277-112">To transfer dimension values in the general ledger to the chart of cost centers</span></span>  
1.  <span data-ttu-id="7a277-113">Установите измерение, которое должно быть измерением центра затрат, на странице **Обновить измерения учета затрат**.</span><span class="sxs-lookup"><span data-stu-id="7a277-113">Set up a dimension to be the cost center dimension on the **Update Cost Acctg. Dimensions** page.</span></span> <span data-ttu-id="7a277-114">Передаются только значения данного измерения.</span><span class="sxs-lookup"><span data-stu-id="7a277-114">Only the values from this dimension are transferred.</span></span>  
2.  <span data-ttu-id="7a277-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Диаграмма центров затрат**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="7a277-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Cost Centers**, and then choose the related link.</span></span>  
3.  <span data-ttu-id="7a277-116">На вкладке **Действия** в группе **Функции** выберите **Получить места возникновения затрат из измерения** для возвращения значений измерений в диаграмму мест возникновения затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-116">On the **Actions** tab, in the **Functions** group, choose **Get Cost Centers from Dimension** to transfer dimension values to the chart of cost centers.</span></span> <span data-ttu-id="7a277-117">Функция перемещает значения измерений, заданные на шаге 1.</span><span class="sxs-lookup"><span data-stu-id="7a277-117">The function transfers the dimension values that you defined in step 1.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="7a277-118">Можно настроить поле **Выровнять измерение центра затрат** для односторонней синхронизации значений измерений из главной книги в диаграмму центров затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-118">You can set up the **Align Cost Center Dimension**  field to define a one-way synchronization of dimension values from the general ledger to the chart of cost centers.</span></span> <span data-ttu-id="7a277-119">Нельзя определить синхронизацию диаграммы мест возникновения затрат со значениями измерений из главной книги.</span><span class="sxs-lookup"><span data-stu-id="7a277-119">You cannot define a synchronization of the chart of cost centers to dimension values from the general ledger.</span></span>  

<span data-ttu-id="7a277-120">Диаграмма мест возникновения затрат теперь содержит все заданные значения измерений из главной книги и включает должности и подытоги.</span><span class="sxs-lookup"><span data-stu-id="7a277-120">The chart of cost centers now contains all specified dimension values from the general ledger and includes titles and subtotals.</span></span>  

## <a name="to-create-new-cost-centers-in-the-chart-of-cost-centers-page"></a><span data-ttu-id="7a277-121">Создание новых центров затрат на странице "Диаграмма центров затрат"</span><span class="sxs-lookup"><span data-stu-id="7a277-121">To create new cost centers in the Chart of Cost Centers page</span></span>  
<span data-ttu-id="7a277-122">Можно настроить и обслуживать центры затрат в карточке **Карта центров затрат** или на странице **Диаграмма центров затрат**.</span><span class="sxs-lookup"><span data-stu-id="7a277-122">You can set up and maintain cost centers in either the **Cost Center Card** card or on the **Chart of Cost Centers** page.</span></span> <span data-ttu-id="7a277-123">В рамках этой процедуры настраиваются центры затрат на странице **Диаграмма центров затрат**.</span><span class="sxs-lookup"><span data-stu-id="7a277-123">In this procedure, you set up cost centers on the **Chart of Cost Centers** page.</span></span>  

1. <span data-ttu-id="7a277-124">Откройте страницу **Диаграмма центров затрат** в режиме редактирования.</span><span class="sxs-lookup"><span data-stu-id="7a277-124">Open the **Chart of Cost Centers** page in edit mode.</span></span>  
2. <span data-ttu-id="7a277-125">В поле **Код** введите код центра затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-125">In the **Code** field, enter the cost center code.</span></span> <span data-ttu-id="7a277-126">У всех мест возникновения затрат должен быть код.</span><span class="sxs-lookup"><span data-stu-id="7a277-126">All cost centers must have a code.</span></span>  
3. <span data-ttu-id="7a277-127">В поле **Имя** введите название центра затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-127">In the **Name** field, enter the cost center name.</span></span>  
4. <span data-ttu-id="7a277-128">Выберите стрелку раскрывающегося списка в поле **Тип строки**, чтобы указать назначение центра затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-128">Choose the drop-down arrow in the **Line Type** field to specify the purpose of the cost center.</span></span>  

    - <span data-ttu-id="7a277-129">Для центров затрат, принадлежащих к типу счетов **Итог**, нужно заполнить поле **Группировка**.</span><span class="sxs-lookup"><span data-stu-id="7a277-129">For cost centers of the **Total** type, you must fill in the **Totaling** field.</span></span> <span data-ttu-id="7a277-130">Используйте оператор **или**, который представлен вертикальной чертой (**&#124;**), чтобы установить диапазоны центров затрат.</span><span class="sxs-lookup"><span data-stu-id="7a277-130">Use the **or** operator, which is a vertical line (**&#124;**) to set ranges of cost centers.</span></span>  
    - <span data-ttu-id="7a277-131">Для мест возникновения затрат с типом строки **Сумма (до)** это поле заполняется автоматически при использовании функции отступа.</span><span class="sxs-lookup"><span data-stu-id="7a277-131">For cost centers of the **End-Total** line type, this field is filled in automatically when you use the indent function.</span></span>  
5.  <span data-ttu-id="7a277-132">Заполните поля **Порядок сортировки** и **Подтип затрат**.</span><span class="sxs-lookup"><span data-stu-id="7a277-132">Fill in the **Sorting Order** and **Cost Subtype** fields.</span></span>  
6.  <span data-ttu-id="7a277-133">Выберите следующую пустую строку, чтобы создать новое место возникновения затрат, затем повторите шаги с 2 по 5.</span><span class="sxs-lookup"><span data-stu-id="7a277-133">Choose the next empty line to create a new cost center, and then repeat steps 2 through 5.</span></span>  
7.  <span data-ttu-id="7a277-134">После настройки всех центров затрат выберите действие **Сдвинуть центры затрат**.</span><span class="sxs-lookup"><span data-stu-id="7a277-134">After you have set up all the cost centers, choose the **Indent Cost Centers** action.</span></span> <span data-ttu-id="7a277-135">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="7a277-135">Choose the **Yes** button.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="7a277-136">Если введены определения в полях **Группировка** для центров затрат **Сумма (до)**, то перед запуском этой функции необходимо снова ввести определения.</span><span class="sxs-lookup"><span data-stu-id="7a277-136">If you have entered definitions in the **Totaling** fields for **End-Total** cost centers before you run the indent function, then you must enter them again.</span></span> <span data-ttu-id="7a277-137">Функция переопределяет значения во всех полях **Сумма (до)**.</span><span class="sxs-lookup"><span data-stu-id="7a277-137">The function overwrites the values in all **End-Total** fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="7a277-138">См. также</span><span class="sxs-lookup"><span data-stu-id="7a277-138">See Also</span></span>  
[<span data-ttu-id="7a277-139">Учет по затратам</span><span class="sxs-lookup"><span data-stu-id="7a277-139">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
<span data-ttu-id="7a277-140">[Настройка учета затрат](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="7a277-140">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
<span data-ttu-id="7a277-141">[Терминология в учете затрат](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="7a277-141">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
[<span data-ttu-id="7a277-142">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="7a277-142">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
<span data-ttu-id="7a277-143">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7a277-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
