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
ms.date: 04/16/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 7c346455a9e27d7274b116754f1d594484b95d67
ms.openlocfilehash: f9f5b3a25a24d4d10c80d048153e68030733bf9e
ms.contentlocale: ru-ru
ms.lasthandoff: 04/18/2018

---
# <a name="work-with-account-schedules"></a><span data-ttu-id="b2433-103">Работа с финансовыми отчетами</span><span class="sxs-lookup"><span data-stu-id="b2433-103">Work with Account Schedules</span></span>
<span data-ttu-id="b2433-104">Используйте финансовые отчеты для получения сведений о финансовых данных, сохраненных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="b2433-104">Use account schedules to get insight into the financial data stored in your chart of accounts.</span></span> <span data-ttu-id="b2433-105">Финансовые отчеты анализируют цифры на счетах главной книги и сравнивают операции главной книги с операциями бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="b2433-105">Account schedules analyze figures in G/L accounts, and compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="b2433-106">Результаты отображаются на диаграммах в ролевом центре, например на диаграмме "Движение денежных средств".</span><span class="sxs-lookup"><span data-stu-id="b2433-106">The results display in charts on your Role Center, such as the Cash Flow chart.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="b2433-107"> обеспечивает несколько примеров финансовых отчетов, которые можно использовать сразу же, либо можно настроить собственные строки и столбцы для указания цифр для сравнения.</span><span class="sxs-lookup"><span data-stu-id="b2433-107"> provides a few sample account schedules that you can use right away, or you can set up your own rows and columns to specify the figures to compare.</span></span> <span data-ttu-id="b2433-108">Например, вы можете создавать финансовые отчеты для вычисления размеров прибыли по таким измерениям, как подразделения или группы клиентов.</span><span class="sxs-lookup"><span data-stu-id="b2433-108">For example, you can create account schedules to calculate profit margins on dimensions like departments or customer groups.</span></span> <span data-ttu-id="b2433-109">Можно создать столько пользовательских финансовых отчетов, сколько нужно.</span><span class="sxs-lookup"><span data-stu-id="b2433-109">You can create as many customized financial statements as you want.</span></span>  

<span data-ttu-id="b2433-110">Настройка финансовых отчетов требует понимания финансовых данных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="b2433-110">Setting up account schedules requires an understanding of the financial data in the chart of accounts.</span></span> <span data-ttu-id="b2433-111">Например, можно рассматривать операции главной книги как процент от бюджетных операций.</span><span class="sxs-lookup"><span data-stu-id="b2433-111">For example, you can view general ledger entries as percentages of budget entries.</span></span> <span data-ttu-id="b2433-112">Для этого необходимо создать бюджеты.</span><span class="sxs-lookup"><span data-stu-id="b2433-112">This requires that budgets are created.</span></span> <span data-ttu-id="b2433-113">Дополнительные сведения см. в разделе [Создание бюджетов ГК](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="b2433-113">For more information, see [Create G/L Budgets](finance-how-create-budgets.md).</span></span>

## <a name="account-categories-and-account-schedules"></a><span data-ttu-id="b2433-114">Категории счетов и финансовые отчеты</span><span class="sxs-lookup"><span data-stu-id="b2433-114">Account Categories and Account Schedules</span></span>
<span data-ttu-id="b2433-115">Дл изменения макетов финансовых отчетов можно использовать категории счетов.</span><span class="sxs-lookup"><span data-stu-id="b2433-115">You can use account categories to change the layout of your financial statements.</span></span> <span data-ttu-id="b2433-116">После настройки категорий счетов в окне **Категории счетов ГК** и выбора действия **Создать финансовые отчеты** соответствующие финансовые отчеты для основных финансовых отчетов будут обновлены.</span><span class="sxs-lookup"><span data-stu-id="b2433-116">After you set up your account categories in the **G/L Account Categories** window, and you choose the **Generate Account Schedules** action, the underlying account schedules for the core financial reports are updated.</span></span> <span data-ttu-id="b2433-117">При следующем выполнении одного из этих отчетов, например балансового отчета, будут добавлены новые итоговые значения и вложенные операции на основании внесенных изменений.</span><span class="sxs-lookup"><span data-stu-id="b2433-117">The next time you run one of these reports, such as the balance statement, new totals and subentries are added, based on your changes.</span></span> <span data-ttu-id="b2433-118">Дополнительные сведения см. в разделе [Главная книга и план счетов](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="b2433-118">For more information, see [The General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>  

## <a name="to-create-new-account-schedules"></a><span data-ttu-id="b2433-119">Создание новых финансовых отчетов</span><span class="sxs-lookup"><span data-stu-id="b2433-119">To create new account schedules</span></span>  
 <span data-ttu-id="b2433-120">Использование финансовых отчетов для анализа числовых значений на счетах главной книги или для сравнения операций главной книги с операциями бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="b2433-120">You use account schedules to analyze figures in general ledger accounts or to compare general ledger entries with general ledger budget entries.</span></span> <span data-ttu-id="b2433-121">Например, можно рассматривать операции ГК как процент от бюджетных операций.</span><span class="sxs-lookup"><span data-stu-id="b2433-121">For example, you can view the general ledger entries as percentages of the budget entries.</span></span>

1. <span data-ttu-id="b2433-122">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовые отчеты**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b2433-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>  
2. <span data-ttu-id="b2433-123">В окне **Названия финансовых отчетов** на выберите действие **Создать**, чтобы создать новое название финансового отчета.</span><span class="sxs-lookup"><span data-stu-id="b2433-123">In the **Account Schedule Names** window, choose the **New** action to create a new account schedule name.</span></span>
3. <span data-ttu-id="b2433-124">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="b2433-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="b2433-125">Выберите действие **Изменение финансового отчета**.</span><span class="sxs-lookup"><span data-stu-id="b2433-125">Choose the **Edit Account Schedule** action.</span></span>
5. <span data-ttu-id="b2433-126">В окне **Финансовый отчет** заполните все поля соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="b2433-126">In the **Account Schedule** window, fill in the fields as necessary.</span></span>  

    <span data-ttu-id="b2433-127">После создания нового финансового отчета и настройки строк следует настроить столбцы.</span><span class="sxs-lookup"><span data-stu-id="b2433-127">When you have created a new account schedule and set up the rows, you must set up columns.</span></span> <span data-ttu-id="b2433-128">Настройку можно производить либо вручную, либо предварительно задать для финансового отчета раскладку столбцов.</span><span class="sxs-lookup"><span data-stu-id="b2433-128">You can either set them up manually or assign a predefined column layout to your account schedule.</span></span>
6. <span data-ttu-id="b2433-129">Выберите действие **Изменить настройку макета столбца**.</span><span class="sxs-lookup"><span data-stu-id="b2433-129">Choose the **Edit Column Layout Setup** action.</span></span>
7. <span data-ttu-id="b2433-130">В окне **Раскладка столбцов** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="b2433-130">In the **Column Layout** window, fill in the fields as necessary.</span></span>

> [!NOTE]  
>   <span data-ttu-id="b2433-131">Если финансовому отчету не назначена используемая по умолчанию раскладка столбцов, необходимо настроить столбцы вручную.</span><span class="sxs-lookup"><span data-stu-id="b2433-131">If you did not assign a default column layout to the account schedule, you must set the columns up manually.</span></span>   

### <a name="to-create-a-column-that-calculates-percentages"></a><span data-ttu-id="b2433-132">Создание столбца для вычисления процентов</span><span class="sxs-lookup"><span data-stu-id="b2433-132">To create a column that calculates percentages</span></span>  
<span data-ttu-id="b2433-133">Иногда может возникать потребность включить столбец в финансовый отчет для расчета процентов по итоговой сумме.</span><span class="sxs-lookup"><span data-stu-id="b2433-133">Sometimes you may want to include a column in an account schedule to calculate percentages of a total.</span></span> <span data-ttu-id="b2433-134">Например, если имеется несколько строк, разбивающих продажи по измерениям, может потребоваться столбец с указанием процента от общих продаж для каждой строки.</span><span class="sxs-lookup"><span data-stu-id="b2433-134">For example, if you have a number of rows that break down sales by dimension, you may want a column to indicate the percentage of total sales that each row represents.</span></span>

1. <span data-ttu-id="b2433-135">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовые отчеты**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b2433-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="b2433-136">В окне **Названия финансовых отчетов** выберите финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="b2433-136">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="b2433-137">Выберите действие **Изменение финансового отчета**, чтобы настроить строку финансового отчета для вычисления общей суммы, на которой будет основан процент.</span><span class="sxs-lookup"><span data-stu-id="b2433-137">Choose the **Edit Account Schedule** action to set up an account schedule row to calculate the total on which the percentages will be based.</span></span>  
4. <span data-ttu-id="b2433-138">Вставьте строку непосредственно перед первой строкой, для которой необходимо отобразить проценты.</span><span class="sxs-lookup"><span data-stu-id="b2433-138">Insert a line immediately above the first row for which you want to display a percentage.</span></span>  
5. <span data-ttu-id="b2433-139">Заполните поля в строке следующим образом: В поле **Тип группировки** укажите **Задать базу для процентов**.</span><span class="sxs-lookup"><span data-stu-id="b2433-139">Fill in the fields on the line as follows: In the **Totaling Type** field, enter **Set Base for Percent**.</span></span> <span data-ttu-id="b2433-140">В поле **Подсчет итога** введите формулу для итога, на которой будет основан расчет процента.</span><span class="sxs-lookup"><span data-stu-id="b2433-140">In the **Totaling** field, enter a formula for the total that the percentage will be based on.</span></span> <span data-ttu-id="b2433-141">Например, если строка 11 показывает итоговые продажи, введите **11**.</span><span class="sxs-lookup"><span data-stu-id="b2433-141">For example, if row 11 contains the total sales, enter **11**.</span></span>  
6. <span data-ttu-id="b2433-142">Выберите действие **Изменить настройку макета столбца**.</span><span class="sxs-lookup"><span data-stu-id="b2433-142">Choose the **Edit Column Layout Setup** action to set up a column.</span></span>  
7. <span data-ttu-id="b2433-143">Заполните поля в строке следующим образом: В поле **Тип столбца** выберите **Формула**.</span><span class="sxs-lookup"><span data-stu-id="b2433-143">Fill in the fields on the line as follows: In the **Column Type** field, select **Formula**.</span></span> <span data-ttu-id="b2433-144">В поле **Формула** введите формулу для суммы, для которой необходимо вычислить процент, добавив в конце символ %.</span><span class="sxs-lookup"><span data-stu-id="b2433-144">In the **Formula** field, enter a formula for the amount that you want to calculate a percentage for, followed by %.</span></span> <span data-ttu-id="b2433-145">Например, если столбец с номером N содержит чистое изменение, то введите **N%**.</span><span class="sxs-lookup"><span data-stu-id="b2433-145">For example, if column number N contains the net change, enter **N%**.</span></span>  
8. <span data-ttu-id="b2433-146">Повторите шаги с 4 по 7 для каждой группы строк, по которым требуется получить процент.</span><span class="sxs-lookup"><span data-stu-id="b2433-146">Repeat steps 4 through 7 for each group of rows that you want to break down by percentage.</span></span>

## <a name="to-set-up-account-schedules-with-overviews"></a><span data-ttu-id="b2433-147">Настройка финансовых отчетов с обзорами</span><span class="sxs-lookup"><span data-stu-id="b2433-147">To set up account schedules with overviews</span></span>  
<span data-ttu-id="b2433-148">Финансовый отчет можно использовать для создания отчета, содержащего сравнение цифр главной книги с цифрами бюджета главной книги.</span><span class="sxs-lookup"><span data-stu-id="b2433-148">You can use an account schedule to create a statement comparing general ledger figures and general leger budget figures.</span></span>

1. <span data-ttu-id="b2433-149">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовые отчеты**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b2433-149">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Account Schedules**, and then choose the related link.</span></span>
2. <span data-ttu-id="b2433-150">В окне **Названия финансовых отчетов** выберите финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="b2433-150">In the **Account Schedule Names** window, select an account schedule.</span></span>  
3. <span data-ttu-id="b2433-151">Выберите действие **Изменение финансового отчета**.</span><span class="sxs-lookup"><span data-stu-id="b2433-151">Choose the **Edit Account Schedule** action</span></span>  
4. <span data-ttu-id="b2433-152">В окне **Финансовый отчет** в поле **Имя** выберите название финансового графика по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b2433-152">In the **Account Schedule** window, in the **Name** field, select the default account schedule name.</span></span>
5. <span data-ttu-id="b2433-153">Выберите действие **Вставить счета**.</span><span class="sxs-lookup"><span data-stu-id="b2433-153">Choose the **Insert Accounts** action.</span></span>  
6. <span data-ttu-id="b2433-154">Выделите счета, по которым необходимо составить отчет, затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b2433-154">Select the accounts that you want to include in your statement, and then choose the **OK** button.</span></span>

    <span data-ttu-id="b2433-155">Теперь счета вставлены в финансовый отчет.</span><span class="sxs-lookup"><span data-stu-id="b2433-155">The accounts are now inserted into your account schedule.</span></span> <span data-ttu-id="b2433-156">При желании можно изменить также раскладку столбцов.</span><span class="sxs-lookup"><span data-stu-id="b2433-156">If you want you can also change the column layout.</span></span>  
7. <span data-ttu-id="b2433-157">Выберите действие **Обзор**.</span><span class="sxs-lookup"><span data-stu-id="b2433-157">Choose the **Overview** action.</span></span>  
8. <span data-ttu-id="b2433-158">На экспресс-вкладке **Фильтры измерения** задайте фильтр по бюджету с требуемым названием фильтра.</span><span class="sxs-lookup"><span data-stu-id="b2433-158">On the **Dimension Filters** FastTab, set the budget filter to the desired filter name.</span></span>  
9. <span data-ttu-id="b2433-159">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b2433-159">Choose the **OK** button.</span></span>  

<span data-ttu-id="b2433-160">Теперь можно копировать и вставлять бюджетные отчеты в таблицу.</span><span class="sxs-lookup"><span data-stu-id="b2433-160">Now you can copy and paste your budget statement into a spreadsheet.</span></span>  

## <a name="comparing-accounting-periods-using-period-formulas"></a><span data-ttu-id="b2433-161">Сравнение учетных периодов с использованием формул периодов</span><span class="sxs-lookup"><span data-stu-id="b2433-161">Comparing Accounting Periods using Period Formulas</span></span>
<span data-ttu-id="b2433-162">В финансовом отчете можно сравнивать результаты различных финансовых периодов, например результаты за месяцы с результатами за тот же месяц прошлого года.</span><span class="sxs-lookup"><span data-stu-id="b2433-162">Your account schedule can compare the results of different accounting periods, such as this month versus same month last year.</span></span> <span data-ttu-id="b2433-163">Чтобы это сделать, нужно добавить столбец с полем **Формула периода сравнения**, а затем задать в этом поле формулу периода.</span><span class="sxs-lookup"><span data-stu-id="b2433-163">To do that, you add a column with the **Comparison Period Formula** field, and then set that field to a period formula.</span></span>  

<span data-ttu-id="b2433-164">Учетный период не обязательно должен совпадать с календарным, но все финансовые годы должны содержать одинаковое количество учетных периодов, даже если периоды могут различаться по длине.</span><span class="sxs-lookup"><span data-stu-id="b2433-164">An accounting period does not have to match the calendar, but each fiscal year must have the same number of accounting periods, even though each period can be different in length.</span></span>   

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="b2433-165"> использует формулу периода для расчета суммы из периода сравнения по отношению к периоду, представленному в фильтре дат запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="b2433-165"> uses the period formula to calculate the amount from the comparison period in relation to the period represented by the date filter on the report request.</span></span> <span data-ttu-id="b2433-166">Период сравнения основан на периоде начальной даты из фильтра дат.</span><span class="sxs-lookup"><span data-stu-id="b2433-166">The comparison period is based on the period of the start date of the date filter.</span></span> <span data-ttu-id="b2433-167">Для обозначений периодов используются следующие сокращения.</span><span class="sxs-lookup"><span data-stu-id="b2433-167">The abbreviations for period specifications are:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b2433-168">Сокращение</span><span class="sxs-lookup"><span data-stu-id="b2433-168">Abbreviation</span></span></th>
<th><span data-ttu-id="b2433-169">Описанием</span><span class="sxs-lookup"><span data-stu-id="b2433-169">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="b2433-170">П</span><span class="sxs-lookup"><span data-stu-id="b2433-170">P</span></span></p></td>
<td><p><span data-ttu-id="b2433-171">периодам</span><span class="sxs-lookup"><span data-stu-id="b2433-171">Period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b2433-172">LP</span><span class="sxs-lookup"><span data-stu-id="b2433-172">LP</span></span></p></td>
<td><p><span data-ttu-id="b2433-173">Последний период финансового года, полугодия или квартала.</span><span class="sxs-lookup"><span data-stu-id="b2433-173">Last period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b2433-174">CP</span><span class="sxs-lookup"><span data-stu-id="b2433-174">CP</span></span></p></td>
<td><p><span data-ttu-id="b2433-175">Текущий период финансового года, полугодия или квартала.</span><span class="sxs-lookup"><span data-stu-id="b2433-175">Current period of a fiscal year, half-year or quarter.</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b2433-176">FY</span><span class="sxs-lookup"><span data-stu-id="b2433-176">FY</span></span></p></td>
<td><p><span data-ttu-id="b2433-177">Финансовый год.</span><span class="sxs-lookup"><span data-stu-id="b2433-177">Fiscal year.</span></span> <span data-ttu-id="b2433-178">Например, FY[1..3] обозначает первый квартал текущего финансового года.</span><span class="sxs-lookup"><span data-stu-id="b2433-178">For example, FY[1..3] denotes first quarter of the current fiscal year</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="b2433-179">Примеры формул:</span><span class="sxs-lookup"><span data-stu-id="b2433-179">Examples of formulas:</span></span>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b2433-180">Формула</span><span class="sxs-lookup"><span data-stu-id="b2433-180">Formula</span></span></th>
<th><span data-ttu-id="b2433-181">Описанием</span><span class="sxs-lookup"><span data-stu-id="b2433-181">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="b2433-182">&lt;Пусто&gt;</span><span class="sxs-lookup"><span data-stu-id="b2433-182">&lt;Blank&gt;</span></span></p></td>
<td><p><span data-ttu-id="b2433-183">Текущий период.</span><span class="sxs-lookup"><span data-stu-id="b2433-183">Current period</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b2433-184">-1P</span><span class="sxs-lookup"><span data-stu-id="b2433-184">-1P</span></span></p></td>
<td><p><span data-ttu-id="b2433-185">Предыдущий период.</span><span class="sxs-lookup"><span data-stu-id="b2433-185">Previous period</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b2433-186">-1FY[1..LP]</span><span class="sxs-lookup"><span data-stu-id="b2433-186">-1FY[1..LP]</span></span></p></td>
<td><p><span data-ttu-id="b2433-187">Весь предыдущий финансовый год</span><span class="sxs-lookup"><span data-stu-id="b2433-187">Entire previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b2433-188">-1FY</span><span class="sxs-lookup"><span data-stu-id="b2433-188">-1FY</span></span></p></td>
<td><p><span data-ttu-id="b2433-189">Текущий период предыдущего финансового года</span><span class="sxs-lookup"><span data-stu-id="b2433-189">Current period in previous fiscal year</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b2433-190">-1FY[1..3]</span><span class="sxs-lookup"><span data-stu-id="b2433-190">-1FY[1..3]</span></span></p></td>
<td><p><span data-ttu-id="b2433-191">Первый квартал предыдущего финансового года.</span><span class="sxs-lookup"><span data-stu-id="b2433-191">First quarter of previous fiscal year</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b2433-192">-1ФГ[1..CP]</span><span class="sxs-lookup"><span data-stu-id="b2433-192">-1FY[1..CP]</span></span></p></td>
<td><p><span data-ttu-id="b2433-193">С начала предыдущего финансового года до текущего периода в предыдущем финансовом году, включительно</span><span class="sxs-lookup"><span data-stu-id="b2433-193">From the beginning of previous fiscal year to current period in previous fiscal year, inclusive</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b2433-194">-1FY[CP..LP]</span><span class="sxs-lookup"><span data-stu-id="b2433-194">-1FY[CP..LP]</span></span></p></td>
<td><p><span data-ttu-id="b2433-195">С текущего периода в предыдущем финансовом году до последнего периода предыдущего финансового года, включительно</span><span class="sxs-lookup"><span data-stu-id="b2433-195">From current period in previous fiscal year to last period of previous fiscal year, inclusive</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="b2433-196">Если вычисления необходимо выполнять регулярно через заданный промежуток времени, вместо этого нужно ввести формулу в поле **Формула даты сравнения**.</span><span class="sxs-lookup"><span data-stu-id="b2433-196">If you want to calculate by regular time periods, you must enter a formula in the **Comparison Date Formula** field instead.</span></span>

> [!NOTE]
> <span data-ttu-id="b2433-197">Не всегда очевидно, какие периоды сравниваются, потому что вы можете установить в отчете фильтр по дате, который охватывает даты иные, нежели учетные периоды, отраженные в данных в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="b2433-197">It is not always transparent which periods you are comparing because you can set a date filter on a report that spans different dates than the accounting periods that are reflected in the data in the chart of accounts.</span></span> <span data-ttu-id="b2433-198">Например, вы можете создать отчет для сравнения данного периода с тем же периодом в прошлом году, т. е. задать в поле **Фильтр по периоду даты сравнения** значение *-1ФГ*.</span><span class="sxs-lookup"><span data-stu-id="b2433-198">For example, you create an account schedule where you want to compare this period with the same period last year, so you set the **Comparison Date Period Filter** field to *-1FY*.</span></span> <span data-ttu-id="b2433-199">После этого вы запускаете отчет 28 февраля и устанавливаете в качестве фильтра по дате январь и февраль.</span><span class="sxs-lookup"><span data-stu-id="b2433-199">Then, you run the report on February 28th and set the date filter to January and February.</span></span> <span data-ttu-id="b2433-200">В результате в отчете сравниваются январь и февраль этого года с январем прошлого года, которые представляет собой единственный завершенный учетный период из двух периодов за прошлый год.</span><span class="sxs-lookup"><span data-stu-id="b2433-200">As a result, the account schedule compares January and February this year to January last year, which is the only completed accounting period of the two for last year.</span></span>  


## <a name="see-also"></a><span data-ttu-id="b2433-201">См. также</span><span class="sxs-lookup"><span data-stu-id="b2433-201">See Also</span></span>
[<span data-ttu-id="b2433-202">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="b2433-202">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="b2433-203">Финансы</span><span class="sxs-lookup"><span data-stu-id="b2433-203">Finance</span></span>](finance.md)  
[<span data-ttu-id="b2433-204">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="b2433-204">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="b2433-205">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="b2433-205">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="b2433-206">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b2433-206">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

