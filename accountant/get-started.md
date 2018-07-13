---
title: "Работа бухгалтера в Dynamics 365 | Документы Майкрософт"
description: "Узнайте об Accountant Hub для Dynamics 365."
author: edupont04
ms.service: dynamics365-accountant
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 05/15/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4bc9199b879c23115082b07a81d6da5a0b46e60d
ms.openlocfilehash: bb700a7c65721efb7c1322420a4929eb7adc4433
ms.contentlocale: ru-ru
ms.lasthandoff: 05/31/2018

---
# <a name="get-started-with-include-d365acclongincludesd365acclongmdmd"></a><span data-ttu-id="9c64d-103">Начало работы с [!INCLUDE [d365acc_long](includes/d365acc_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="9c64d-103">Get started with [!INCLUDE [d365acc_long](includes/d365acc_long_md.md)]</span></span>
[!INCLUDE [d365fin_early_release](includes/d365fin_early_release.md.md)]

<span data-ttu-id="9c64d-104">Любой организации нужно вести учет и подписывать соответствующую документацию.</span><span class="sxs-lookup"><span data-stu-id="9c64d-104">Any business must do its books and sign off on the accounting.</span></span> <span data-ttu-id="9c64d-105">Некоторые организации используют внешнего бухгалтера, а у других — бухгалтер в штате.</span><span class="sxs-lookup"><span data-stu-id="9c64d-105">Some businesses employ an external accountant, and others have an accountant on staff.</span></span> <span data-ttu-id="9c64d-106">Если вы бухгалтер, в которого несколько клиентов, вы можете использовать [!INCLUDE [d365acc](includes/d365acc_md.md)] в качестве панели мониторинга для более наглядного представления информации о своих клиентах.</span><span class="sxs-lookup"><span data-stu-id="9c64d-106">If you are an accountant with several clients, you can use [!INCLUDE [d365acc](includes/d365acc_md.md)] as your dashboard for a better overview of your clients.</span></span>  

<span data-ttu-id="9c64d-107">Получить доступ к [!INCLUDE [d365acc](includes/d365acc_md.md)] можно, зарегистрировавшись на странице [Dynamics 365 — Accountant Hub на Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants).</span><span class="sxs-lookup"><span data-stu-id="9c64d-107">You can get access to [!INCLUDE [d365acc](includes/d365acc_md.md)] by signing up from [Dynamics 365 — Accountant Hub on Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants).</span></span>  

> [!TIP]
>  <span data-ttu-id="9c64d-108">Когда вы регистрируетесь на [!INCLUDE [d365acc](includes/d365acc_md.md)], вы должны указать свой рабочий адрес электронной почты, например <em>me@accountant.com</em>.</span><span class="sxs-lookup"><span data-stu-id="9c64d-108">When you sign up for [!INCLUDE [d365acc](includes/d365acc_md.md)], you must specify your work email address, such as <em>me@accountant.com</em>.</span></span> <span data-ttu-id="9c64d-109">Рекомендуется использовать этот же адрес электронной почты при работе в клиентах [!INCLUDE [d365fin_long](includes/d365fin_long_md.md)], чтобы вы могли легко переключаться между клиентами.</span><span class="sxs-lookup"><span data-stu-id="9c64d-109">We recommend that you use the same email address when you work in your clients' [!INCLUDE [d365fin_long](includes/d365fin_long_md.md)], so that you can easily switch between clients.</span></span> <span data-ttu-id="9c64d-110">Адрес электронной почты должен представлять собой рабочий адрес, основанный на Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9c64d-110">The email address must be a work address that is based on Active Directory.</span></span>

## <a name="working-with-individual-clients"></a><span data-ttu-id="9c64d-111">Работа с индивидуальными клиентами</span><span class="sxs-lookup"><span data-stu-id="9c64d-111">Working with individual clients</span></span>
<span data-ttu-id="9c64d-112">На панели мониторинга отображается наиболее важная информация о каждом клиенте.</span><span class="sxs-lookup"><span data-stu-id="9c64d-112">The dashboard shows the most important information about each client.</span></span>  
![Accountant Hub](./media/accountant-get-started/accountant-dashboard-tasks.png)

<span data-ttu-id="9c64d-114">Столбец **Название клиента** содержит названия клиентов, а столбец **Название организации** — все организации, если у клиента в [!INCLUDE [d365fin_long](includes/d365fin_long_md.md)] имеется более одной организации.</span><span class="sxs-lookup"><span data-stu-id="9c64d-114">The **Client Name** column shows the names of your clients, and the **Company Name** column lists all companies if the client has more than one company in [!INCLUDE [d365fin_long](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="9c64d-115">Также здесь имеются поля для отображения задач, назначенных вам в компании-клиенте, включая просроченные задачи.</span><span class="sxs-lookup"><span data-stu-id="9c64d-115">There are also fields to show you tasks that are assigned to you in your client's company, including overdue tasks.</span></span>  

<span data-ttu-id="9c64d-116">Вы можете настроить панель мониторинга, чтобы на ней отображались только нужные данные. Для этого можно добавить или удалить столбцы.</span><span class="sxs-lookup"><span data-stu-id="9c64d-116">You can customize the dashboard to show the data points that you want to see by adding or removing columns.</span></span> <span data-ttu-id="9c64d-117">Например, может возникнуть необходимость видеть налоги к уплате, количество открытых документов продажи по каждому клиенту и общее число счетов покупки, которые нужно оплатить на следующей неделе.</span><span class="sxs-lookup"><span data-stu-id="9c64d-117">For example, you might want to see taxes that are due, how many open sales documents each client has, or the number of purchase invoices that are due next week.</span></span> <span data-ttu-id="9c64d-118">Вы можете настроить представление в соответствии со своими потребностями.</span><span class="sxs-lookup"><span data-stu-id="9c64d-118">You can configure the view to suit your needs.</span></span> <span data-ttu-id="9c64d-119">Если у вас много клиентов, вы можете использовать фильтры для сортировки представления.</span><span class="sxs-lookup"><span data-stu-id="9c64d-119">If you have many clients, you can use filters to sort your view.</span></span>  

<span data-ttu-id="9c64d-120">Рядом с названием клиента многоточие (...) открывает краткое меню:</span><span class="sxs-lookup"><span data-stu-id="9c64d-120">Next to the client name, the ellipsis (...) reveals a short menu:</span></span>

- <span data-ttu-id="9c64d-121">Обновление текущей организации и получение свежих данных по клиенту</span><span class="sxs-lookup"><span data-stu-id="9c64d-121">Refresh the current company and get fresh data for the client</span></span>  
- <span data-ttu-id="9c64d-122">Переход к [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента</span><span class="sxs-lookup"><span data-stu-id="9c64d-122">Go to the client's [!INCLUDE [d365fin](includes/d365fin_md.md)]</span></span>  
- <span data-ttu-id="9c64d-123">Выберите дополнительных клиентов</span><span class="sxs-lookup"><span data-stu-id="9c64d-123">Select more clients</span></span>  

<span data-ttu-id="9c64d-124">Аналогично можно использовать раскрывающимся меню **Сводка по клиенту**, чтобы обновить информацию по всем компаниям.</span><span class="sxs-lookup"><span data-stu-id="9c64d-124">Similarly, you can use the **Client Summary** drop-down menu to refresh all companies, for example.</span></span>  

> [!TIP]
>  <span data-ttu-id="9c64d-125">Для получения доступа к [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента, в меню выберите команду **Переход к клиенту**. Вход будет выполнен автоматически.</span><span class="sxs-lookup"><span data-stu-id="9c64d-125">To access a client's [!INCLUDE [d365fin](includes/d365fin_md.md)], choose the **Go To Client** menu item - you are logged in automatically.</span></span>

## <a name="company-details"></a><span data-ttu-id="9c64d-126">Подробная информация по организации</span><span class="sxs-lookup"><span data-stu-id="9c64d-126">Company details</span></span>
<span data-ttu-id="9c64d-127">Можно просмотреть дополнительную информацию о данных вашего клиента, выбрав название организации, по которой требуются дополнительные сведения.</span><span class="sxs-lookup"><span data-stu-id="9c64d-127">You can see more information about your clients' data by choosing the name of the company that you want to learn more about.</span></span> <span data-ttu-id="9c64d-128">При этом откроется область **Подробная информация по организации**, в которой можно просмотреть дополнительную информацию, например:</span><span class="sxs-lookup"><span data-stu-id="9c64d-128">This opens the **Company Details** pane, where you can see additional information, such as the following:</span></span>  

* <span data-ttu-id="9c64d-129">Сальдо кассы</span><span class="sxs-lookup"><span data-stu-id="9c64d-129">Cash account balances</span></span>  
* <span data-ttu-id="9c64d-130">Прогноз движения денежных средств</span><span class="sxs-lookup"><span data-stu-id="9c64d-130">Cash flow forecast</span></span>  
* <span data-ttu-id="9c64d-131">Просроченные счета покупки</span><span class="sxs-lookup"><span data-stu-id="9c64d-131">Overdue purchase invoices</span></span>  
* <span data-ttu-id="9c64d-132">Просроченные счета продажи</span><span class="sxs-lookup"><span data-stu-id="9c64d-132">Overdue sales invoices</span></span>  

![Подробные сведения о компании-клиенте на панели мониторинга бухгалтера](./media/accountant-get-started/accountant-company-details.png)

<span data-ttu-id="9c64d-134">Технически вы теперь выполнили вход в [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента, и отображаются актуальные данные.</span><span class="sxs-lookup"><span data-stu-id="9c64d-134">Technically, you have now logged into your client's [!INCLUDE [d365fin](includes/d365fin_md.md)], and data you see is live data.</span></span> <span data-ttu-id="9c64d-135">Если необходимо более тщательно изучить данные, например просроченные счета покупки, выберите ссылку, и будет выполнен переход в организацию клиента.</span><span class="sxs-lookup"><span data-stu-id="9c64d-135">If you want to take a closer look at the data, such as an overdue purchase invoice, choose the link, and you are taken to the client company.</span></span>  

> [!TIP]
>  <span data-ttu-id="9c64d-136">С помощью вкладки **Отчеты** на вкладке можно запускать заранее заданные книги Excel.</span><span class="sxs-lookup"><span data-stu-id="9c64d-136">You can launch predefined Excel workbooks from the **Reports** tab in the ribbon.</span></span> <span data-ttu-id="9c64d-137">Эти книги Excel разработаны как готовые к печати ключевые финансовые выписки и отчеты, но можно также изменять их в соответствии со своими потребностями.</span><span class="sxs-lookup"><span data-stu-id="9c64d-137">These Excel workbooks are designed as ready-to-print key financial statements and reports, but you can also modify them to fit your needs.</span></span> <span data-ttu-id="9c64d-138">Дополнительные сведения см. в разделе [Анализ финансовых выписок в Microsoft Excel](/dynamics365/business-central/finance-analyze-excel?toc=/dynamics365/accountants/toc.json) в справке по [!INCLUDE [d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="9c64d-138">For more information, see [Analyzing Financial Statements in Microsoft Excel](/dynamics365/business-central/finance-analyze-excel?toc=/dynamics365/accountants/toc.json) in the Help for [!INCLUDE [d365fin](includes/d365fin_md.md)].</span></span>  

<span data-ttu-id="9c64d-139">В противном случае закройте область сведений и переходите к следующему клиенту.</span><span class="sxs-lookup"><span data-stu-id="9c64d-139">Otherwise, close the details pane and continue to the next client.</span></span>  

## <a name="assigned-tasks"></a><span data-ttu-id="9c64d-140">Назначенные задачи</span><span class="sxs-lookup"><span data-stu-id="9c64d-140">Assigned tasks</span></span>
<span data-ttu-id="9c64d-141">В [!INCLUDE [d365fin](includes/d365fin_md.md)] своего клиента вы можете назначать задачи себе и другим пользователям, а другие пользователи могут назначать задачи вам.</span><span class="sxs-lookup"><span data-stu-id="9c64d-141">In your client's [!INCLUDE [d365fin](includes/d365fin_md.md)], you can assign tasks to yourself and others, and others can assign tasks to you.</span></span> <span data-ttu-id="9c64d-142">Ваша панель мониторинга в [!INCLUDE [d365acc](includes/d365acc_md.md)] позволяет получить представление о назначенных задачах по каждому клиенту; кроме того, вы можете открыть список всех назначенных задач, выбрав **Мои задачи пользователя** в левой области навигации.</span><span class="sxs-lookup"><span data-stu-id="9c64d-142">Your dashboard in [!INCLUDE [d365acc](includes/d365acc_md.md)] gives you an overview of assigned tasks for each client, and you can also access a list of all assigned tasks by choosing **My User Tasks** in the left navigation.</span></span>  

<span data-ttu-id="9c64d-143">В компании-клиенте также имеются индикаторы для обозначения задач, назначенных вам в данной компании.</span><span class="sxs-lookup"><span data-stu-id="9c64d-143">In the client company, you also have cues that call out tasks assigned to you in this particular client.</span></span>

![Задачи, назначенные бухгалтеру в компании-клиенте](./media/accountant-get-started/accountant-company-details-tasks.png)

### <a name="my-user-tasks"></a><span data-ttu-id="9c64d-145">Мои задачи пользователя</span><span class="sxs-lookup"><span data-stu-id="9c64d-145">My user tasks</span></span>
<span data-ttu-id="9c64d-146">Список **Мои задачи пользователя** в [!INCLUDE [d365acc](includes/d365acc_md.md)] поможет вам расставить приоритеты и спланировать свой рабочий день: в нем отображается дополнительная информация о задачах, назначенных вам различными вашими клиентами.</span><span class="sxs-lookup"><span data-stu-id="9c64d-146">The **My User Tasks** list in [!INCLUDE [d365acc](includes/d365acc_md.md)] helps you prioritize your day by showing more information about tasks assigned to you across all your clients.</span></span>  

![Список задач, назначенных мне как внешнему бухгалтеру](./media/accountant-get-started/accountant-tasklist.png)

<span data-ttu-id="9c64d-148">Вы можете сортировать его по сроку выполнения, например, или по любому другому типу данных, чтобы расставить приоритеты для планирования своей работы.</span><span class="sxs-lookup"><span data-stu-id="9c64d-148">You can sort by due date, for example, or any other type of data that helps you prioritize your day.</span></span> <span data-ttu-id="9c64d-149">По умолчанию в списке отображаются все назначенные вам задачи, однако вы можете настроить фильтры, чтобы в нем отображались только задачи, помеченные как высокоприоритетные, например.</span><span class="sxs-lookup"><span data-stu-id="9c64d-149">By default, the list shows all tasks that are assigned to you, but you can set up filters to only show tasks that are marked as high priority, for example.</span></span>

<span data-ttu-id="9c64d-150">Чтобы выбрать задачу, просто выберите ее в списке ожидающих задач пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c64d-150">To pick up a task, simply choose it from the list of pending user tasks.</span></span> <span data-ttu-id="9c64d-151">На ленте ссылка **Перейти к элементу задачи** открывает окно, в котором можно сделать работу.</span><span class="sxs-lookup"><span data-stu-id="9c64d-151">In the ribbon, the link **Go to Task Item** opens the window where you can do the work.</span></span>  

<span data-ttu-id="9c64d-152">После завершения задачи просто отметьте ее как выполненную.</span><span class="sxs-lookup"><span data-stu-id="9c64d-152">When you have completed a task, simply mark it as completed.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9c64d-153">См. также</span><span class="sxs-lookup"><span data-stu-id="9c64d-153">See Also</span></span>
<span data-ttu-id="9c64d-154">[Добавление клиентов на панель мониторинга в [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md)</span><span class="sxs-lookup"><span data-stu-id="9c64d-154">[Add Clients to Your Dashboard in [!INCLUDE[d365acc](includes/d365acc_md.md)]](add-client.md)</span></span>  
<span data-ttu-id="9c64d-155">[Добро пожаловать в [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="9c64d-155">[Welcome to [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="9c64d-156">[Анализ финансовых отчетов в Microsoft Excel](/dynamics365/business-central/finance-analyze-excel?toc=/dynamics365/accountants/toc.json) </span><span class="sxs-lookup"><span data-stu-id="9c64d-156">[Analyzing Financial Statements in Microsoft Excel](/dynamics365/business-central/finance-analyze-excel?toc=/dynamics365/accountants/toc.json) </span></span>  
<span data-ttu-id="9c64d-157">[Работа бухгалтера в [!INCLUDE[d365fin](includes/d365fin_md.md)]](/dynamics365/business-central/finance-accounting?toc=/dynamics365/accountants/toc.json)</span><span class="sxs-lookup"><span data-stu-id="9c64d-157">[Accountant Experiences in [!INCLUDE[d365fin](includes/d365fin_md.md)]](/dynamics365/business-central/finance-accounting?toc=/dynamics365/accountants/toc.json)</span></span>  
[<span data-ttu-id="9c64d-158">Dynamics 365 — Accountant Hub на Microsoft.com</span><span class="sxs-lookup"><span data-stu-id="9c64d-158">Dynamics 365 — Accountant Hub on Microsoft.com</span></span>](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  

