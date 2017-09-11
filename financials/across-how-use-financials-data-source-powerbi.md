---
title: "Создание источника данных Power BI в Financials | Microsoft Docs"
description: "Можно сделать данные Financials доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 53fb2ae7bbbaf3215ca2549e207512f7c06838b4
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="using-included365finincludesd365finmdmd-as-a-power-bi-data-source"></a><span data-ttu-id="a7606-103">Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI</span><span class="sxs-lookup"><span data-stu-id="a7606-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source</span></span>
<span data-ttu-id="a7606-104">Можно сделать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] доступными в качестве источника данных в Power BI и создать мощные отчеты о состоянии вашего бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a7606-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="a7606-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Power BI.</span><span class="sxs-lookup"><span data-stu-id="a7606-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="a7606-106">Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="a7606-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="a7606-107">Добавление [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных в Power BI Desktop</span><span class="sxs-lookup"><span data-stu-id="a7606-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span></span>
1. <span data-ttu-id="a7606-108">В Power BI Desktop в левой области навигации выберите **Получить данные**.</span><span class="sxs-lookup"><span data-stu-id="a7606-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="a7606-109">В окне **Получить данные** выберите **Веб-службы**, выберите **Dynamics 365 for Financials**, а затем нажмите кнопку **Подключиться**.</span><span class="sxs-lookup"><span data-stu-id="a7606-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 for Financials**, and then choose the **Connect** button.</span></span>

   <span data-ttu-id="a7606-110">Power BI отобразит мастер с руководством по процессу подключения.</span><span class="sxs-lookup"><span data-stu-id="a7606-110">Power BI displays a wizard that will guide you though the connection process.</span></span> <span data-ttu-id="a7606-111">Первым шагом будет ввод URL-адреса OData и названия организации, связанного с учетной записью [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7606-111">The first step will be to enter an OData URL and the company name that is associated with your [!INCLUDE[d365fin](includes/d365fin_md.md)] account.</span></span>  

   <span data-ttu-id="a7606-112">Для параметра *URL-адрес OData* можно скопировать URL-адрес OData V4 любой из веб-служб, перечисленных на странице **Веб-службы** в [!INCLUDE[d365fin](includes/d365fin_md.md)], например `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span><span class="sxs-lookup"><span data-stu-id="a7606-112">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span></span>  

   <span data-ttu-id="a7606-113">Для параметра *Название организации* используйте название, которое отображается в поле **Имя** в окне **Информация об организации** в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7606-113">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="a7606-114">Если [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит несколько организаций, выберите соответствующее название организации из списка в окне **Организации**.</span><span class="sxs-lookup"><span data-stu-id="a7606-114">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span></span> <span data-ttu-id="a7606-115">В обоих случаях убедитесь, что название, указываемое в мастере Power BI точно соответствует тексту, отображаемому в [!INCLUDE[d365fin](includes/d365fin_md.md)], например `My Company`.</span><span class="sxs-lookup"><span data-stu-id="a7606-115">In both cases, make sure that the name that you specify in the Power BI wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span></span>
3. <span data-ttu-id="a7606-116">После ввода информации нажмите кнопку ОК.</span><span class="sxs-lookup"><span data-stu-id="a7606-116">Once you have entered the information, choose the OK button.</span></span> <span data-ttu-id="a7606-117">Следующий шаг в мастере — ввод имени пользователя и пароля.</span><span class="sxs-lookup"><span data-stu-id="a7606-117">The next step in the wizard will be to enter your username and password.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="a7606-118">Если доступны другие параметры проверки подлинности в левой области навигации, выберите *Базовый*.</span><span class="sxs-lookup"><span data-stu-id="a7606-118">If there are other authentication options available in the left hand navigation, choose *Basic*.</span></span>
4. <span data-ttu-id="a7606-119">Введите имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="a7606-119">Enter your username and password.</span></span> <span data-ttu-id="a7606-120">Эти сведения можно найти в окне **Пользователи** в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7606-120">You can find this information in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="a7606-121">Используйте **Ключ веб-доступа** в качестве пароля.</span><span class="sxs-lookup"><span data-stu-id="a7606-121">Use the **Web Access Key** as your password.</span></span>

   <span data-ttu-id="a7606-122">Например, ваше имя пользователя — *ADMIN*, а ключ доступа веб-службы, который используется как пароль, — *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span><span class="sxs-lookup"><span data-stu-id="a7606-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span></span>
5. <span data-ttu-id="a7606-123">Нажмите кнопку **Подключение**, чтобы продолжить.</span><span class="sxs-lookup"><span data-stu-id="a7606-123">Choose the **Connection** button to continue.</span></span> <span data-ttu-id="a7606-124">Мастер Power BI отобразит список источников данных [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7606-124">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] data sources.</span></span> <span data-ttu-id="a7606-125">Эти источники данных представляют все веб-службы, которые вы опубликовали из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="a7606-125">These data source represent all the web services that you have published from your [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="a7606-126">Либо создайте новый URL-адрес веб-службы в [!INCLUDE[d365fin](includes/d365fin_md.md)], используя действие **Создать набор данных** на странице **Веб-службы** с помощью руководства по сопровождаемой настройке **Настройка отчетов** либо используя действие **Изменить в Excel** в любом списке.</span><span class="sxs-lookup"><span data-stu-id="a7606-126">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
6. <span data-ttu-id="a7606-127">Укажите данные, которые требуется добавить в модель данных, а затем нажмите кнопку **Загрузить**.</span><span class="sxs-lookup"><span data-stu-id="a7606-127">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="a7606-128">Повторите предыдущие шаги для добавления дополнительных данных [!INCLUDE[d365fin](includes/d365fin_md.md)] в модель данных Power BI.</span><span class="sxs-lookup"><span data-stu-id="a7606-128">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="a7606-129">После успешного подключения к [!INCLUDE[d365fin](includes/d365fin_md.md)] вводить URL-адрес OData, имя пользователя или пароль повторно не требуется.</span><span class="sxs-lookup"><span data-stu-id="a7606-129">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span></span>

<span data-ttu-id="a7606-130">После загрузки данные отобразятся в правой области навигации на странице.</span><span class="sxs-lookup"><span data-stu-id="a7606-130">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="a7606-131">На этом шаге вы успешно подключились с данным Dynamics 365 и готовы начать создание отчета Power BI.</span><span class="sxs-lookup"><span data-stu-id="a7606-131">At this point, you have successfully connected to your Dynamics 365 data and are ready to begin building your Power BI report.</span></span> <span data-ttu-id="a7606-132">Дополнительные сведения см. в разделе [Документация Power BI](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span><span class="sxs-lookup"><span data-stu-id="a7606-132">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span></span>

## <a name="see-also"></a><span data-ttu-id="a7606-133">См. также</span><span class="sxs-lookup"><span data-stu-id="a7606-133">See Also</span></span>
<span data-ttu-id="a7606-134">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="a7606-134">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="a7606-135">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="a7606-135">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="a7606-136">[Установка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="a7606-136">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="a7606-137">Финансы</span><span class="sxs-lookup"><span data-stu-id="a7606-137">Finance</span></span>](finance.md)  
