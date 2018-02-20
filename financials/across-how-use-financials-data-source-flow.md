---
title: "Связывание данных с Flow | Документы Майкрософт"
description: "Данные Financials можно сделать доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса."
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 01/25/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: ef4d841723b6bb0af37695a8c3ed1d805319be78
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="using-included365finincludesd365finmdmd-in-an-automated-workflow"></a><span data-ttu-id="63010-103">Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе</span><span class="sxs-lookup"><span data-stu-id="63010-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow</span></span>
<span data-ttu-id="63010-104">Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="63010-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="63010-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.</span><span class="sxs-lookup"><span data-stu-id="63010-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-flow"></a><span data-ttu-id="63010-106">Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Flow</span><span class="sxs-lookup"><span data-stu-id="63010-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Flow</span></span>
1. <span data-ttu-id="63010-107">В браузере перейдите к [flow.microsoft.com](https://flow.microsoft.com/en-us/) и выполните вход.</span><span class="sxs-lookup"><span data-stu-id="63010-107">In your browser, navigate to [flow.microsoft.com](https://flow.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="63010-108">Выберите **Мои Flow** в ленте вверху страницы.</span><span class="sxs-lookup"><span data-stu-id="63010-108">Choose **My Flows** from the ribbon at the top of the page.</span></span>
3. <span data-ttu-id="63010-109">В окне **Мои Flow** выберите параметр **Создать новый**.</span><span class="sxs-lookup"><span data-stu-id="63010-109">In the **My Flows** window, choose the **Create from blank** option.</span></span>
4. <span data-ttu-id="63010-110">Из списка доступных триггеров выберите один из доступных триггеров [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="63010-110">From the list of available triggers, select one of the [!INCLUDE[d365fin](includes/d365fin_md.md)] triggers available:</span></span>  
    <span data-ttu-id="63010-111">*При создании записи*</span><span class="sxs-lookup"><span data-stu-id="63010-111">*When a record is created*,</span></span>  
    <span data-ttu-id="63010-112">*При удалении записи*</span><span class="sxs-lookup"><span data-stu-id="63010-112">*When a record is deleted*,</span></span>  
    <span data-ttu-id="63010-113">*При изменении записи*</span><span class="sxs-lookup"><span data-stu-id="63010-113">*When a record is modified*,</span></span>  
    <span data-ttu-id="63010-114">*Если запрашивается утверждение клиента*</span><span class="sxs-lookup"><span data-stu-id="63010-114">*When a customer approval is requested*,</span></span>  
    <span data-ttu-id="63010-115">*Если запрашивается утверждение раздела финансового журнала*</span><span class="sxs-lookup"><span data-stu-id="63010-115">*When a general journal batch approval is requested*,</span></span>  
    <span data-ttu-id="63010-116">*Если запрашивается утверждение строки финансового журнала*</span><span class="sxs-lookup"><span data-stu-id="63010-116">*When a general journal line approval is requested*,</span></span>  
    <span data-ttu-id="63010-117">*Если запрашивается утверждение товара*</span><span class="sxs-lookup"><span data-stu-id="63010-117">*When an item approval is requested*,</span></span>  
    <span data-ttu-id="63010-118">*Если запрашивается утверждение документа покупки*</span><span class="sxs-lookup"><span data-stu-id="63010-118">*When a purchase document approval is requested*,</span></span>  
    <span data-ttu-id="63010-119">*Если запрашивается утверждение документа продажи*, или</span><span class="sxs-lookup"><span data-stu-id="63010-119">*When a sales document approval is requested*, or</span></span>  
    <span data-ttu-id="63010-120">*Если запрашивается утверждение поставщика*</span><span class="sxs-lookup"><span data-stu-id="63010-120">*When a vendor aproval is requested*.</span></span>
5. <span data-ttu-id="63010-121">Flow отобразит запрос на ввод информации, необходимой для подключения к данным [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="63010-121">Flow will prompt you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span></span> <span data-ttu-id="63010-122">При выборе одного из следующих триггеров *При создании записи*, *При изменении записи* или *При удалении записи* необходимо выбрать название организации или имя таблицы.</span><span class="sxs-lookup"><span data-stu-id="63010-122">If you selected one of the following triggers: *When a record is created*, *When a record is modified*, or *When a record is deleted*, you must select a company name and table name.</span></span> <span data-ttu-id="63010-123">В случае любого другого триггера для подключения требуется только название организации.</span><span class="sxs-lookup"><span data-stu-id="63010-123">With any other trigger, only the company name is required to connect.</span></span>

   <span data-ttu-id="63010-124">Flow отобразит список организаций и таблиц, доступных для [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="63010-124">Flow will show a list of companies and tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="63010-125">Эти таблицы или конечные точки представляют все веб-службы, которые вы опубликовали из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="63010-125">These tables, or end points, represent all the web services that you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="63010-126">Либо создайте новый URL-адрес веб-службы в [!INCLUDE[d365fin](includes/d365fin_md.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.</span><span class="sxs-lookup"><span data-stu-id="63010-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>

<span data-ttu-id="63010-127">На этом шаге вы успешно подключились с данным Finance and Operations, Business edition и готовы начать создание потока.</span><span class="sxs-lookup"><span data-stu-id="63010-127">At this point, you have successfully connected to your Finance and Operations, Business edition data and are ready to begin building your flow.</span></span> <span data-ttu-id="63010-128">Дополнительные сведения см. в разделе [Документация Flow](https://flow.microsoft.com/documentation/getting-started/).</span><span class="sxs-lookup"><span data-stu-id="63010-128">For more information, see the [Flow documentation](https://flow.microsoft.com/documentation/getting-started/).</span></span>

<span data-ttu-id="63010-129">При устранении неполадок с Microsoft Flow см. раздел [Устранение неполадок при интеграции с Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="63010-129">For troubleshooting your Microsoft Flow, see [Troubleshooting Integration with Microsoft Flow](across-troubleshooting-how-use-financials-data-source-flow.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="63010-130">См. также</span><span class="sxs-lookup"><span data-stu-id="63010-130">See Also</span></span>
<span data-ttu-id="63010-131">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="63010-131">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="63010-132">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="63010-132">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="63010-133">[Управление пользователями и разрешениями](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="63010-133">[Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="63010-134">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="63010-134">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="63010-135">Финансы</span><span class="sxs-lookup"><span data-stu-id="63010-135">Finance</span></span>](finance.md)  

