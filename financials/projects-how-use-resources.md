---
title: "Регистрация и корректировка потребления ресурсов и цен | Документы Майкрософт"
description: "Описывается процедура регистрации потребления ресурсов, связанных с работой, для отслеживания и управления затратами, ценами и типами работ."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 48692c9837007c6dd9c3891f0940b6f15b1d6541
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="d52ef-103">Практическое руководство. Использование ресурсов для работ</span><span class="sxs-lookup"><span data-stu-id="d52ef-103">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="d52ef-104">Вы регистрируете потребления ресурсов в журнале работ, чтобы отслеживать затраты и цены, а также виды работ, которые связаны с работами.</span><span class="sxs-lookup"><span data-stu-id="d52ef-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="d52ef-105">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация использования для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="d52ef-105">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="d52ef-106">Использование ресурса также может учитываться в журнале ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d52ef-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="d52ef-107">Операции, учтенные в журнале ресурсов, не оказывают влияния на Главную книгу.</span><span class="sxs-lookup"><span data-stu-id="d52ef-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d52ef-108">Эта функция требует, чтобы было задано значение **Пакет**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="d52ef-109">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="d52ef-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="d52ef-110">Назначение ресурсов работам</span><span class="sxs-lookup"><span data-stu-id="d52ef-110">To assign resources to jobs</span></span>
<span data-ttu-id="d52ef-111">Ресурсы можно назначить работам, создав строки планирования работы для работы.</span><span class="sxs-lookup"><span data-stu-id="d52ef-111">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="d52ef-112">Дополнительные сведения см. в разделе [Практическое руководство. Создание работ](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="d52ef-112">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="d52ef-113">Регистрация потребления ресурсов для работы</span><span class="sxs-lookup"><span data-stu-id="d52ef-113">To record resource usage for a job</span></span>
1. <span data-ttu-id="d52ef-114">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы работ**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d52ef-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="d52ef-115">Откройте соответствующий раздел журнала работ, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="d52ef-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="d52ef-116">Когда журнал будет готов, выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-116">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="d52ef-117">Корректировка цен ресурсов</span><span class="sxs-lookup"><span data-stu-id="d52ef-117">To adjust resource prices</span></span>
<span data-ttu-id="d52ef-118">Для изменения стоимости или цен большого количества ресурсов рекомендуется воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="d52ef-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="d52ef-119">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Коррекция цен/стоимостей ресурсов**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d52ef-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="d52ef-120">Заполните поля в строке, как требуется, и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d52ef-121">При выполнении этого пакетного задания не добавляются и не корректируются альтернативные стоимости или цены ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d52ef-121">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="d52ef-122">Это меняет только содержимое поля в карточке ресурса для поля **Коррекция поля**, выбранного в пакетном задании.</span><span class="sxs-lookup"><span data-stu-id="d52ef-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="d52ef-123">Коррекция вступит в силу сразу для всех ресурсов, поэтому проверьте коэффициенты перед запуском пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d52ef-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="d52ef-124">Получения предложений по изменению цены ресурса на основе существующих альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="d52ef-124">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="d52ef-125">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d52ef-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="d52ef-126">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Resource Price Changes**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d52ef-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="d52ef-127">Выберите действие **Предлож. изменения цен ресурсов (цена)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="d52ef-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="d52ef-128">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-128">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="d52ef-129">После выполнения пакетного задания окно **Изменение цен ресурсов** показывает результаты пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d52ef-129">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="d52ef-130">Получение предложений по изменению цены ресурса на основе стандартных цен</span><span class="sxs-lookup"><span data-stu-id="d52ef-130">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="d52ef-131">Если требуется настроить несколько альтернативных цен ресурсов на основе стандартных цен из карточек ресурсов, можно воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="d52ef-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="d52ef-132">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Resource Price Changes**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d52ef-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="d52ef-133">Выберите действие **Предлож. изменение цен ресурсов (рес.)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="d52ef-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="d52ef-134">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-134">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="d52ef-135">После выполнения пакетного задания откройте окно **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d52ef-135">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="d52ef-136">Получение предложений по изменению цены ресурса на основе альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="d52ef-136">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="d52ef-137">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d52ef-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="d52ef-138">В поле **Поиск** введите **Предлож. изменения цен ресурсов (цена)**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d52ef-138">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d52ef-139">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="d52ef-139">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="d52ef-140">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d52ef-140">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="d52ef-141">После выполнения пакетного задания откройте окно **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="d52ef-141">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="d52ef-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d52ef-142">See Also</span></span>
[<span data-ttu-id="d52ef-143">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="d52ef-143">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="d52ef-144">Финансы</span><span class="sxs-lookup"><span data-stu-id="d52ef-144">Finance</span></span>](finance.md)  
<span data-ttu-id="d52ef-145">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="d52ef-145">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="d52ef-146">[Продажи](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="d52ef-146">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="d52ef-147">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d52ef-147">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
