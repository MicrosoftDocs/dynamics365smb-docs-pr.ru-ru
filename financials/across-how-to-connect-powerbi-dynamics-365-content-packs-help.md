---
title: "Подключение Power BI к Finance and Operations, Business edition | Microsoft Docs"
description: "Анализ данных, бизнес-аналитика и КПЭ на основе данных Finance and Operations, Business edition становятся проще благодаря пакетам содержимого Power BI и Finance and Operations, Business edition."
author: SusanneWindfeldPedersen
ms.service: dynamics365-financials
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 02/05/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: b4e2e7bc1c2622d329c73ae5bf47b4accff10aa8
ms.openlocfilehash: aff8d95b13f795fa12d3146e5613712fb3baf9b4
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-power-bi-to-finance-and-operations-business-edition-content-packs"></a><span data-ttu-id="37fb3-103">Подключение Power BI к пакетам содержимого Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="37fb3-103">Connecting Power BI to Finance and Operations, Business edition Content Packs</span></span>
<span data-ttu-id="37fb3-104">Анализ данных Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] становится проще благодаря Power BI и пакетам содержимого Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="37fb3-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="37fb3-105">Power BI извлекает ваши данные, а затем создает готовую панель мониторинга и отчеты на основе этих данных.</span><span class="sxs-lookup"><span data-stu-id="37fb3-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

> [!NOTE]  
>  <span data-ttu-id="37fb3-106">Вы должны иметь допустимую учетную запись в Dynamics 365 и Power BI.</span><span class="sxs-lookup"><span data-stu-id="37fb3-106">You must have a valid account with Dynamics 365 and with Power BI.</span></span> <span data-ttu-id="37fb3-107">Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span><span class="sxs-lookup"><span data-stu-id="37fb3-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  
>  <span data-ttu-id="37fb3-108">Для пакетов содержимого Power BI требуются разрешения к таблицам, из которых извлекаются данные.</span><span class="sxs-lookup"><span data-stu-id="37fb3-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="37fb3-109">Дополнительные сведения о требованиях см. ниже.</span><span class="sxs-lookup"><span data-stu-id="37fb3-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="37fb3-110">Подключение</span><span class="sxs-lookup"><span data-stu-id="37fb3-110">How to Connect</span></span>
1. <span data-ttu-id="37fb3-111">Выберите **Получить данные** в нижней части левой панели навигации.</span><span class="sxs-lookup"><span data-stu-id="37fb3-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="37fb3-112">![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="37fb3-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>
2. <span data-ttu-id="37fb3-113">В поле **Службы** выберите **Получить**.</span><span class="sxs-lookup"><span data-stu-id="37fb3-113">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="37fb3-114">Откроется окно **AppSource** и **Приложения для приложений Power BI**.</span><span class="sxs-lookup"><span data-stu-id="37fb3-114">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="37fb3-115">![Выбор пакетов содержимого из веб-служб](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="37fb3-115">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="37fb3-116">Выберите **Приложения** на вкладке **Приложения для приложений Power BI**, выберите требуемый пакет содержимого **Microsoft Dynamics 365 for Finance and Operations** и щелкните **Получить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="37fb3-116">Select **Apps** from the **Apps for Power BI apps** tab, and choose the **Microsoft Dynamics 365 for Finance and Operations** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="37fb3-117">![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="37fb3-117">![Select Dynamics 365 for Finance and Operations, Business edition and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="37fb3-118">При появлении запроса ведите имя *вашей организации* в [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="37fb3-118">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="37fb3-119">Это не отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="37fb3-119">This is not the display name.</span></span>  
<span data-ttu-id="37fb3-120">![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="37fb3-120">![Select Dynamics 365 for Finance and Operations, Business edition and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="37fb3-121">После подключения панель мониторинга, отчет и набор данных будут автоматически отправлены в рабочую область Power BI.</span><span class="sxs-lookup"><span data-stu-id="37fb3-121">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="37fb3-122">По завершении плитки обновятся для отображения данных из учетной записи.</span><span class="sxs-lookup"><span data-stu-id="37fb3-122">When completed, the tiles will update with data from your account.</span></span>
<span data-ttu-id="37fb3-123">![Выбор Dynamics 365 for Finance and Operations, Business edition и выбор "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="37fb3-123">![Select Dynamics 365 for Finance and Operations, Business edition  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="37fb3-124">Что теперь?</span><span class="sxs-lookup"><span data-stu-id="37fb3-124">What Now?</span></span>

- <span data-ttu-id="37fb3-125">Попробуйте [задать вопрос в поле "Вопросы и ответы"](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) вверху панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="37fb3-125">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span></span>  
- <span data-ttu-id="37fb3-126">[Измените плитки](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) на панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="37fb3-126">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="37fb3-127">[Выберите плитку](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.</span><span class="sxs-lookup"><span data-stu-id="37fb3-127">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="37fb3-128">Хотя набор данных будет обновляться ежедневно, можно изменить график обновлений или попытаться обновить его по требованию с помощью функции **Обновить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="37fb3-128">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="37fb3-129">Требования к системе</span><span class="sxs-lookup"><span data-stu-id="37fb3-129">System Requirements</span></span>
<span data-ttu-id="37fb3-130">Чтобы импортировать данные [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных.</span><span class="sxs-lookup"><span data-stu-id="37fb3-130">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="37fb3-131">Веб-службы, необходимые для каждого пакета содержимого:</span><span class="sxs-lookup"><span data-stu-id="37fb3-131">The web services required for each content pack include:</span></span>

<span data-ttu-id="37fb3-132">**Microsoft Dynamics 365 for Finance and Operations, Business edition – CRM**</span><span class="sxs-lookup"><span data-stu-id="37fb3-132">**Microsoft Dynamics 365 for Finance and Operations, Business edition – CRM**</span></span>
- <span data-ttu-id="37fb3-133">SalesOpportunities</span><span class="sxs-lookup"><span data-stu-id="37fb3-133">SalesOpportunities</span></span>
- <span data-ttu-id="37fb3-134">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-134">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="37fb3-135">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Sales**</span><span class="sxs-lookup"><span data-stu-id="37fb3-135">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Sales**</span></span>
- <span data-ttu-id="37fb3-136">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="37fb3-136">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="37fb3-137">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="37fb3-137">SalesDashboard</span></span>
- <span data-ttu-id="37fb3-138">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-138">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="37fb3-139">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Finance**</span><span class="sxs-lookup"><span data-stu-id="37fb3-139">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Finance**</span></span>
- <span data-ttu-id="37fb3-140">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="37fb3-140">PowerBIFinance</span></span>
- <span data-ttu-id="37fb3-141">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-141">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="37fb3-142">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Jobs**</span><span class="sxs-lookup"><span data-stu-id="37fb3-142">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Jobs**</span></span>
- <span data-ttu-id="37fb3-143">Список работ</span><span class="sxs-lookup"><span data-stu-id="37fb3-143">Job List</span></span>
- <span data-ttu-id="37fb3-144">Строки планирования работ</span><span class="sxs-lookup"><span data-stu-id="37fb3-144">Job Planning Lines</span></span>
- <span data-ttu-id="37fb3-145">Строки рабочего задания</span><span class="sxs-lookup"><span data-stu-id="37fb3-145">Job Task Lines</span></span>

<span data-ttu-id="37fb3-146">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список клиентов**</span><span class="sxs-lookup"><span data-stu-id="37fb3-146">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Customers List**</span></span>
- <span data-ttu-id="37fb3-147">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="37fb3-147">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="37fb3-148">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-148">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="37fb3-149">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-149">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="37fb3-150">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="37fb3-150">SalesDashboard</span></span>
- <span data-ttu-id="37fb3-151">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-151">Power_BI_Customer_List</span></span>
- <span data-ttu-id="37fb3-152">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-152">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="37fb3-153">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список товаров**</span><span class="sxs-lookup"><span data-stu-id="37fb3-153">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Items List**</span></span>
- <span data-ttu-id="37fb3-154">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="37fb3-154">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="37fb3-155">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-155">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="37fb3-156">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-156">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="37fb3-157">Товаров</span><span class="sxs-lookup"><span data-stu-id="37fb3-157">Items</span></span>
- <span data-ttu-id="37fb3-158">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="37fb3-158">SalesDashboard</span></span>
- <span data-ttu-id="37fb3-159">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-159">ExcelTemplateViewCompany</span></span>

<span data-ttu-id="37fb3-160">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Список поставщиков**</span><span class="sxs-lookup"><span data-stu-id="37fb3-160">**Microsoft Dynamics 365 for Finance and Operations, Business edition – Vendors List**</span></span>
- <span data-ttu-id="37fb3-161">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="37fb3-161">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="37fb3-162">Power_BI_Item_Purchase_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-162">Power_BI_Item_Purchase_List</span></span>
- <span data-ttu-id="37fb3-163">Power_BI_Item_Sales_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-163">Power_BI_Item_Sales_List</span></span>
- <span data-ttu-id="37fb3-164">Товаров</span><span class="sxs-lookup"><span data-stu-id="37fb3-164">Items</span></span>
- <span data-ttu-id="37fb3-165">SalesDashboard</span><span class="sxs-lookup"><span data-stu-id="37fb3-165">SalesDashboard</span></span>
- <span data-ttu-id="37fb3-166">Power_BI_Customer_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-166">Power_BI_Customer_List</span></span>
- <span data-ttu-id="37fb3-167">ItemSalesbyCustomer</span><span class="sxs-lookup"><span data-stu-id="37fb3-167">ItemSalesbyCustomer</span></span>
- <span data-ttu-id="37fb3-168">Power_BI_Vendor_List</span><span class="sxs-lookup"><span data-stu-id="37fb3-168">Power_BI_Vendor_List</span></span>
- <span data-ttu-id="37fb3-169">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="37fb3-169">ExcelTemplateViewCompany</span></span>

## <a name="web-services"></a><span data-ttu-id="37fb3-170">Веб-службы</span><span class="sxs-lookup"><span data-stu-id="37fb3-170">Web Services</span></span>
<span data-ttu-id="37fb3-171">Простой способ найти веб-службы — найти веб-службы в [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="37fb3-171">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="37fb3-172">В списке проверьте, что установлен флажок "Опубликовать" для веб-служб, перечисленных выше.</span><span class="sxs-lookup"><span data-stu-id="37fb3-172">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="37fb3-173">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="37fb3-173">Troubleshooting</span></span>
<span data-ttu-id="37fb3-174">Панель мониторинга Power BI основана на опубликованных веб-службах, которые перечислены выше, и содержит данные демонстрационной организации или вашей организации, если вы импортировали данные из текущего финансового решения.</span><span class="sxs-lookup"><span data-stu-id="37fb3-174">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="37fb3-175">Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.</span><span class="sxs-lookup"><span data-stu-id="37fb3-175">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="37fb3-176">Неверное название организации</span><span class="sxs-lookup"><span data-stu-id="37fb3-176">Incorrect Company Name</span></span>  
<span data-ttu-id="37fb3-177">Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации.</span><span class="sxs-lookup"><span data-stu-id="37fb3-177">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="37fb3-178">Чтобы найти название организации, найдите **Организации**.</span><span class="sxs-lookup"><span data-stu-id="37fb3-178">To find the company name search for **Companies**.</span></span> <span data-ttu-id="37fb3-179">Затем в поле **Название** введите название организации.</span><span class="sxs-lookup"><span data-stu-id="37fb3-179">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="37fb3-180">Неверные имя пользователя и пароль</span><span class="sxs-lookup"><span data-stu-id="37fb3-180">Incorrect User Name and Password</span></span>  
<span data-ttu-id="37fb3-181">Имя пользователя и пароль, используемые для подключения, аналогичны используемым для подключения к учетной записи Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="37fb3-181">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="37fb3-182">Также для пакетов содержимого требуется наличие учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="37fb3-182">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="37fb3-183">После ввода учетных данных будут автоматически обнаружены все арендаторы Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="37fb3-183">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="37fb3-184">Если у вас нет лицензированной или пробной учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], вы получите сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="37fb3-184">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="37fb3-185">Ключ не соответствует ни одной из строк в таблице</span><span class="sxs-lookup"><span data-stu-id="37fb3-185">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="37fb3-186">Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице".</span><span class="sxs-lookup"><span data-stu-id="37fb3-186">If you enter a non valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="37fb3-187">Укажите правильное название организации и попробуйте подключиться снова.</span><span class="sxs-lookup"><span data-stu-id="37fb3-187">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="37fb3-188">См. также</span><span class="sxs-lookup"><span data-stu-id="37fb3-188">See Also</span></span>
[<span data-ttu-id="37fb3-189">Начало работы с Power BI</span><span class="sxs-lookup"><span data-stu-id="37fb3-189">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
<span data-ttu-id="37fb3-190">[Power BI — основные понятия](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Бизнес-аналитика](bi.md)</span><span class="sxs-lookup"><span data-stu-id="37fb3-190">[Power BI - Basic Concepts](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)
[Business Intelligence](bi.md)</span></span>  
<span data-ttu-id="37fb3-191">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="37fb3-191">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="37fb3-192">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="37fb3-192">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="37fb3-193">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="37fb3-193">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="37fb3-194">Финансы</span><span class="sxs-lookup"><span data-stu-id="37fb3-194">Finance</span></span>](finance.md)  
<span data-ttu-id="37fb3-195">[Настройка отчетов для [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="37fb3-195">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

