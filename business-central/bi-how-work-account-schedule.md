---
title: "Построение финансовых отчетов"
description: "Описывается использование финансовых отчетов для создания различных представлений и отчетности для анализа данных о финансовых результатах."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 10/01/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 8e63e507411f41c67caa94834f4d99861bd1ae77
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="prepare-financial-reporting-with-account-schedules-and-account-categories"></a><span data-ttu-id="88152-103">Подготовка финансовой отчетности с помощью финансовых отчетов и категорий счетов</span><span class="sxs-lookup"><span data-stu-id="88152-103">Prepare Financial Reporting with Account Schedules and Account Categories</span></span>
<span data-ttu-id="88152-104">Используйте финансовые отчеты для получения сведений о финансовых данных, сохраненных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="88152-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span></span> <span data-ttu-id="88152-105">Финансовые отчеты анализируют цифры на счетах главной книги и сравнивают операции главной книги с операциями бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="88152-105">Account schedules analyze figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="88152-106">Результаты отображаются на диаграммах в ролевом центре, таких как диаграмма движения денежных средств, а также в отчетах, например в отчете о прибылях и убытках или балансовом отчете.</span><span class="sxs-lookup"><span data-stu-id="88152-106">The results display in charts on your Role Center, such as the Cash Flow chart, and in reports, such as the Income Statement and the Balance Sheet reports.</span></span>

<span data-ttu-id="88152-107">Для доступа к этим отчетам можно использовать действие **Финансовые отчеты** ролевых центров "Бизнес-руководитель" и "Бухгалтер".</span><span class="sxs-lookup"><span data-stu-id="88152-107">You access these two reports, for example, with the **Financials Statements** action on the Business Manager and Accountant Role Centers.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="88152-108">обеспечивает несколько примеров финансовых отчетов, которые можно использовать сразу же, либо можно настроить собственные строки и столбцы для указания цифр для сравнения.</span><span class="sxs-lookup"><span data-stu-id="88152-108">provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span></span> <span data-ttu-id="88152-109">Например, вы можете создавать финансовые отчеты для вычисления размеров прибыли по таким измерениям, как подразделения или группы клиентов.</span><span class="sxs-lookup"><span data-stu-id="88152-109">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span></span> <span data-ttu-id="88152-110">Можно создать столько пользовательских финансовых отчетов, сколько нужно.</span><span class="sxs-lookup"><span data-stu-id="88152-110">You can create as many customized financial statements as you want.</span></span>  

<span data-ttu-id="88152-111">Настройка финансовых отчетов требует понимания финансовых данных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="88152-111">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span></span> <span data-ttu-id="88152-112">Например, можно рассматривать операции главной книги как процент от бюджетных операций.</span><span class="sxs-lookup"><span data-stu-id="88152-112">For example, you can view general ledger entries as percentages of budget entries.</span></span> <span data-ttu-id="88152-113">Для этого необходимо создать бюджеты.</span><span class="sxs-lookup"><span data-stu-id="88152-113">This requires that budgets are created.</span></span> <span data-ttu-id="88152-114">Дополнительные сведения см. в разделе [Создание бюджетов ГК](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="88152-114">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="account-categories-and-account-schedules"></a><span data-ttu-id="88152-115">Категории счетов и финансовые отчеты</span><span class="sxs-lookup"><span data-stu-id="88152-115">Account Categories and Account Schedules</span></span>
<span data-ttu-id="88152-116">Дл изменения макетов финансовых отчетов можно использовать категории счетов.</span><span class="sxs-lookup"><span data-stu-id="88152-116">You can use account categories to change the layout of your financial statements.</span></span> <span data-ttu-id="88152-117">После настройки категорий счетов в окне **Категории счетов ГК** и выбора действия **Создать финансовые отчеты** соответствующие финансовые отчеты для основных финансовых отчетов будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="88152-117">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span></span> <span data-ttu-id="88152-118">При следующем выполнении одного из этих отчетов, например балансового отчета, будут добавлены новые итоговые значения и вложенные операции на основании внесенных изменений.</span><span class="sxs-lookup"><span data-stu-id="88152-118">The next time you run one of these reports, such as the Balance Statement report, new totals and subentries are added, based on your changes.</span></span> <span data-ttu-id="88152-119">Дополнительные сведения см. в подразделе "Категории счетов" раздела [Принципы работы с главной книгой и планом счетов](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="88152-119">For more information, see The "Account Categories" section in [Understanding the General Ledger and the COA](finance-general-ledger.md).</span></span>  

## <a name="to-create-new-account-schedules"></a><span data-ttu-id="88152-120">Создание новых финансовых отчетов</span><span class="sxs-lookup"><span data-stu-id="88152-120">To create new account schedules</span></span>  
 <span data-ttu-id="88152-121">Использование финансовых отчетов для анализа числовых значений на счетах главной книги или для сравнения операций главной книги с операциями бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="88152-121">You use account schedules to analyze figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="88152-122">Например, можно рассматривать операции ГК как процент от бюджетных операций.</span><span class="sxs-lookup"><span data-stu-id="88152-122">For example, you can view the general ledger entries as percentages of the budget entries.</span></span>

1. <span data-ttu-id="88152-123">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые отчеты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="88152-123">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2. <span data-ttu-id="88152-124">В окне **Названия финансовых отчетов** на выберите действие **Создать**, чтобы создать новое название финансового отчета.</span><span class="sxs-lookup"><span data-stu-id="88152-124">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span></span>
3. <span data-ttu-id="88152-125">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="88152-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="88152-126">Выберите действие **Изменение финансового отчета**.</span><span class="sxs-lookup"><span data-stu-id="88152-126">Choose the **Edit Account Schedule** action.</span></span>
5. <span data-ttu-id="88152-127">В окне **Финансовый отчет** заполните все поля соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="88152-127">In the **Account Schedule** window, fill in the fields as necessary.</span></span>  

    <span data-ttu-id="88152-128">После создания нового финансового отчета и настройки строк следует настроить столбцы.</span><span class="sxs-lookup"><span data-stu-id="88152-128">When you have created a new account schedule and set up the rows, you must set up columns.</span></span> <span data-ttu-id="88152-129">Настройку можно производить либо вручную, либо предварительно задать для финансового отчета раскладку столбцов.</span><span class="sxs-lookup"><span data-stu-id="88152-129">You can either set them up manually or assign a predefined column layout to your account schedule.</span></span>
6. <span data-ttu-id="88152-130">Выберите действие **Изменить настройку макета столбца**.</span><span class="sxs-lookup"><span data-stu-id="88152-130">Choose the **Edit Column Layout Setup** action.</span></span>
7. <span data-ttu-id="88152-131">В окне **Раскладка столбцов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="88152-131">In the **Column Layout** window, fill in the fields as necessary.</span></span>

> [!NOTE]  
> <span data-ttu-id="88152-132">Если финансовому отчету не назначена используемая по умолчанию раскладка столбцов, необходимо настроить столбцы вручную.</span><span class="sxs-lookup"><span data-stu-id="88152-132">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span></span>

### <a name="to-copy-an-existing-account-schedule"></a><span data-ttu-id="88152-133">Копирование существующего финансового отчета</span><span class="sxs-lookup"><span data-stu-id="88152-133">To copy an existing account schedule</span></span>
<span data-ttu-id="88152-134">Финансовые отчеты в стандартной версии [!INCLUDE[d365fin](includes/d365fin_md.md)] лежат в основе стандартных финансовых отчетов, которые могут не соответствовать потребностям вашей компании.</span><span class="sxs-lookup"><span data-stu-id="88152-134">The account schedules in the standard version of [!INCLUDE[d365fin](includes/d365fin_md.md)] are the basis of the standard financial reports, which may not suit the needs of your business.</span></span> <span data-ttu-id="88152-135">Чтобы быстро создать собственный финансовый отчет, можно сначала скопировать имеющийся отчет.</span><span class="sxs-lookup"><span data-stu-id="88152-135">To quickly create your own financial reports, you can start by copying an existing account schedule.</span></span>
1. <span data-ttu-id="88152-136">В окне **Финансовые отчеты** выберите отчет, а затем действие **Копировать финансовый отчет**.</span><span class="sxs-lookup"><span data-stu-id="88152-136">In the **Account Schedules** window, select an account schedule, and then choose the **Copy Account Schedule** action.</span></span>
2. <span data-ttu-id="88152-137">В окне **Копирование финансового отчета** заполните поля по мере необходимости, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="88152-137">In the **Copy Account Schedule** window, fill in the fields as necessary, and then choose the **OK** button.</span></span>

### <a name="to-create-a-column-that-calculates-percentages"></a><span data-ttu-id="88152-138">Создание столбца для вычисления процентов</span><span class="sxs-lookup"><span data-stu-id="88152-138">To create a column that calculates percentages</span></span>  
<span data-ttu-id="88152-139">Иногда может возникать потребность включить столбец в финансовый отчет для расчета процентов по итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="88152-139">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span></span> <span data-ttu-id="88152-140">Например, если имеется несколько строк, разбивающих продажи по измерениям, может потребоваться столбец с указанием процента от общих продаж для каждой строки.</span><span class="sxs-lookup"><span data-stu-id="88152-140">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span></span>

1. <span data-ttu-id="88152-141">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые отчеты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="88152-141">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="88152-142">В окне **Названия финансовых отчетов** выберите финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="88152-142">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="88152-143">Выберите действие **Изменение финансового отчета**, чтобы настроить строку финансового отчета для вычисления общей суммы, на которой будет основан процент.</span><span class="sxs-lookup"><span data-stu-id="88152-143">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span></span>  
4. <span data-ttu-id="88152-144">Вставьте строку непосредственно перед первой строкой, для которой необходимо отобразить проценты.</span><span class="sxs-lookup"><span data-stu-id="88152-144">Insert a line immediately above the first row for which you want to display a percentage.</span></span>  
5. <span data-ttu-id="88152-145">Заполните поля в строке следующим образом: В поле **Тип группировки** укажите **Задать базу для процентов**.</span><span class="sxs-lookup"><span data-stu-id="88152-145">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span></span> <span data-ttu-id="88152-146">В поле **Подсчет итога** введите формулу для итога, на которой будет основан расчет процента.</span><span class="sxs-lookup"><span data-stu-id="88152-146">In the **Totaling** field, enter a formula for the total that the percentage will be based on.</span></span> <span data-ttu-id="88152-147">Например, если строка 11 показывает итоговые продажи, введите **11**.</span><span class="sxs-lookup"><span data-stu-id="88152-147">For example, if row 11 contains the total sales, enter **11**.</span></span>  
6. <span data-ttu-id="88152-148">Выберите действие **Изменить настройку макета столбца**.</span><span class="sxs-lookup"><span data-stu-id="88152-148">Choose the **Edit Column Layout Setup** action to set up a column.</span></span>  
7. <span data-ttu-id="88152-149">Заполните поля в строке следующим образом: В поле **Тип столбца** выберите **Формула**.</span><span class="sxs-lookup"><span data-stu-id="88152-149">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span></span> <span data-ttu-id="88152-150">В поле **Формула** введите формулу для суммы, для которой необходимо вычислить процент, добавив в конце символ %.</span><span class="sxs-lookup"><span data-stu-id="88152-150">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span></span> <span data-ttu-id="88152-151">Например, если столбец с номером N содержит чистое изменение, то введите **N%**.</span><span class="sxs-lookup"><span data-stu-id="88152-151">For example, if column number N contains the net change, enter **N%**.</span></span>  
8. <span data-ttu-id="88152-152">Повторите шаги с 4 по 7 для каждой группы строк, по которым требуется получить процент.</span><span class="sxs-lookup"><span data-stu-id="88152-152">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span></span>

## <a name="to-set-up-account-schedules-with-overviews"></a><span data-ttu-id="88152-153">Настройка финансовых отчетов с обзорами</span><span class="sxs-lookup"><span data-stu-id="88152-153">To set up account schedules with overviews</span></span>  
<span data-ttu-id="88152-154">Финансовый отчет можно использовать для создания отчета, содержащего сравнение цифр главной книги с цифрами бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="88152-154">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span></span>

1. <span data-ttu-id="88152-155">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые отчеты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="88152-155">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="88152-156">В окне **Названия финансовых отчетов** выберите финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="88152-156">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="88152-157">Выберите действие **Изменение финансового отчета**.</span><span class="sxs-lookup"><span data-stu-id="88152-157">Choose the **Edit Account Schedule** action</span></span>  
4. <span data-ttu-id="88152-158">В окне **Финансовый отчет** в поле **Имя** выберите название финансового графика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="88152-158">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span></span>
5. <span data-ttu-id="88152-159">Выберите действие **Вставить счета**.</span><span class="sxs-lookup"><span data-stu-id="88152-159">Choose the **Insert Accounts** action.</span></span>  
6. <span data-ttu-id="88152-160">Выделите счета, по которым необходимо составить отчет, затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="88152-160">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span></span>

    <span data-ttu-id="88152-161">Теперь счета вставлены в финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="88152-161">The accounts are now inserted into your account schedule.</span></span> <span data-ttu-id="88152-162">При желании можно изменить также раскладку столбцов.</span><span class="sxs-lookup"><span data-stu-id="88152-162">If you want you can also change the column layout.</span></span>  
7. <span data-ttu-id="88152-163">Выберите действие **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="88152-163">Choose the **Overview** action.</span></span>  
8. <span data-ttu-id="88152-164">На экспресс-вкладке **Фильтры измерения** задайте фильтр по бюджету с требуемым названием фильтра.</span><span class="sxs-lookup"><span data-stu-id="88152-164">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span></span>  
9. <span data-ttu-id="88152-165">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="88152-165">Choose the **OK** button.</span></span>  

<span data-ttu-id="88152-166">Теперь можно копировать и вставлять бюджетные отчеты в таблицу.</span><span class="sxs-lookup"><span data-stu-id="88152-166">Now you can copy and paste your budget statement into a spreadsheet.</span></span>  

## <a name="comparing-accounting-periods-using-period-formulas"></a><span data-ttu-id="88152-167">Сравнение учетных периодов с использованием формул периодов</span><span class="sxs-lookup"><span data-stu-id="88152-167">Comparing Accounting Periods using Period Formulas</span></span>
<span data-ttu-id="88152-168">В финансовом отчете можно сравнивать результаты различных финансовых периодов, например результаты за месяцы с результатами за тот же месяц прошлого года.</span><span class="sxs-lookup"><span data-stu-id="88152-168">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span></span> <span data-ttu-id="88152-169">Чтобы это сделать, нужно добавить столбец с полем **Формула периода сравнения**, а затем задать в этом поле формулу периода.</span><span class="sxs-lookup"><span data-stu-id="88152-169">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span></span>  

<span data-ttu-id="88152-170">Учетный период не обязательно должен совпадать с календарным, но все финансовые годы должны содержать одинаковое количество учетных периодов, даже если периоды могут различаться по длине.</span><span class="sxs-lookup"><span data-stu-id="88152-170">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="88152-171">использует формулу периода для расчета суммы из периода сравнения по отношению к периоду, представленному в фильтре дат запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="88152-171">uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span></span> <span data-ttu-id="88152-172">Период сравнения основан на периоде начальной даты из фильтра дат.</span><span class="sxs-lookup"><span data-stu-id="88152-172">The comparison period is based on the period of the start date of the date filter.</span></span> <span data-ttu-id="88152-173">Для обозначений периодов используются следующие сокращения.</span><span class="sxs-lookup"><span data-stu-id="88152-173">The abbreviations for period specifications are:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="88152-174">Сокращение</span><span class="sxs-lookup"><span data-stu-id="88152-174">Abbreviation</span></span></th>
<th><span data-ttu-id="88152-175">Описанием</span><span class="sxs-lookup"><span data-stu-id="88152-175">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="88152-176">П</span><span class="sxs-lookup"><span data-stu-id="88152-176">P</span></span></p></td>
<td><p><span data-ttu-id="88152-177">периодам</span><span class="sxs-lookup"><span data-stu-id="88152-177">Period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="88152-178">LP</span><span class="sxs-lookup"><span data-stu-id="88152-178">LP</span></span></p></td>
<td><p><span data-ttu-id="88152-179">Последний период финансового года, полугодия или квартала.</span><span class="sxs-lookup"><span data-stu-id="88152-179">Last period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="88152-180">CP</span><span class="sxs-lookup"><span data-stu-id="88152-180">CP</span></span></p></td>
<td><p><span data-ttu-id="88152-181">Текущий период финансового года, полугодия или квартала.</span><span class="sxs-lookup"><span data-stu-id="88152-181">Current period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="88152-182">FY</span><span class="sxs-lookup"><span data-stu-id="88152-182">FY</span></span></p></td>
<td><p><span data-ttu-id="88152-183">Финансовый год.</span><span class="sxs-lookup"><span data-stu-id="88152-183">Fiscal year.</span></span> <span data-ttu-id="88152-184">Например, FY[1..3] обозначает первый квартал текущего финансового года.</span><span class="sxs-lookup"><span data-stu-id="88152-184">For example, FY[1..3] denotes first quarter of the current fiscal year</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="88152-185">Примеры формул:</span><span class="sxs-lookup"><span data-stu-id="88152-185">Examples of formulas:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="88152-186">Формула</span><span class="sxs-lookup"><span data-stu-id="88152-186">Formula</span></span></th>
<th><span data-ttu-id="88152-187">Описанием</span><span class="sxs-lookup"><span data-stu-id="88152-187">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="88152-188">&lt;Пусто&gt;</span><span class="sxs-lookup"><span data-stu-id="88152-188">&lt;Blank&gt;</span></span></p></td>
<td><p><span data-ttu-id="88152-189">Текущий период.</span><span class="sxs-lookup"><span data-stu-id="88152-189">Current period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="88152-190">-1P</span><span class="sxs-lookup"><span data-stu-id="88152-190">-1P</span></span></p></td>
<td><p><span data-ttu-id="88152-191">Предыдущий период.</span><span class="sxs-lookup"><span data-stu-id="88152-191">Previous period</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="88152-192">-1FY[1..LP]</span><span class="sxs-lookup"><span data-stu-id="88152-192">-1FY[1..LP]</span></span></p></td>
<td><p><span data-ttu-id="88152-193">Весь предыдущий финансовый год</span><span class="sxs-lookup"><span data-stu-id="88152-193">Entire previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="88152-194">-1FY</span><span class="sxs-lookup"><span data-stu-id="88152-194">-1FY</span></span></p></td>
<td><p><span data-ttu-id="88152-195">Текущий период предыдущего финансового года</span><span class="sxs-lookup"><span data-stu-id="88152-195">Current period in previous fiscal year</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="88152-196">-1FY[1..3]</span><span class="sxs-lookup"><span data-stu-id="88152-196">-1FY[1..3]</span></span></p></td>
<td><p><span data-ttu-id="88152-197">Первый квартал предыдущего финансового года.</span><span class="sxs-lookup"><span data-stu-id="88152-197">First quarter of previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="88152-198">-1ФГ[1..CP]</span><span class="sxs-lookup"><span data-stu-id="88152-198">-1FY[1..CP]</span></span></p></td>
<td><p><span data-ttu-id="88152-199">С начала предыдущего финансового года до текущего периода в предыдущем финансовом году, включительно</span><span class="sxs-lookup"><span data-stu-id="88152-199">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="88152-200">-1FY[CP..LP]</span><span class="sxs-lookup"><span data-stu-id="88152-200">-1FY[CP..LP]</span></span></p></td>
<td><p><span data-ttu-id="88152-201">С текущего периода в предыдущем финансовом году до последнего периода предыдущего финансового года, включительно</span><span class="sxs-lookup"><span data-stu-id="88152-201">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="88152-202">Если вычисления необходимо выполнять регулярно через заданный промежуток времени, вместо этого нужно ввести формулу в поле **Формула даты сравнения**.</span><span class="sxs-lookup"><span data-stu-id="88152-202">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span></span>

> [!NOTE]
> <span data-ttu-id="88152-203">Не всегда очевидно, какие периоды сравниваются, потому что вы можете установить в отчете фильтр по дате, который охватывает даты иные, нежели учетные периоды, отраженные в данных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="88152-203">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span></span> <span data-ttu-id="88152-204">Например, вы можете создать отчет для сравнения данного периода с тем же периодом в прошлом году, т. е. задать в поле **Фильтр по периоду даты сравнения** значение *-1ФГ*.</span><span class="sxs-lookup"><span data-stu-id="88152-204">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span></span> <span data-ttu-id="88152-205">После этого вы запускаете отчет 28 февраля и устанавливаете в качестве фильтра по дате январь и февраль.</span><span class="sxs-lookup"><span data-stu-id="88152-205">Then, you run the report on February 28th and set the date filter to January and February.</span></span> <span data-ttu-id="88152-206">В результате в отчете сравниваются январь и февраль этого года с январем прошлого года, которые представляет собой единственный завершенный учетный период из двух периодов за прошлый год.</span><span class="sxs-lookup"><span data-stu-id="88152-206">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span></span>  


## <a name="see-also"></a><span data-ttu-id="88152-207">См. также</span><span class="sxs-lookup"><span data-stu-id="88152-207">See Also</span></span>
[<span data-ttu-id="88152-208">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="88152-208">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="88152-209">Финансы</span><span class="sxs-lookup"><span data-stu-id="88152-209">Finance</span></span>](finance.md)  
[<span data-ttu-id="88152-210">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="88152-210">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="88152-211">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="88152-211">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="88152-212">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="88152-212">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

