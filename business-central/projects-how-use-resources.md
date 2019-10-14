---
title: Регистрация и корректировка потребления ресурсов и цен | Документация Майкрософт
description: Описывается процедура регистрации потребления ресурсов, связанных с работой, для отслеживания и управления затратами, ценами и типами работ.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 8d637a21a795db46554a45c688bf7ad081533e4a
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2312704"
---
# <a name="use-resources-for-jobs"></a><span data-ttu-id="95f5a-103">Использование ресурсов для работ</span><span class="sxs-lookup"><span data-stu-id="95f5a-103">Use Resources for Jobs</span></span>
<span data-ttu-id="95f5a-104">Вы регистрируете потребления ресурсов в журнале работ, чтобы отслеживать затраты и цены, а также виды работ, которые связаны с работами.</span><span class="sxs-lookup"><span data-stu-id="95f5a-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="95f5a-105">Дополнительные сведения см. в разделе [Регистрация использования для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="95f5a-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="95f5a-106">Использование ресурса также может учитываться в журнале ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95f5a-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="95f5a-107">Операции, учтенные в журнале ресурсов, не оказывают влияния на Главную книгу.</span><span class="sxs-lookup"><span data-stu-id="95f5a-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="95f5a-108">Назначение ресурсов работам</span><span class="sxs-lookup"><span data-stu-id="95f5a-108">To assign resources to jobs</span></span>
<span data-ttu-id="95f5a-109">Ресурсы можно назначить работам, создав строки планирования работы для работы.</span><span class="sxs-lookup"><span data-stu-id="95f5a-109">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="95f5a-110">Дополнительные сведения см. в разделе [Создание работ](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="95f5a-110">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="95f5a-111">Регистрация потребления ресурсов для работы</span><span class="sxs-lookup"><span data-stu-id="95f5a-111">To record resource usage for a job</span></span>
1. <span data-ttu-id="95f5a-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы работ**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95f5a-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="95f5a-113">Откройте соответствующий раздел журнала работ, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="95f5a-113">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="95f5a-114">Когда журнал будет готов, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="95f5a-114">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="95f5a-115">Корректировка цен ресурсов</span><span class="sxs-lookup"><span data-stu-id="95f5a-115">To adjust resource prices</span></span>
<span data-ttu-id="95f5a-116">Для изменения стоимости или цен большого количества ресурсов рекомендуется воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="95f5a-116">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="95f5a-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коррекция цен/стоимостей ресурсов**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95f5a-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="95f5a-118">Заполните поля в строке, как требуется, и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="95f5a-118">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="95f5a-119">При выполнении этого пакетного задания не добавляются и не корректируются альтернативные стоимости или цены ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95f5a-119">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="95f5a-120">Это меняет только содержимое поля в карточке ресурса для поля **Коррекция поля**, выбранного в пакетном задании.</span><span class="sxs-lookup"><span data-stu-id="95f5a-120">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="95f5a-121">Коррекция вступит в силу сразу для всех ресурсов, поэтому проверьте коэффициенты перед запуском пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="95f5a-121">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="95f5a-122">Получения предложений по изменению цены ресурса на основе существующих альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="95f5a-122">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="95f5a-123">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95f5a-123">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="95f5a-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Изменение цен ресурсов**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95f5a-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="95f5a-125">Выберите действие **Предлож. изменения цен ресурсов (цена)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="95f5a-125">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="95f5a-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="95f5a-126">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="95f5a-127">После выполнения пакетного задания страница **Изменение цен ресурсов** показывает результаты пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="95f5a-127">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="95f5a-128">Получение предложений по изменению цены ресурса на основе стандартных цен</span><span class="sxs-lookup"><span data-stu-id="95f5a-128">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="95f5a-129">Если требуется настроить несколько альтернативных цен ресурсов на основе стандартных цен из карточек ресурсов, можно воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="95f5a-129">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="95f5a-130">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Изменение цен ресурсов**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95f5a-130">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="95f5a-131">Выберите действие **Предлож. изменение цен ресурсов (рес.)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="95f5a-131">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="95f5a-132">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="95f5a-132">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="95f5a-133">После выполнения пакетного задания откройте страницу **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="95f5a-133">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="95f5a-134">Получение предложений по изменению цены ресурса на основе альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="95f5a-134">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="95f5a-135">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95f5a-135">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="95f5a-136">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Предлож. изменения цен ресурсов (цена)**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95f5a-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95f5a-137">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="95f5a-137">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="95f5a-138">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="95f5a-138">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="95f5a-139">После выполнения пакетного задания откройте страницу **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="95f5a-139">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="95f5a-140">См. также</span><span class="sxs-lookup"><span data-stu-id="95f5a-140">See Also</span></span>
[<span data-ttu-id="95f5a-141">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="95f5a-141">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="95f5a-142">Финансы</span><span class="sxs-lookup"><span data-stu-id="95f5a-142">Finance</span></span>](finance.md)  
<span data-ttu-id="95f5a-143">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="95f5a-143">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="95f5a-144">[Продажи](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="95f5a-144">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="95f5a-145">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="95f5a-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
