---
title: "Анализ фактических сумм в сравнении с бюджетом | Документы Майкрософт"
description: "Далее описывается порядок анализа фактических сумм в с равнении с суммами бюджета."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 12/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: cfe0eed4090ef458e774da8d0bc03910247570d7
ms.openlocfilehash: e76d590476b1236bf1d82a7f5e4f502ffdd9d02d
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="fe5f2-103">Практическое руководство. Анализ фактических сумм в с равнении с суммами бюджета</span><span class="sxs-lookup"><span data-stu-id="fe5f2-103">How to: Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="fe5f2-104">В процессе сбора, анализа и предоставления доступа к данным своей организации вы просматриваете фактические суммы в сравнении с суммами бюджета для всех счетов и для различных периодов.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="fe5f2-105">Чтобы проанализировать суммы бюджетов, сначала нужно создать бюджеты ГК.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-105">To analyze budgeted amounts, you must first create G(L budgets.</span></span> <span data-ttu-id="fe5f2-106">Дополнительные сведения см. в разделе [Практическое руководство. Создание бюджетов ГК](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="fe5f2-106">For more information, see [How to: Create G/L Budgets](finance-how-create-budgets.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="fe5f2-107">Для этой функциональности необходимо использовать вариант настройки интерфейса **Suite**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-107">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="fe5f2-108">Дополнительные сведения см. в разделе [Настройка интерфейса [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="fe5f2-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-view-a-gl-budget"></a><span data-ttu-id="fe5f2-109">Просмотр бюджета ГК</span><span class="sxs-lookup"><span data-stu-id="fe5f2-109">To view a G/L budget</span></span>
<span data-ttu-id="fe5f2-110">Для бюджета с измерениями операции можно фильтровать и просматривать конкретные бюджеты.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-110">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="fe5f2-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Бюджеты ГК**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="fe5f2-112">В окне **Бюджеты ГК** откройте бюджет, который требуется посмотреть.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-112">In the **G/L Budgets** window, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="fe5f2-113">В верхней части окна заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-113">At the top of the window, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="fe5f2-114">Если выбрано значение **Период** в поле **Показывать в строках** или **Показывать в столбцах**, необходимо заполнить поле **Просмотр по**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-114">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="fe5f2-115">Если значение **Период** в полях **Показывать в строках** или **Показывать в столбцах** не выбрано, тогда необходимо ввести соответствующий период в поле **Фильтр по дате**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-115">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="fe5f2-116">В расчет будут включены только те операции бюджета Главной книги, для которых на экспресс-вкладке **Фильтры** были указаны коды фильтра.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-116">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="fe5f2-117">Операции бюджетирования с другими кодами фильтра либо без них включаться в расчет не будут.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-117">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="fe5f2-118">Пока в окне стоит фильтр, бюджет отражает только операции с кодами фильтра.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-118">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="fe5f2-119">Если требуется изменить бюджет, можно изменить операции бюджетирования.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-119">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="fe5f2-120">Выберите сумму для просмотра базовых операций бюджета Главной книги.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-120">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="fe5f2-121">Просмотр фактических сумм и сумм бюджета по всем счетам</span><span class="sxs-lookup"><span data-stu-id="fe5f2-121">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="fe5f2-122">Бюджеты главной книги и их сравнение с фактическими цифрами можно просмотреть в разных областях [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="fe5f2-122">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="fe5f2-123">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **План счетов**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fe5f2-124">В окне **План счетов** выберите действие **Сальдо/бюджет ГК**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-124">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="fe5f2-125">В верхней части окна заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-125">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="fe5f2-126">Чтобы просмотреть спецификацию, формирующую показанную сумму, выберите поле.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-126">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="fe5f2-127">Фильтры, настроенные в верхней части окна, применяются к операциям главной книги и к бюджетным операциям.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-127">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="fe5f2-128">В столбцах слева содержится план счетов.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-128">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="fe5f2-129">Из пяти столбцов в крайней справа части, первые четыре показывают для каждого счета фактические и бюджетные суммы по дебету и по кредиту.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-129">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="fe5f2-130">В пятом столбце показано соотношение между фактическими и бюджетными суммами для счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-130">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="fe5f2-131">Используйте поле **Просмотр как** в окне **Сальдо/бюджет ГК** для выбора продолжительности периода.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-131">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span></span> <span data-ttu-id="fe5f2-132">Используйте поле **Просмотр как** для выбора способа подсчета сумм: **Оборот** или **Сальдо на дату**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-132">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="fe5f2-133">Выберите действие **Предыдущий период** или **Следующий период**, чтобы изменить период.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-133">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="fe5f2-134">Просмотр фактических сумм и сумм бюджета по нескольким периодам</span><span class="sxs-lookup"><span data-stu-id="fe5f2-134">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="fe5f2-135">Вместо просмотра фактических и бюджетных сумм по всем счетам в рамках одного периода, можно просмотреть данные по одному счету для нескольких периодов.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-135">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="fe5f2-136">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **План счетов**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fe5f2-137">В окне **План счетов**, выберите соответствующий счет главной книги, а затем действие **Сальдо/бюджет по счету ГК**.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-137">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="fe5f2-138">В верхней части окна заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-138">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="fe5f2-139">Чтобы просмотреть спецификацию показанной суммы, выберите поле.</span><span class="sxs-lookup"><span data-stu-id="fe5f2-139">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fe5f2-140">См. также</span><span class="sxs-lookup"><span data-stu-id="fe5f2-140">See Also</span></span>
[<span data-ttu-id="fe5f2-141">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="fe5f2-141">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="fe5f2-142">Практическое руководство. Работа с финансовыми отчетами</span><span class="sxs-lookup"><span data-stu-id="fe5f2-142">How to: Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
[<span data-ttu-id="fe5f2-143">Финансы</span><span class="sxs-lookup"><span data-stu-id="fe5f2-143">Finance</span></span>](finance.md)  
[<span data-ttu-id="fe5f2-144">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="fe5f2-144">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="fe5f2-145">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="fe5f2-145">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="fe5f2-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fe5f2-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

