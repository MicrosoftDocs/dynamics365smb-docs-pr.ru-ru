---
title: Анализ фактических сумм в сравнении с бюджетом | Документация Майкрософт
description: Далее описывается порядок анализа фактических сумм в с равнении с суммами бюджета.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9c601dc3507b0777f3aeecb063e6cebe8866768c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781126"
---
# <a name="analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="be2f9-103">Анализ фактических сумм в с равнении с суммами бюджета</span><span class="sxs-lookup"><span data-stu-id="be2f9-103">Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="be2f9-104">В процессе сбора, анализа и предоставления доступа к данным своей организации вы просматриваете фактические суммы в сравнении с суммами бюджета для всех счетов и для различных периодов.</span><span class="sxs-lookup"><span data-stu-id="be2f9-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="be2f9-105">Чтобы проанализировать суммы бюджетов, сначала нужно создать бюджеты ГК.</span><span class="sxs-lookup"><span data-stu-id="be2f9-105">To analyze budgeted amounts, you must first create G(L budgets.</span></span> <span data-ttu-id="be2f9-106">Дополнительные сведения см. в разделе [Создание бюджетов ГК](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="be2f9-106">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="to-view-a-gl-budget"></a><span data-ttu-id="be2f9-107">Просмотр бюджета ГК</span><span class="sxs-lookup"><span data-stu-id="be2f9-107">To view a G/L budget</span></span>
<span data-ttu-id="be2f9-108">Для бюджета с измерениями операции можно фильтровать и просматривать конкретные бюджеты.</span><span class="sxs-lookup"><span data-stu-id="be2f9-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="be2f9-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Бюджеты ГК**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="be2f9-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="be2f9-110">На странице **Бюджеты ГК** откройте бюджет, который требуется посмотреть.</span><span class="sxs-lookup"><span data-stu-id="be2f9-110">On the **G/L Budgets** page, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="be2f9-111">В верхней части страницы заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="be2f9-111">At the top of the page, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="be2f9-112">Если выбрано значение **Период** в поле **Показывать в строках** или **Показывать в столбцах**, необходимо заполнить поле **Просмотр по**.</span><span class="sxs-lookup"><span data-stu-id="be2f9-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="be2f9-113">Если значение **Период** в полях **Показывать в строках** или **Показывать в столбцах** не выбрано, тогда необходимо ввести соответствующий период в поле **Фильтр по дате**.</span><span class="sxs-lookup"><span data-stu-id="be2f9-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="be2f9-114">В расчет будут включены только те операции бюджета Главной книги, для которых на экспресс-вкладке **Фильтры** были указаны коды фильтра.</span><span class="sxs-lookup"><span data-stu-id="be2f9-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="be2f9-115">Операции бюджетирования с другими кодами фильтра либо без них включаться в расчет не будут.</span><span class="sxs-lookup"><span data-stu-id="be2f9-115">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="be2f9-116">Пока на странице стоит фильтр, бюджет отражает только операции с кодами фильтра.</span><span class="sxs-lookup"><span data-stu-id="be2f9-116">As long as the filter remains on the page, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="be2f9-117">Если требуется изменить бюджет, можно изменить операции бюджетирования.</span><span class="sxs-lookup"><span data-stu-id="be2f9-117">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="be2f9-118">Выберите сумму для просмотра базовых операций бюджета Главной книги.</span><span class="sxs-lookup"><span data-stu-id="be2f9-118">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="be2f9-119">Просмотр фактических сумм и сумм бюджета по всем счетам</span><span class="sxs-lookup"><span data-stu-id="be2f9-119">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="be2f9-120">Бюджеты главной книги и их сравнение с фактическими цифрами можно просмотреть в разных областях [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="be2f9-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

1. <span data-ttu-id="be2f9-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **План счетов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="be2f9-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="be2f9-122">На странице **План счетов** выберите действие **Сальдо/бюджет ГК**.</span><span class="sxs-lookup"><span data-stu-id="be2f9-122">On the **Chart of Accounts** page, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="be2f9-123">В верхней части страницы заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="be2f9-123">At the top of the page, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="be2f9-124">Чтобы просмотреть спецификацию, формирующую показанную сумму, выберите поле.</span><span class="sxs-lookup"><span data-stu-id="be2f9-124">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="be2f9-125">Фильтры, настроенные в верхней части страницы, применяются к операциям главной книги и к бюджетным операциям.</span><span class="sxs-lookup"><span data-stu-id="be2f9-125">The filters you set on the page header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="be2f9-126">В столбцах слева содержится план счетов.</span><span class="sxs-lookup"><span data-stu-id="be2f9-126">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="be2f9-127">Из пяти столбцов в крайней справа части, первые четыре показывают для каждого счета фактические и бюджетные суммы по дебету и по кредиту.</span><span class="sxs-lookup"><span data-stu-id="be2f9-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="be2f9-128">В пятом столбце показано соотношение между фактическими и бюджетными суммами для счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="be2f9-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="be2f9-129">Используйте поле **Просмотр как** на странице **Сальдо/бюджет ГК** для выбора продолжительности периода.</span><span class="sxs-lookup"><span data-stu-id="be2f9-129">Use the **View by** field on the **G/L Balance/Budget** page to select the period length.</span></span> <span data-ttu-id="be2f9-130">Используйте поле **Просмотр как** для выбора способа подсчета сумм: **Оборот** или **Сальдо на дату**.</span><span class="sxs-lookup"><span data-stu-id="be2f9-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="be2f9-131">Выберите действие **Предыдущий период** или **Следующий период**, чтобы изменить период.</span><span class="sxs-lookup"><span data-stu-id="be2f9-131">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="be2f9-132">Просмотр фактических сумм и сумм бюджета по нескольким периодам</span><span class="sxs-lookup"><span data-stu-id="be2f9-132">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="be2f9-133">Вместо просмотра фактических и бюджетных сумм по всем счетам в рамках одного периода, можно просмотреть данные по одному счету для нескольких периодов.</span><span class="sxs-lookup"><span data-stu-id="be2f9-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="be2f9-134">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **План счетов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="be2f9-134">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="be2f9-135">На странице **План счетов**, выберите соответствующий счет главной книги, а затем действие **Сальдо/бюджет по счету ГК**.</span><span class="sxs-lookup"><span data-stu-id="be2f9-135">On the **Chart of Accounts** page, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="be2f9-136">В верхней части страницы заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="be2f9-136">At the top of the page, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="be2f9-137">Чтобы просмотреть спецификацию показанной суммы, выберите поле.</span><span class="sxs-lookup"><span data-stu-id="be2f9-137">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="be2f9-138">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/budgets-exchange-rates-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="be2f9-138">See Related Training at [Microsoft Learn](/learn/modules/budgets-exchange-rates-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="be2f9-139">См. также</span><span class="sxs-lookup"><span data-stu-id="be2f9-139">See Also</span></span>
[<span data-ttu-id="be2f9-140">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="be2f9-140">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="be2f9-141">Работа с финансовыми отчетами</span><span class="sxs-lookup"><span data-stu-id="be2f9-141">Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
[<span data-ttu-id="be2f9-142">Финансы</span><span class="sxs-lookup"><span data-stu-id="be2f9-142">Finance</span></span>](finance.md)  
[<span data-ttu-id="be2f9-143">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="be2f9-143">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="be2f9-144">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="be2f9-144">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="be2f9-145">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="be2f9-145">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]