---
title: "Реклассификация основных средств | Документы Майкрософт"
description: "Вы выполняете реклассификацию основных средств для их перемещения в другие отделы, разделения или объединения с другими основными средствами."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 4e29a08e9b0fd9c20dac12bb32dd1be604ff2dcf
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-transfer-split-or-combine-fixed-assets"></a><span data-ttu-id="6b0b8-103">Практическое руководство. Перемещение, разделение или объединение основных средств</span><span class="sxs-lookup"><span data-stu-id="6b0b8-103">How to: Transfer, Split, or Combine Fixed Assets</span></span>
<span data-ttu-id="6b0b8-104">Для перемещения, разделения и объединения основных средств можно использовать журнал реклассификации основных средств.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-104">You use the fixed asset reclassification journal to transfer, split up, and combine fixed assets.</span></span> <span data-ttu-id="6b0b8-105">Результаты реклассификации основных средств можно просматривать или печатать с помощью отчета **ОС - балансовая стоимость 02**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-105">You view or print the results of fixed asset reclassification with the **Fixed Asset-Book Value 02** report.</span></span>

## <a name="to-transfer-a-fixed-asset-to-a-different-department"></a><span data-ttu-id="6b0b8-106">Перемещение основного средства в другое подразделение</span><span class="sxs-lookup"><span data-stu-id="6b0b8-106">To transfer a fixed asset to a different department</span></span>
<span data-ttu-id="6b0b8-107">Перемещение основного средства в другое подразделение может потребоваться, например, если основное средство размещается в производственном отделе, когда оно находится в состоянии строительства; затем, когда оно будет готово, оно перемещается в административный отдел.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-107">You may need to transfer a fixed asset to a different department when, for example, you place an asset in the production department while it is under construction and then move it to the administration department when it is finished.</span></span>  

1. <span data-ttu-id="6b0b8-108">Настройте новое основное средство.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-108">Set up a new fixed asset.</span></span> <span data-ttu-id="6b0b8-109">Введите новое подразделение в поле **Код подразделения**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-109">Enter the new department in the **Department Code** field.</span></span>
2. <span data-ttu-id="6b0b8-110">Назначьте книгу амортизации основных средств новому основному средству.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-110">Assign a fixed asset depreciation book to the new fixed asset.</span></span> <span data-ttu-id="6b0b8-111">Дополнительные сведения см. в разделе [Практическое руководство. Приобретение основных средств](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b8-111">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span></span>
3. <span data-ttu-id="6b0b8-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы реклассификации ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Reclass. Journals**, and then choose the related link.</span></span>
4. <span data-ttu-id="6b0b8-113">Создайте журнал реклассификации, где поле **Номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-113">Create a reclassification journal where the **FA No.**</span></span> <span data-ttu-id="6b0b8-114">содержит исходное основное средство, а поле **Новый номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-114">field contains the original fixed asset, and the **New FA No.**</span></span> <span data-ttu-id="6b0b8-115">содержит новое основное средство, которое необходимо переместить.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-115">field contains the new fixed asset to be moved.</span></span>  
5. <span data-ttu-id="6b0b8-116">Выберите действие **Реклассиф.**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-116">Choose the **Reclassify** action.</span></span>

    <span data-ttu-id="6b0b8-117">Создаются две строки в журнале ГК учета основных средств, используя шаблон и раздел, указанные в окне **ОС - настройка журнала** для указанной книги амортизации.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-117">Two lines are now created in the fixed asset G/L journal using the template and batch that you have specified in the **FA Journal Setup** window for the specified depreciation book.</span></span> <span data-ttu-id="6b0b8-118">Дополнительные сведения см. в разделе [Практическое руководство. Настройка амортизации основных средств](fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b8-118">For more information, see [How to: Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md).</span></span>
6. <span data-ttu-id="6b0b8-119">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы ГК ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>    
7. <span data-ttu-id="6b0b8-120">В окне **Журнал ГК учета основных средств** выберите действие **Учесть**, чтобы учесть реклассификацию, выполненную в шагах 4 и 5.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-120">In the **Fixed Asset G/L Journal** window, choose the **Post** action to post the reclassification that you performed in steps 4 and 5.</span></span>

<span data-ttu-id="6b0b8-121">Если выполняется учет стоимости приобретения одного основного средства, можно использовать журнал реклассификации основных средств для разделения стоимости приобретения среди нескольких основных средств.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-121">If you have posted an acquisition cost for one asset, you can use the fixed asset reclassification journal to split the acquisition cost among several assets.</span></span>  

## <a name="to-split-a-fixed-asset-into-three-fixed-assets"></a><span data-ttu-id="6b0b8-122">Разделение основного средства на три основные средства</span><span class="sxs-lookup"><span data-stu-id="6b0b8-122">To split a fixed asset into three fixed assets</span></span>
<span data-ttu-id="6b0b8-123">Можно разделить одно основное средство на несколько основных средств, например если требуется разделить основное средство на три различных подразделения.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-123">You can split one fixed asset into multiple fixed assets, for example when you need to distribute a fixed asset onto three different departments.</span></span> <span data-ttu-id="6b0b8-124">В таком случае можно, например, переместить 25% стоимости приобретения и амортизации для исходного основного средства на второе основное средство, а 45% на третье основное средство.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-124">In that case, you can move, for example, 25 percent of the acquisition cost and depreciation for the original fixed asset to the second fixed asset and 45 percent to the third asset.</span></span> <span data-ttu-id="6b0b8-125">Остальные 30% остаются на первоначальном основном средстве.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-125">The remaining 30 percent will remain on the original fixed asset.</span></span>

1. <span data-ttu-id="6b0b8-126">Настройте два новых основных средства.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-126">Set up two new fixed assets.</span></span> <span data-ttu-id="6b0b8-127">Введите новое подразделение в поле **Код подразделения**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-127">Enter the new department in the **Department Code** field.</span></span>
2. <span data-ttu-id="6b0b8-128">Назначьте книги амортизации основных средств новым основным средствам.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-128">Assign fixed asset depreciation books to the new fixed assets.</span></span> <span data-ttu-id="6b0b8-129">Дополнительные сведения см. в разделе [Практическое руководство. Приобретение основных средств](fa-how-acquire.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b8-129">For more information, see [How to: Acquire Fixed Assets](fa-how-acquire.md).</span></span>
3. <span data-ttu-id="6b0b8-130">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы реклассификации ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Reclass. Journals**, and then choose the related link.</span></span>
4. <span data-ttu-id="6b0b8-131">Создайте две строки журнала реклассификации, по одной для каждого нового основного средства.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-131">Create two reclassification journal lines, one for each new fixed asset.</span></span>
5. <span data-ttu-id="6b0b8-132">В первой строке введите второе основное средство в поле **Новый номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-132">On the first line, enter the second fixed asset in the **New FA No.**</span></span> <span data-ttu-id="6b0b8-133">и 25 — в поле **Реклассиф. стоим. приобретения (%)**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-133">field and 25 in the **Reclassify Acq. Cost %** field.</span></span>
6. <span data-ttu-id="6b0b8-134">Во второй строке введите третье основное средство в поле **Новый номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-134">On the second line, enter the third fixed asset in the **New FA No.**</span></span> <span data-ttu-id="6b0b8-135">и 40 — в поле **Реклассиф. стоим. приобретения (%)**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-135">field and 40 in the **Reclassify Acq. Cost %** field.</span></span>
7. <span data-ttu-id="6b0b8-136">В обеих строках установите флажки **Реклассиф. стоимости приобретения** и **Реклассиф. амортизации**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-136">On both lines, select the **Reclassify Acquisition Cost** and **Reclassify Depreciation** check boxes.</span></span>   
8. <span data-ttu-id="6b0b8-137">Выберите действие **Реклассиф.**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-137">Choose the **Reclassify** action.</span></span>

    <span data-ttu-id="6b0b8-138">Создаются две строки в журнале ГК учета основных средств, используя шаблон и раздел, указанные в окне **ОС - настройка журнала** для указанной книги амортизации.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-138">Two lines are now created in the fixed asset G/L journal using the template and batch that you have specified in the **FA Journal Setup** window for the specified depreciation book.</span></span> <span data-ttu-id="6b0b8-139">Дополнительные сведения см. в разделе [Практическое руководство. Настройка амортизации основных средств](fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b8-139">For more information, see [How to: Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md).</span></span>    
9. <span data-ttu-id="6b0b8-140">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы ГК ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-140">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>
10. <span data-ttu-id="6b0b8-141">В окне **Журнал ГК учета основных средств** выберите действие **Учесть**, чтобы учесть реклассификацию, выполненную в шагах с 4 по 8.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-141">In the **Fixed Asset G/L Journal** window, choose the **Post** action to post the reclassification that you performed in steps 4 through 8.</span></span>

## <a name="to-combine-two-fixed-assets-into-one"></a><span data-ttu-id="6b0b8-142">Объединение двух основных средств в одно</span><span class="sxs-lookup"><span data-stu-id="6b0b8-142">To combine two fixed assets into one</span></span>
<span data-ttu-id="6b0b8-143">Можно объединить несколько основных средств в одно основное средство, например при перемещении распределенных основных средств в одно подразделение.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-143">You can combine multiple fixed assets into one fixed asset, for example when you move distributed fixed assets into one department.</span></span> <span data-ttu-id="6b0b8-144">Если произведен учет стоимости приобретения и амортизации для основного средства, которое необходимо переместить, эти значения будут объединены в одном основном средстве.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-144">If you have posted acquisition costs and depreciation for the fixed asset to be moved, those values will be combined in the single fixed asset.</span></span>

1. <span data-ttu-id="6b0b8-145">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы реклассификации ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="6b0b8-146">Создайте журнал реклассификации, где поле **Номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-146">Create a reclassification journal where the **FA No.**</span></span> <span data-ttu-id="6b0b8-147">поле содержит перемещаемое или объединяемое основное средство, а поле **Новый номер ОС**</span><span class="sxs-lookup"><span data-stu-id="6b0b8-147">field contains the fixed asset to be moved/combined, and the **New FA No.**</span></span> <span data-ttu-id="6b0b8-148">содержит основное средство. с которым производится объединение.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-148">field contains the fixed asset that it will be combined with.</span></span>
3. <span data-ttu-id="6b0b8-149">Оставьте поле **Реклассиф. стоим. приобретения (%)** пустым, чтобы переместить или объединить всю стоимость приобретения.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-149">Leave the **Reclassify Acq. Cost %** field empty to move/combine the entire acquisition cost.</span></span>    
4. <span data-ttu-id="6b0b8-150">Установите флажки **Реклассиф. стоимости приобретения** и **Реклассиф. амортизации**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-150">Select the **Reclassify Acquisition Cost** and **Reclassify Depreciation** check boxes.</span></span>
5. <span data-ttu-id="6b0b8-151">На вкладке **Действия** выберите **Реклассифицировать**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-151">On the **Actions** tab, choose **Reclassify**.</span></span>

    <span data-ttu-id="6b0b8-152">Создаются две строки в журнале ГК учета основных средств, используя шаблон и раздел, указанные в окне **ОС - настройка журнала** для указанной книги амортизации.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-152">Two lines are now created in the fixed asset G/L journal using the template and batch that you have specified in the **FA Journal Setup** window for the specified depreciation book.</span></span> <span data-ttu-id="6b0b8-153">Дополнительные сведения см. в разделе [Практическое руководство. Настройка амортизации основных средств](fa-how-setup-depreciation.md).</span><span class="sxs-lookup"><span data-stu-id="6b0b8-153">For more information, see [How to: Set Up Fixed Asset Depreciation](fa-how-setup-depreciation.md).</span></span>   
6. <span data-ttu-id="6b0b8-154">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы ГК ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-154">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>
7. <span data-ttu-id="6b0b8-155">В окне **Журнал ГК учета основных средств** выберите действие **Учесть**, чтобы учесть реклассификацию, выполненную в шагах с 2 по 5.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-155">In the **Fixed Asset G/L Journal** window, choose the **Post** action to post the reclassification that you performed in steps 2 through 5.</span></span>

## <a name="to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification"></a><span data-ttu-id="6b0b8-156">Просмотр балансовых значений амортизации, измененных из-за реклассификации основных средств</span><span class="sxs-lookup"><span data-stu-id="6b0b8-156">To view changed depreciation book values due to fixed asset reclassification</span></span>
1. <span data-ttu-id="6b0b8-157">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **ОС - балансовая стоимость 02**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-157">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA Book Value 02**, and then choose the related link.</span></span>
2. <span data-ttu-id="6b0b8-158">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-158">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="6b0b8-159">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="6b0b8-159">Choose the **Print** or **Preview** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6b0b8-160">См. также</span><span class="sxs-lookup"><span data-stu-id="6b0b8-160">See Also</span></span>
[<span data-ttu-id="6b0b8-161">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="6b0b8-161">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="6b0b8-162">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="6b0b8-162">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="6b0b8-163">Финансы</span><span class="sxs-lookup"><span data-stu-id="6b0b8-163">Finance</span></span>](finance.md)  
<span data-ttu-id="6b0b8-164">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="6b0b8-164">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="6b0b8-165">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6b0b8-165">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
