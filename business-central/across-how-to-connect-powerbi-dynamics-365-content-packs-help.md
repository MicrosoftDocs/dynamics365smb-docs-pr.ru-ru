---
title: "Подключение Power BI к Business Central | Microsoft Docs"
description: "Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря пакетам содержимого Power BI и Business Central."
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 03/16/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 315d4b188cdd834e82676a0c5ef77272ad873eb7
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-power-bi-to-business-central-content-packs"></a><span data-ttu-id="5450f-103">Подключение Power BI к пакетам содержимого Business Central</span><span class="sxs-lookup"><span data-stu-id="5450f-103">Connecting Power BI to Business Central Content Packs</span></span>
<span data-ttu-id="5450f-104">Анализ данных Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] становится проще благодаря Power BI и пакетам содержимого Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5450f-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="5450f-105">Power BI извлекает ваши данные, а затем создает готовую панель мониторинга и отчеты на основе этих данных.</span><span class="sxs-lookup"><span data-stu-id="5450f-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

> [!NOTE]  
>  <span data-ttu-id="5450f-106">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Power BI.</span><span class="sxs-lookup"><span data-stu-id="5450f-106">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="5450f-107">Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="5450f-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  
>  <span data-ttu-id="5450f-108">Для пакетов содержимого Power BI требуются разрешения к таблицам, из которых извлекаются данные.</span><span class="sxs-lookup"><span data-stu-id="5450f-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="5450f-109">Дополнительные сведения о требованиях см. ниже.</span><span class="sxs-lookup"><span data-stu-id="5450f-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="5450f-110">Подключение</span><span class="sxs-lookup"><span data-stu-id="5450f-110">How to Connect</span></span>
1. <span data-ttu-id="5450f-111">Выберите **Получить данные** в нижней части левой панели навигации.</span><span class="sxs-lookup"><span data-stu-id="5450f-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="5450f-112">![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="5450f-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>
2. <span data-ttu-id="5450f-113">В поле **Службы** выберите **Получить**.</span><span class="sxs-lookup"><span data-stu-id="5450f-113">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="5450f-114">Откроется окно **AppSource** и **Приложения для приложений Power BI**.</span><span class="sxs-lookup"><span data-stu-id="5450f-114">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="5450f-115">![Выбор пакетов содержимого из веб-служб](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="5450f-115">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="5450f-116">Выберите **Приложения** на вкладке **Приложения для приложений Power BI**, выберите требуемый пакет содержимого **Microsoft Dynamics 365 Business Central** и щелкните **Получить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="5450f-116">Select **Apps** from the **Apps for Power BI apps** tab, and choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="5450f-117">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="5450f-117">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="5450f-118">При появлении запроса ведите имя *вашей организации* в [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5450f-118">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="5450f-119">Это не отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="5450f-119">This is not the display name.</span></span>  
<span data-ttu-id="5450f-120">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="5450f-120">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="5450f-121">После подключения панель мониторинга, отчет и набор данных будут автоматически отправлены в рабочую область Power BI.</span><span class="sxs-lookup"><span data-stu-id="5450f-121">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="5450f-122">По завершении плитки обновятся для отображения данных из учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5450f-122">When completed, the tiles will update with data from your account.</span></span>
<span data-ttu-id="5450f-123">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="5450f-123">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="5450f-124">Что теперь?</span><span class="sxs-lookup"><span data-stu-id="5450f-124">What Now?</span></span>

- <span data-ttu-id="5450f-125">[Измените плитки](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) на панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="5450f-125">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="5450f-126">[Выберите плитку](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.</span><span class="sxs-lookup"><span data-stu-id="5450f-126">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="5450f-127">Хотя набор данных будет обновляться ежедневно, можно изменить график обновлений или попытаться обновить его по требованию с помощью функции **Обновить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="5450f-127">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="5450f-128">Требования к системе</span><span class="sxs-lookup"><span data-stu-id="5450f-128">System Requirements</span></span>
<span data-ttu-id="5450f-129">Чтобы импортировать данные [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных.</span><span class="sxs-lookup"><span data-stu-id="5450f-129">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="5450f-130">Веб-службы, необходимые для каждого пакета содержимого:</span><span class="sxs-lookup"><span data-stu-id="5450f-130">The web services required for each content pack include:</span></span>

<span data-ttu-id="5450f-131">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="5450f-131">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="5450f-132">SalesOpportunities</span><span class="sxs-lookup"><span data-stu-id="5450f-132">SalesOpportunities</span></span>
- <span data-ttu-id="5450f-133">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-133">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="5450f-134">**Microsoft Dynamics 365 Business Central – Продажи**</span><span class="sxs-lookup"><span data-stu-id="5450f-134">**Microsoft Dynamics 365 Business Central – Sales**</span></span>
- <span data-ttu-id="5450f-135">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="5450f-135">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="5450f-136">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="5450f-136">SalesDashboard</span></span>
- <span data-ttu-id="5450f-137">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-137">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="5450f-138">**Microsoft Dynamics 365 Business Central – Финансы**</span><span class="sxs-lookup"><span data-stu-id="5450f-138">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="5450f-139">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="5450f-139">PowerBIFinance</span></span>
- <span data-ttu-id="5450f-140">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-140">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="5450f-141">**Microsoft Dynamics 365 Business Central – Работы**</span><span class="sxs-lookup"><span data-stu-id="5450f-141">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="5450f-142">Список работ</span><span class="sxs-lookup"><span data-stu-id="5450f-142">Job List</span></span>
- <span data-ttu-id="5450f-143">Строки планирования работ</span><span class="sxs-lookup"><span data-stu-id="5450f-143">Job Planning Lines</span></span>
- <span data-ttu-id="5450f-144">Строки рабочего задания</span><span class="sxs-lookup"><span data-stu-id="5450f-144">Job Task Lines</span></span>

<span data-ttu-id="5450f-145">**Microsoft Dynamics 365 Business Central – Список клиентов**</span><span class="sxs-lookup"><span data-stu-id="5450f-145">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="5450f-146">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="5450f-146">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="5450f-147">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="5450f-147">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="5450f-148">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="5450f-148">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="5450f-149">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="5450f-149">SalesDashboard</span></span>
- <span data-ttu-id="5450f-150">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="5450f-150">Power_BI_Customer_List</span></span>
- <span data-ttu-id="5450f-151">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-151">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="5450f-152">**Microsoft Dynamics 365 Business Central – Список товаров**</span><span class="sxs-lookup"><span data-stu-id="5450f-152">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="5450f-153">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="5450f-153">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="5450f-154">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="5450f-154">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="5450f-155">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="5450f-155">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="5450f-156">Товаров</span><span class="sxs-lookup"><span data-stu-id="5450f-156">Items</span></span>
- <span data-ttu-id="5450f-157">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="5450f-157">SalesDashboard</span></span>
- <span data-ttu-id="5450f-158">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-158">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="5450f-159">**Microsoft Dynamics 365 Business Central – Список поставщиков**</span><span class="sxs-lookup"><span data-stu-id="5450f-159">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="5450f-160">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="5450f-160">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="5450f-161">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="5450f-161">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="5450f-162">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="5450f-162">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="5450f-163">Товаров</span><span class="sxs-lookup"><span data-stu-id="5450f-163">Items</span></span>
- <span data-ttu-id="5450f-164">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="5450f-164">SalesDashboard</span></span>
- <span data-ttu-id="5450f-165">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="5450f-165">Power_BI_Customer_List</span></span>
- <span data-ttu-id="5450f-166">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="5450f-166">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="5450f-167">Power_BI_Vendor_List</span><span class="sxs-lookup"><span data-stu-id="5450f-167">Power_BI_Vendor_List</span></span>
- <span data-ttu-id="5450f-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="5450f-168">ExcelTemplateViewCompany</span></span>

## <a name="web-services"></a><span data-ttu-id="5450f-169">Веб-службы</span><span class="sxs-lookup"><span data-stu-id="5450f-169">Web Services</span></span>
<span data-ttu-id="5450f-170">Простой способ найти веб-службы — найти веб-службы в [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5450f-170">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="5450f-171">В списке проверьте, что установлен флажок "Опубликовать" для веб-служб, перечисленных выше.</span><span class="sxs-lookup"><span data-stu-id="5450f-171">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="5450f-172">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5450f-172">Troubleshooting</span></span>
<span data-ttu-id="5450f-173">Панель мониторинга Power BI основана на опубликованных веб-службах, которые перечислены выше, и содержит данные демонстрационной организации или вашей организации, если вы импортировали данные из текущего финансового решения.</span><span class="sxs-lookup"><span data-stu-id="5450f-173">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="5450f-174">Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.</span><span class="sxs-lookup"><span data-stu-id="5450f-174">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="5450f-175">Неверное название организации</span><span class="sxs-lookup"><span data-stu-id="5450f-175">Incorrect Company Name</span></span>  
<span data-ttu-id="5450f-176">Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации.</span><span class="sxs-lookup"><span data-stu-id="5450f-176">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="5450f-177">Чтобы найти название организации, найдите **Организации**.</span><span class="sxs-lookup"><span data-stu-id="5450f-177">To find the company name search for **Companies**.</span></span> <span data-ttu-id="5450f-178">Затем в поле **Название** введите название организации.</span><span class="sxs-lookup"><span data-stu-id="5450f-178">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="5450f-179">Неверные имя пользователя и пароль</span><span class="sxs-lookup"><span data-stu-id="5450f-179">Incorrect User Name and Password</span></span>  
<span data-ttu-id="5450f-180">Имя пользователя и пароль, используемые для подключения, аналогичны используемым для подключения к учетной записи Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="5450f-180">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="5450f-181">Также для пакетов содержимого требуется наличие учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="5450f-181">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="5450f-182">После ввода учетных данных будут автоматически обнаружены все арендаторы Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="5450f-182">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="5450f-183">Если у вас нет лицензированной или пробной учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], вы получите сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5450f-183">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="5450f-184">Ключ не соответствует ни одной из строк в таблице</span><span class="sxs-lookup"><span data-stu-id="5450f-184">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="5450f-185">Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице".</span><span class="sxs-lookup"><span data-stu-id="5450f-185">If you enter a non valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="5450f-186">Укажите правильное название организации и попробуйте подключиться снова.</span><span class="sxs-lookup"><span data-stu-id="5450f-186">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="5450f-187">См. также</span><span class="sxs-lookup"><span data-stu-id="5450f-187">See Also</span></span>
[<span data-ttu-id="5450f-188">Начало работы с Power BI</span><span class="sxs-lookup"><span data-stu-id="5450f-188">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
<span data-ttu-id="5450f-189">[Power BI — основные понятия](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="5450f-189">[Power BI - Basic Concepts](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Business Intelligence](bi.md)</span></span>  
<span data-ttu-id="5450f-190">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="5450f-190">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="5450f-191">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="5450f-191">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="5450f-192">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="5450f-192">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="5450f-193">Финансы</span><span class="sxs-lookup"><span data-stu-id="5450f-193">Finance</span></span>](finance.md)  
<span data-ttu-id="5450f-194">[Настройка отчетов для [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="5450f-194">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

