---
title: "Создание бюджетов | Документы Майкрософт"
description: "Описывает порядок создания бюджетов для прогнозирования различных финансовых действий и назначения измерений для целей бизнес-анализа."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: cda69d70ece090a149a13e5e1f4ed02fa70c49f7
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create--budgets"></a><span data-ttu-id="04781-103">Практическое руководство. Создание бюджетов</span><span class="sxs-lookup"><span data-stu-id="04781-103">How to: Create  Budgets</span></span>
<span data-ttu-id="04781-104">Путем создания бюджетов с различными кодами можно для одного и того же промежутка времени создать несколько бюджетов.</span><span class="sxs-lookup"><span data-stu-id="04781-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span></span> <span data-ttu-id="04781-105">Сначала настраивается код бюджета и заносятся бюджетные данные.</span><span class="sxs-lookup"><span data-stu-id="04781-105">First, you set up the budget name and enter the budget figures.</span></span> <span data-ttu-id="04781-106">Название бюджета затем помещается во все созданные бюджетные операции.</span><span class="sxs-lookup"><span data-stu-id="04781-106">The budget name is then included on all the budget entries you create.</span></span>  

 <span data-ttu-id="04781-107">При создании бюджетов можно для каждого из них можно задать четыре измерения.</span><span class="sxs-lookup"><span data-stu-id="04781-107">When you create a budget, you can define four dimensions for each budget.</span></span> <span data-ttu-id="04781-108">Эти измерения, ориентированные на бюджет, называются бюджетными.</span><span class="sxs-lookup"><span data-stu-id="04781-108">These budget-specific dimensions are called budget dimensions.</span></span> <span data-ttu-id="04781-109">Бюджетные измерения для каждого бюджета выбираются из уже существующих измерений.</span><span class="sxs-lookup"><span data-stu-id="04781-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span></span> <span data-ttu-id="04781-110">Бюджетные измерения могут использоваться для установки фильтров бюджета и для добавления информации по измерениям к бюджетным операциям.</span><span class="sxs-lookup"><span data-stu-id="04781-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span></span> <span data-ttu-id="04781-111">Дополнительные сведения см. в разделе [Работа с измерениями](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="04781-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

 <span data-ttu-id="04781-112">Бюджеты играют важную роль в бизнес-анализе, например в финансовая отчетности, основанной на финансовых отчетах, которые включают операции бюджета, или при анализе бюджета в сравнении с фактическими суммами в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="04781-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="04781-113">Дополнительные сведения см. в разделе [Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="04781-113">For more information, see [Business Intelligence](bi.md).</span></span>

 <span data-ttu-id="04781-114">Бюджеты играют важную роль в бизнес-анализе, например в финансовая отчетности, основанной на финансовых отчетах, которые включают операции бюджета, или при анализе бюджета в сравнении с фактическими суммами в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="04781-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="04781-115">Дополнительные сведения см. в разделе [Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="04781-115">For more information, see [Business Intelligence](bi.md).</span></span>

<span data-ttu-id="04781-116">В учете затрат работа с бюджетами затрат производится аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="04781-116">In cost accounting, you work with cost budgets in a similar way.</span></span> <span data-ttu-id="04781-117">Дополнительные сведения см. в разделе [Создание бюджетов затрат](finance-create-cost-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="04781-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span></span>    

 > [!NOTE]  
>   <span data-ttu-id="04781-118">Эта функция требует, чтобы было задано значение **Suite**.</span><span class="sxs-lookup"><span data-stu-id="04781-118">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="04781-119">Дополнительные сведения см. в разделе [Настройка взаимодействия [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="04781-119">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>  

### <a name="to-create-a-new-budget"></a><span data-ttu-id="04781-120">Создание бюджета</span><span class="sxs-lookup"><span data-stu-id="04781-120">To create a new budget</span></span>  

1. <span data-ttu-id="04781-121">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Бюджеты ГК**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="04781-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="04781-122">Выберите действие **Изменить список**, затем введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="04781-122">Choose the **Edit List** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="04781-123">Выберите действие **Изменить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="04781-123">Choose the **Edit Budget** action.</span></span>
4. <span data-ttu-id="04781-124">В верхней части окна **Бюджет** заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="04781-124">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span></span>  

    <span data-ttu-id="04781-125">Теперь будут отображаться только те операции, которые содержат название бюджета, введенное в поле **Название бюджета**.</span><span class="sxs-lookup"><span data-stu-id="04781-125">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span></span> <span data-ttu-id="04781-126">Поскольку название бюджета только что создано, соответствующие фильтру операции отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="04781-126">Because the budget name has just been created, there are no entries that match the filter.</span></span> <span data-ttu-id="04781-127">Поэтому это окно пустое.</span><span class="sxs-lookup"><span data-stu-id="04781-127">Therefore, the window is empty.</span></span>  
5. <span data-ttu-id="04781-128">Чтобы ввести сумму, выберите соответствующую ячейку в матрице.</span><span class="sxs-lookup"><span data-stu-id="04781-128">To enter an amount, choose the relevant cell in the matrix.</span></span> <span data-ttu-id="04781-129">Откроется окно **Операции бюджета ГК**.</span><span class="sxs-lookup"><span data-stu-id="04781-129">The **G/L Budget Entries** window opens.</span></span>  
6. <span data-ttu-id="04781-130">Создайте новую строку и заполните поле **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="04781-130">Create a new line and fill in the **Amount** field.</span></span> <span data-ttu-id="04781-131">Закройте окно **Операции бюджета ГК**.</span><span class="sxs-lookup"><span data-stu-id="04781-131">Close the **G/L Budget Entries** window.</span></span>  
7. <span data-ttu-id="04781-132">Повторяйте шаги 5 и 6, пока не будут введены все суммы бюджета.</span><span class="sxs-lookup"><span data-stu-id="04781-132">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="04781-133">На экспресс-вкладке **Фильтры** можно фильтровать данные бюджета по бюджетным измерениям, настроенным для названия бюджета.</span><span class="sxs-lookup"><span data-stu-id="04781-133">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span></span>   

## <a name="see-also"></a><span data-ttu-id="04781-134">См. также</span><span class="sxs-lookup"><span data-stu-id="04781-134">See Also</span></span>
[<span data-ttu-id="04781-135">Финансы</span><span class="sxs-lookup"><span data-stu-id="04781-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="04781-136">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="04781-136">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="04781-137">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="04781-137">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="04781-138">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="04781-138">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="04781-139">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="04781-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

