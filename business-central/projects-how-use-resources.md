---
title: Регистрация и корректировка потребления ресурсов и цен | Документация Майкрософт
description: Описывается процедура регистрации потребления ресурсов, связанных с работой, для отслеживания и управления затратами, ценами и типами работ.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 777de65d2cda454491b6c3ea82ebb99d4839dce4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780386"
---
# <a name="use-resources-for-jobs"></a><span data-ttu-id="f8f31-103">Использование ресурсов для работ</span><span class="sxs-lookup"><span data-stu-id="f8f31-103">Use Resources for Jobs</span></span>
<span data-ttu-id="f8f31-104">Вы регистрируете потребления ресурсов в журнале работ, чтобы отслеживать затраты и цены, а также виды работ, которые связаны с работами.</span><span class="sxs-lookup"><span data-stu-id="f8f31-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="f8f31-105">Дополнительные сведения см. в разделе [Регистрация использования для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="f8f31-105">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f8f31-106">Вы также можете приобрести внешние ресурсы, например, чтобы выставить счет поставщику за выполненную работу.</span><span class="sxs-lookup"><span data-stu-id="f8f31-106">You can also purchase external resources, for example, to invoice a vendor for work delivered.</span></span> <span data-ttu-id="f8f31-107">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="f8f31-107">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

<span data-ttu-id="f8f31-108">Использование ресурса также может учитываться в журнале ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f8f31-108">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="f8f31-109">Операции, учтенные в журнале ресурсов, не оказывают влияния на Главную книгу.</span><span class="sxs-lookup"><span data-stu-id="f8f31-109">Entries posted in a resource journal have no effect on the general ledger.</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="f8f31-110">Назначение ресурсов работам</span><span class="sxs-lookup"><span data-stu-id="f8f31-110">To assign resources to jobs</span></span>
<span data-ttu-id="f8f31-111">Ресурсы можно назначить работам, создав строки планирования работы для работы.</span><span class="sxs-lookup"><span data-stu-id="f8f31-111">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="f8f31-112">Дополнительные сведения см. в разделе [Создание работ](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="f8f31-112">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="f8f31-113">Регистрация потребления ресурсов для работы</span><span class="sxs-lookup"><span data-stu-id="f8f31-113">To record resource usage for a job</span></span>
1. <span data-ttu-id="f8f31-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы работ**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8f31-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="f8f31-115">Откройте соответствующий раздел журнала работ, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="f8f31-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="f8f31-116">Когда журнал будет готов, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="f8f31-116">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="f8f31-117">Корректировка цен ресурсов</span><span class="sxs-lookup"><span data-stu-id="f8f31-117">To adjust resource prices</span></span>
<span data-ttu-id="f8f31-118">Для изменения стоимости или цен большого количества ресурсов рекомендуется воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="f8f31-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="f8f31-119">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Коррекция цен/стоимостей ресурсов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8f31-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="f8f31-120">Заполните поля в строке, как требуется, и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f8f31-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="f8f31-121">При выполнении этого пакетного задания не добавляются и не корректируются альтернативные стоимости или цены ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f8f31-121">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="f8f31-122">Это меняет только содержимое поля в карточке ресурса для поля **Коррекция поля**, выбранного в пакетном задании.</span><span class="sxs-lookup"><span data-stu-id="f8f31-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="f8f31-123">Коррекция вступит в силу сразу для всех ресурсов, поэтому проверьте коэффициенты перед запуском пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="f8f31-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="f8f31-124">Получения предложений по изменению цены ресурса на основе существующих альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="f8f31-124">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="f8f31-125">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f8f31-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="f8f31-126">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Изменение цен ресурсов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8f31-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="f8f31-127">Выберите действие **Предлож. изменения цен ресурсов (цена)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="f8f31-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f8f31-128">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f8f31-128">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f8f31-129">После выполнения пакетного задания страница **Изменение цен ресурсов** показывает результаты пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="f8f31-129">When the batch job is finished, the **Resource Price Changes** page shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="f8f31-130">Получение предложений по изменению цены ресурса на основе стандартных цен</span><span class="sxs-lookup"><span data-stu-id="f8f31-130">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="f8f31-131">Если требуется настроить несколько альтернативных цен ресурсов на основе стандартных цен из карточек ресурсов, можно воспользоваться пакетным заданием.</span><span class="sxs-lookup"><span data-stu-id="f8f31-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="f8f31-132">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Изменение цен ресурсов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8f31-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="f8f31-133">Выберите действие **Предлож. изменение цен ресурсов (рес.)**, затем заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="f8f31-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="f8f31-134">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f8f31-134">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f8f31-135">После выполнения пакетного задания откройте страницу **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="f8f31-135">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="f8f31-136">Получение предложений по изменению цены ресурса на основе альтернативных цен</span><span class="sxs-lookup"><span data-stu-id="f8f31-136">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="f8f31-137">Если для некоторых ресурсов уже определены альтернативные цены, можно воспользоваться пакетным заданием для установления нескольких альтернативных цен ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f8f31-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="f8f31-138">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Предлож. изменения цен ресурсов (цена)**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f8f31-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f8f31-139">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="f8f31-139">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="f8f31-140">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f8f31-140">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="f8f31-141">После выполнения пакетного задания откройте страницу **Изменение цен ресурсов** для просмотра результатов пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="f8f31-141">When the batch job is finished, open the **Resource Price Changes** page to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="f8f31-142">См. также</span><span class="sxs-lookup"><span data-stu-id="f8f31-142">See Also</span></span>
[<span data-ttu-id="f8f31-143">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="f8f31-143">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="f8f31-144">Финансы</span><span class="sxs-lookup"><span data-stu-id="f8f31-144">Finance</span></span>](finance.md)  
<span data-ttu-id="f8f31-145">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="f8f31-145">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="f8f31-146">[Продажи](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="f8f31-146">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="f8f31-147">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f8f31-147">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]