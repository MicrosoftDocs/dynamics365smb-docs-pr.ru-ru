---
title: "Обзор задач по распределению затрат и доходов | Документы Майкрософт"
description: "Описание задач по распределению операции финансового журнала по нескольким разным счетам при учете журнала."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/07/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 1620e69ce8018256780dcba108c31312c02166cb
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-allocate-costs-and-income"></a><span data-ttu-id="52576-103">Практическое руководство. Распределение затрат и дохода</span><span class="sxs-lookup"><span data-stu-id="52576-103">How to: Allocate Costs and Income</span></span>
<span data-ttu-id="52576-104">При учете журнала операцию финансового журнала можно распределить по нескольким разным счетам.</span><span class="sxs-lookup"><span data-stu-id="52576-104">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="52576-105">Для распределения можно воспользоваться тремя методами:</span><span class="sxs-lookup"><span data-stu-id="52576-105">The allocation can be made by three different methods:</span></span>

* <span data-ttu-id="52576-106">количество;</span><span class="sxs-lookup"><span data-stu-id="52576-106">Quantity</span></span>
* <span data-ttu-id="52576-107">процент (%);</span><span class="sxs-lookup"><span data-stu-id="52576-107">Percentage (%)</span></span>
* <span data-ttu-id="52576-108">Сумма</span><span class="sxs-lookup"><span data-stu-id="52576-108">Amount</span></span>

<span data-ttu-id="52576-109">Функция распределения может использоваться с типовыми финансовыми журналами и в журналах основных средств.</span><span class="sxs-lookup"><span data-stu-id="52576-109">The allocation features can be used with recurring general journals and in fixed assets journals.</span></span>
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

<span data-ttu-id="52576-110">Далее описана процедура подготовки к распределению затрат в типовом финансовом журнале путем определения ключей распределения.</span><span class="sxs-lookup"><span data-stu-id="52576-110">The following procedures describe how to prepare to allocate costs in a recurring general journal by defining allocation keys.</span></span> <span data-ttu-id="52576-111">После определения ключей распределения вы выполняете и учитываете журнал как любой другой типовой финансовый журнал.</span><span class="sxs-lookup"><span data-stu-id="52576-111">When allocation keys are defined, you complete and post the journal like any other recurring general journal.</span></span> <span data-ttu-id="52576-112">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="52576-112">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="52576-113">Настройка ключей распределения</span><span class="sxs-lookup"><span data-stu-id="52576-113">To set up allocation keys</span></span>
<span data-ttu-id="52576-114">При учете журнала операцию типового финансового журнала можно распределить по нескольким разным счетам.</span><span class="sxs-lookup"><span data-stu-id="52576-114">You can allocate an entry in a recurring general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="52576-115">Распределение может выполняться по количеству, по процентному отношению или сумме.</span><span class="sxs-lookup"><span data-stu-id="52576-115">The allocation can be made by quantity, percentage, or amount.</span></span>
1. <span data-ttu-id="52576-116">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Типовой финансовый журнал**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="52576-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="52576-117">Выберите поле **Код раздела**, чтобы открыть окно **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="52576-117">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="52576-118">Вы можете изменить распределения в существующем разделе в списке или создать новый раздел с распределениями.</span><span class="sxs-lookup"><span data-stu-id="52576-118">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
   * <span data-ttu-id="52576-119">Для создания нового раздела выберите действие **Создать** и перейдите к следующему шагу.</span><span class="sxs-lookup"><span data-stu-id="52576-119">To create a new batch, choose the **New** action, and go to the next step.</span></span>
   * <span data-ttu-id="52576-120">Для изменения распределений в существующем журнале выберите журнал и перейдите к шагу 7.</span><span class="sxs-lookup"><span data-stu-id="52576-120">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="52576-121">В поле **Название** укажите название раздела, например CLEANING.</span><span class="sxs-lookup"><span data-stu-id="52576-121">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="52576-122">В поле **Описание** введите описание, например "Журнал для расходов по уборке".</span><span class="sxs-lookup"><span data-stu-id="52576-122">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="52576-123">По завершении закройте окно.</span><span class="sxs-lookup"><span data-stu-id="52576-123">When you are done, close the window.</span></span> <span data-ttu-id="52576-124">Откроется новый пустой типовой журнал.</span><span class="sxs-lookup"><span data-stu-id="52576-124">A new, empty recurring journal opens.</span></span>
6. <span data-ttu-id="52576-125">Заполните поля строки.</span><span class="sxs-lookup"><span data-stu-id="52576-125">Fill in the fields on the line.</span></span>
7. <span data-ttu-id="52576-126">Выберите действие **Распределения**.</span><span class="sxs-lookup"><span data-stu-id="52576-126">Choose the **Allocations** action.</span></span>
8. <span data-ttu-id="52576-127">Добавьте строку для каждого распределения.</span><span class="sxs-lookup"><span data-stu-id="52576-127">Add a line for each allocation.</span></span> <span data-ttu-id="52576-128">Следует по выбору заполнить поля **Распределение (%)**, **Распред. кол-во** или **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="52576-128">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="52576-129">Необходимо также заполнить поле **Номер счета**</span><span class="sxs-lookup"><span data-stu-id="52576-129">You must also fill in the **Account No.**</span></span> <span data-ttu-id="52576-130">и, если производится распределение транзакции по глобальным измерениям, поля глобального измерения.</span><span class="sxs-lookup"><span data-stu-id="52576-130">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="52576-131">Если в строке указан процент, сумма в поле **Сумма** будет рассчитана автоматически.</span><span class="sxs-lookup"><span data-stu-id="52576-131">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="52576-132">Эти суммы по знаку противоположны итоговой сумме из поля **Сумма** типового журнала.</span><span class="sxs-lookup"><span data-stu-id="52576-132">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="52576-133">После ввода строк распределения выберите **ОК**, чтобы вернуться к окну **Типовой финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="52576-133">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="52576-134">Поле **Распред. сумма (руб.)** будет заполнено и его значение будет соответствовать полю **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="52576-134">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="52576-135">Выполните учет журнала.</span><span class="sxs-lookup"><span data-stu-id="52576-135">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="52576-136">Изменение уже настроенного ключа распределения</span><span class="sxs-lookup"><span data-stu-id="52576-136">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="52576-137">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Типовой финансовый журнал**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="52576-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="52576-138">В окне **Типовой финансовый журнал** выберите журнал с распределением.</span><span class="sxs-lookup"><span data-stu-id="52576-138">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="52576-139">Выберите строку с распределением, а затем выберите действие **Распределения**.</span><span class="sxs-lookup"><span data-stu-id="52576-139">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="52576-140">Измените соответствующие поля и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="52576-140">Change the relevant fields, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="52576-141">См. также</span><span class="sxs-lookup"><span data-stu-id="52576-141">See Also</span></span>
[<span data-ttu-id="52576-142">Закрытие года и периодов</span><span class="sxs-lookup"><span data-stu-id="52576-142">Closing Years and Periods</span></span>](year-close-years-periods.md)  
<span data-ttu-id="52576-143">[Работа с финансовыми журналами](ui-work-general-journals.md)  </span><span class="sxs-lookup"><span data-stu-id="52576-143">[Working with General Journals](ui-work-general-journals.md)  </span></span>  
<span data-ttu-id="52576-144">[Учет документов и журналов](ui-post-documents-journals.md)  </span><span class="sxs-lookup"><span data-stu-id="52576-144">[Posting Documents and Journals](ui-post-documents-journals.md)  </span></span>  
<span data-ttu-id="52576-145">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="52576-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

