---
title: "Создание бюджетов ГК | Microsoft Docs"
description: "Описывает порядок создания бюджетов ГК для прогнозирования различных финансовых действий и назначения измерений для целей бизнес-анализа."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: f1311d566a8166a8a8720bb09789f42c65a1b6e7
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="create-gl-budgets"></a><span data-ttu-id="e568d-103">Создание бюджетов ГК</span><span class="sxs-lookup"><span data-stu-id="e568d-103">Create G/L Budgets</span></span>
<span data-ttu-id="e568d-104">Путем создания бюджетов с различными кодами можно для одного и того же промежутка времени создать несколько бюджетов.</span><span class="sxs-lookup"><span data-stu-id="e568d-104">You can have multiple budgets for identical time periods by creating budgets with separate names.</span></span> <span data-ttu-id="e568d-105">Сначала настраивается код бюджета и заносятся бюджетные данные.</span><span class="sxs-lookup"><span data-stu-id="e568d-105">First, you set up the budget name and enter the budget figures.</span></span> <span data-ttu-id="e568d-106">Название бюджета затем помещается во все созданные бюджетные операции.</span><span class="sxs-lookup"><span data-stu-id="e568d-106">The budget name is then included on all the budget entries you create.</span></span>  

 <span data-ttu-id="e568d-107">При создании бюджетов можно для каждого из них можно задать четыре измерения.</span><span class="sxs-lookup"><span data-stu-id="e568d-107">When you create a budget, you can define four dimensions for each budget.</span></span> <span data-ttu-id="e568d-108">Эти измерения, ориентированные на бюджет, называются бюджетными.</span><span class="sxs-lookup"><span data-stu-id="e568d-108">These budget-specific dimensions are called budget dimensions.</span></span> <span data-ttu-id="e568d-109">Бюджетные измерения для каждого бюджета выбираются из уже существующих измерений.</span><span class="sxs-lookup"><span data-stu-id="e568d-109">You select the budget dimensions for each budget from among the dimensions you have already set up.</span></span> <span data-ttu-id="e568d-110">Бюджетные измерения могут использоваться для установки фильтров бюджета и для добавления информации по измерениям к бюджетным операциям.</span><span class="sxs-lookup"><span data-stu-id="e568d-110">Budget dimensions can be used to set filters on a budget and to add dimension information to budget entries.</span></span> <span data-ttu-id="e568d-111">Дополнительные сведения см. в разделе [Работа с измерениями](finance-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="e568d-111">For more information, see [Working with Dimensions](finance-dimensions.md).</span></span>

 <span data-ttu-id="e568d-112">Бюджеты играют важную роль в бизнес-анализе, например в финансовая отчетности, основанной на финансовых отчетах, которые включают операции бюджета, или при анализе бюджета в сравнении с фактическими суммами в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="e568d-112">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="e568d-113">Дополнительные сведения см. в разделе [Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="e568d-113">For more information, see [Business Intelligence](bi.md).</span></span>

 <span data-ttu-id="e568d-114">Бюджеты играют важную роль в бизнес-анализе, например в финансовая отчетности, основанной на финансовых отчетах, которые включают операции бюджета, или при анализе бюджета в сравнении с фактическими суммами в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="e568d-114">Budgets play an important role in business intelligence, such as in financial statement based on account schedules that include budget entries or when analyzing budgeted versus actual amounts in the chart of accounts.</span></span> <span data-ttu-id="e568d-115">Дополнительные сведения см. в разделе [Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="e568d-115">For more information, see [Business Intelligence](bi.md).</span></span>

<span data-ttu-id="e568d-116">В учете затрат работа с бюджетами затрат производится аналогичным образом.</span><span class="sxs-lookup"><span data-stu-id="e568d-116">In cost accounting, you work with cost budgets in a similar way.</span></span> <span data-ttu-id="e568d-117">Дополнительные сведения см. в разделе [Создание бюджетов затрат](finance-create-cost-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="e568d-117">For more information, see [Creating Cost Budgets](finance-create-cost-budgets.md).</span></span>    

## <a name="to-create-a-new-gl-budget"></a><span data-ttu-id="e568d-118">Создание бюджета ГК</span><span class="sxs-lookup"><span data-stu-id="e568d-118">To create a new G/L budget</span></span>  
1. <span data-ttu-id="e568d-119">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Бюджеты ГК**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e568d-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **G/L Budgets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e568d-120">Выберите действие **Изменить список**, затем введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="e568d-120">Choose the **Edit List** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="e568d-121">Выберите действие **Изменить бюджет**.</span><span class="sxs-lookup"><span data-stu-id="e568d-121">Choose the **Edit Budget** action.</span></span>
4. <span data-ttu-id="e568d-122">В верхней части окна **Бюджет** заполните поля соответствующим образом, чтобы определить, что в нем отображается.</span><span class="sxs-lookup"><span data-stu-id="e568d-122">At the top of the **Budget** window, fill in the fields as necessary to define what is displayed.</span></span>  

    <span data-ttu-id="e568d-123">Теперь будут отображаться только те операции, которые содержат название бюджета, введенное в поле **Название бюджета**.</span><span class="sxs-lookup"><span data-stu-id="e568d-123">Only entries that contain the budget name that you entered in the **budget Name** field are shown.</span></span> <span data-ttu-id="e568d-124">Поскольку название бюджета только что создано, соответствующие фильтру операции отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e568d-124">Because the budget name has just been created, there are no entries that match the filter.</span></span> <span data-ttu-id="e568d-125">Поэтому это окно пустое.</span><span class="sxs-lookup"><span data-stu-id="e568d-125">Therefore, the window is empty.</span></span>  
5. <span data-ttu-id="e568d-126">Чтобы ввести сумму, выберите соответствующую ячейку в матрице.</span><span class="sxs-lookup"><span data-stu-id="e568d-126">To enter an amount, choose the relevant cell in the matrix.</span></span> <span data-ttu-id="e568d-127">Откроется окно **Операции бюджета ГК**.</span><span class="sxs-lookup"><span data-stu-id="e568d-127">The **G/L Budget Entries** window opens.</span></span>  
6. <span data-ttu-id="e568d-128">Создайте новую строку и заполните поле **Сумма**.</span><span class="sxs-lookup"><span data-stu-id="e568d-128">Create a new line and fill in the **Amount** field.</span></span> <span data-ttu-id="e568d-129">Закройте окно **Операции бюджета ГК**.</span><span class="sxs-lookup"><span data-stu-id="e568d-129">Close the **G/L Budget Entries** window.</span></span>  
7. <span data-ttu-id="e568d-130">Повторяйте шаги 5 и 6, пока не будут введены все суммы бюджета.</span><span class="sxs-lookup"><span data-stu-id="e568d-130">Repeat steps 5 and 6 until you have entered all of the budget amounts.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e568d-131">На экспресс-вкладке **Фильтры** можно фильтровать данные бюджета по бюджетным измерениям, настроенным для названия бюджета.</span><span class="sxs-lookup"><span data-stu-id="e568d-131">On the **Filters** FastTab, you can filter the budget information by budget dimensions you have set up under the budget name.</span></span>   

## <a name="see-also"></a><span data-ttu-id="e568d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="e568d-132">See Also</span></span>
[<span data-ttu-id="e568d-133">Финансы</span><span class="sxs-lookup"><span data-stu-id="e568d-133">Finance</span></span>](finance.md)  
[<span data-ttu-id="e568d-134">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="e568d-134">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="e568d-135">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="e568d-135">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="e568d-136">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="e568d-136">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="e568d-137">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e568d-137">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

