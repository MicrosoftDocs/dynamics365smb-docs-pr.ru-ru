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
ms.date: 04/03/2018
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 9cad9c7e2b54506e60af7d38d42f413599a44d01
ms.openlocfilehash: 7b9140611a47b8b823274763731cf000258c681e
ms.contentlocale: ru-ru
ms.lasthandoff: 04/03/2018

---
# <a name="connecting-power-bi-to-dynamics-365-business-central-content-packs"></a><span data-ttu-id="1ee76-103">Подключение Power BI к пакетам содержимого Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="1ee76-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span></span>
<span data-ttu-id="1ee76-104">Анализ данных Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] становится проще благодаря Power BI и пакетам содержимого Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="1ee76-105">Power BI извлекает ваши данные, а затем создает готовую панель мониторинга и отчеты на основе этих данных.</span><span class="sxs-lookup"><span data-stu-id="1ee76-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

<span data-ttu-id="1ee76-106">Вы должны иметь допустимую учетную запись в Dynamics 365 и Power BI.</span><span class="sxs-lookup"><span data-stu-id="1ee76-106">You must have a valid account with Dynamics 365 and with Power BI.</span></span> <span data-ttu-id="1ee76-107">Кроме того, необходимо загрузить [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/), если вы хотите создавать свои собственные отчеты Power BI.</span><span class="sxs-lookup"><span data-stu-id="1ee76-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span></span> <span data-ttu-id="1ee76-108">Для пакетов содержимого Power BI требуются разрешения к таблицам, из которых извлекаются данные.</span><span class="sxs-lookup"><span data-stu-id="1ee76-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="1ee76-109">Дополнительные сведения о требованиях см. ниже.</span><span class="sxs-lookup"><span data-stu-id="1ee76-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="1ee76-110">Подключение</span><span class="sxs-lookup"><span data-stu-id="1ee76-110">How to Connect</span></span>
1. <span data-ttu-id="1ee76-111">Выберите **Получить данные** в нижней части левой панели навигации.</span><span class="sxs-lookup"><span data-stu-id="1ee76-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="1ee76-112">![Переход к разделу "Получить данные"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="1ee76-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>

<span data-ttu-id="1ee76-113">Можно также начать работать из Dynamics 365 Business Edition.</span><span class="sxs-lookup"><span data-stu-id="1ee76-113">You may also get starting from within Dynamics 365 Business Edition.</span></span> <span data-ttu-id="1ee76-114">Из ролевого центра перейдите к пункту **Выбор отчета** части ролевого центра Power BI.</span><span class="sxs-lookup"><span data-stu-id="1ee76-114">From the role center, navigate to **Report Selection** in the Power BI Role Center part.</span></span> <span data-ttu-id="1ee76-115">Выберите на ленте **Сервис** или **Моя организация**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-115">Select either **Service** or **My Organization** from the ribbon.</span></span> <span data-ttu-id="1ee76-116">Когда выбрано одно из этих действий, производится переход к галерее "Организация" в Power BI или к библиотеке сервисов в Power BI, которые также будут отфильтрованы для отображения только соответствующих пакетов, имеющих отношение к [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-116">When either of these actions are selected, you will be taken to either the Organization gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span>

2. <span data-ttu-id="1ee76-117">В поле **Службы** выберите **Получить**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-117">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="1ee76-118">Откроется окно **AppSource** и **Приложения для приложений Power BI**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-118">This will open a window with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="1ee76-119">![Выбор пакетов содержимого из веб-служб](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="1ee76-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="1ee76-120">Выберите **Приложения** на вкладке **Приложения для приложений Power BI**, выберите требуемый пакет содержимого **Microsoft Dynamics 365 Business Central** и щелкните **Получить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="1ee76-121">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="1ee76-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="1ee76-122">При появлении запроса ведите имя *вашей организации* в [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="1ee76-123">Это не отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1ee76-123">This is not the display name.</span></span> <span data-ttu-id="1ee76-124">Название организации можно найти на странице "Организации" в вашем экземпляре [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span></span> 
<span data-ttu-id="1ee76-125">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="1ee76-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="1ee76-126">После подключения панель мониторинга, отчет и набор данных будут автоматически отправлены в рабочую область Power BI.</span><span class="sxs-lookup"><span data-stu-id="1ee76-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="1ee76-127">По завершении плитки обновятся для отображения данных из вашей организации [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span></span>
<span data-ttu-id="1ee76-128">![Выберите Dynamics 365 Business Central и выберите "Получить сейчас"](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="1ee76-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="1ee76-129">Что теперь?</span><span class="sxs-lookup"><span data-stu-id="1ee76-129">What Now?</span></span>

- <span data-ttu-id="1ee76-130">Попробуйте [задать вопрос в поле "Вопросы и ответы"](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) вверху панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="1ee76-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span></span>
- <span data-ttu-id="1ee76-131">[Измените плитки](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) на панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="1ee76-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="1ee76-132">[Выберите плитку](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles), чтобы открыть основной отчет.</span><span class="sxs-lookup"><span data-stu-id="1ee76-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="1ee76-133">Хотя набор данных будет обновляться ежедневно, можно изменить график обновлений или попытаться обновить его по требованию с помощью функции **Обновить сейчас**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="1ee76-134">Требования к системе</span><span class="sxs-lookup"><span data-stu-id="1ee76-134">System Requirements</span></span>
<span data-ttu-id="1ee76-135">Чтобы импортировать данные [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] в Power BI, необходимо иметь разрешения на доступ к веб-службам, используемым для извлечения данных.</span><span class="sxs-lookup"><span data-stu-id="1ee76-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="1ee76-136">Веб-службы, необходимые для каждого пакета содержимого:</span><span class="sxs-lookup"><span data-stu-id="1ee76-136">The web services required for each content pack include:</span></span>

## <a name="role-center-reports"></a><span data-ttu-id="1ee76-137">Отчеты ролевого центра</span><span class="sxs-lookup"><span data-stu-id="1ee76-137">Role Center Reports</span></span>

<span data-ttu-id="1ee76-138">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="1ee76-138">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="1ee76-139">Возможности продаж</span><span class="sxs-lookup"><span data-stu-id="1ee76-139">Sales Opportunities</span></span>
- <span data-ttu-id="1ee76-140">Организация для просмотра шаблона Excel</span><span class="sxs-lookup"><span data-stu-id="1ee76-140">Excel Template View Company</span></span>
- <span data-ttu-id="1ee76-141">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-141">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-142">**Microsoft Dynamics 365 Business Central – Finance**</span><span class="sxs-lookup"><span data-stu-id="1ee76-142">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="1ee76-143">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="1ee76-143">PowerBIFinance</span></span>
- <span data-ttu-id="1ee76-144">Организация для просмотра шаблона Excel</span><span class="sxs-lookup"><span data-stu-id="1ee76-144">Excel Template View Company</span></span>
- <span data-ttu-id="1ee76-145">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-145">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-146">**Microsoft Dynamics 365 Business Central – Jobs**</span><span class="sxs-lookup"><span data-stu-id="1ee76-146">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="1ee76-147">Список работ</span><span class="sxs-lookup"><span data-stu-id="1ee76-147">Job List</span></span>
- <span data-ttu-id="1ee76-148">Строки планирования работ</span><span class="sxs-lookup"><span data-stu-id="1ee76-148">Job Planning Lines</span></span>
- <span data-ttu-id="1ee76-149">Строки рабочего задания</span><span class="sxs-lookup"><span data-stu-id="1ee76-149">Job Task Lines</span></span>
- <span data-ttu-id="1ee76-150">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-150">Power BI Report Labels</span></span>
- <span data-ttu-id="1ee76-151">Организация для просмотра шаблона Excel</span><span class="sxs-lookup"><span data-stu-id="1ee76-151">Excel Template View Company</span></span>

<span data-ttu-id="1ee76-152">**Microsoft Dynamics 365 Business Central - Sales**</span><span class="sxs-lookup"><span data-stu-id="1ee76-152">**Microsoft Dynamics 365 Business Central - Sales**</span></span>
- <span data-ttu-id="1ee76-153">Панель мониторинга продажи</span><span class="sxs-lookup"><span data-stu-id="1ee76-153">Sales Dashboard</span></span>
- <span data-ttu-id="1ee76-154">Организация для просмотра шаблона Excel</span><span class="sxs-lookup"><span data-stu-id="1ee76-154">Excel Template View Company</span></span>
- <span data-ttu-id="1ee76-155">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-155">Power BI Report Labels</span></span>

## <a name="list-page-reports"></a><span data-ttu-id="1ee76-156">Список отчетов страниц</span><span class="sxs-lookup"><span data-stu-id="1ee76-156">List Page Reports</span></span> 

<span data-ttu-id="1ee76-157">**Microsoft Dynamics 365 Business Central – Customers List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-157">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="1ee76-158">Продажа товаров по клиенту</span><span class="sxs-lookup"><span data-stu-id="1ee76-158">Item Sales by Customer</span></span>
- <span data-ttu-id="1ee76-159">Список покупок товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-159">Power BI Item Purchase List</span></span>
- <span data-ttu-id="1ee76-160">Список продаж товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-160">Power BI Item Sales List</span></span>
- <span data-ttu-id="1ee76-161">Панель мониторинга продажи</span><span class="sxs-lookup"><span data-stu-id="1ee76-161">Sales Dashboard</span></span>
- <span data-ttu-id="1ee76-162">Список клиентов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-162">Power BI Customer List</span></span>
- <span data-ttu-id="1ee76-163">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-163">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-164">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-164">Power BI Report Labels</span></span> 

<span data-ttu-id="1ee76-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span></span>
- <span data-ttu-id="1ee76-166">Список сумм ГК Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-166">Power BI GL Amount List</span></span>
- <span data-ttu-id="1ee76-167">Сумма бюджета ГК Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-167">Power BI GL Budgeted Amount</span></span>
- <span data-ttu-id="1ee76-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-168">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-169">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-169">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-170">**Microsoft Dynamics 365 Business Central – Items List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-170">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="1ee76-171">Продажа товаров по клиенту</span><span class="sxs-lookup"><span data-stu-id="1ee76-171">Item Sales by Customer</span></span>
- <span data-ttu-id="1ee76-172">Список покупок товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-172">Power BI Item Purchase List</span></span>
- <span data-ttu-id="1ee76-173">Список продаж товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-173">Power BI Item Sales List</span></span>
- <span data-ttu-id="1ee76-174">Панель мониторинга продажи</span><span class="sxs-lookup"><span data-stu-id="1ee76-174">Sales Dashboard</span></span>
- <span data-ttu-id="1ee76-175">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-175">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-176">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-176">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span></span>
- <span data-ttu-id="1ee76-178">Список работ Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-178">Power BI Jobs List</span></span>
- <span data-ttu-id="1ee76-179">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-179">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-180">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-180">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span></span>
- <span data-ttu-id="1ee76-182">Список покупок Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-182">Power BI Purchase List</span></span>
- <span data-ttu-id="1ee76-183">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-183">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-184">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-184">Power BI Report Labels</span></span>

<span data-ttu-id="1ee76-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span></span>
- <span data-ttu-id="1ee76-186">Список продаж Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-186">Power BI Sales List</span></span>
- <span data-ttu-id="1ee76-187">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-187">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-188">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-188">Power BI Report Labels</span></span>


<span data-ttu-id="1ee76-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span><span class="sxs-lookup"><span data-stu-id="1ee76-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="1ee76-190">Список покупок товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-190">Power BI Item Purchase List</span></span>
- <span data-ttu-id="1ee76-191">Список продаж товаров Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-191">Power BI Item Sales List</span></span>
- <span data-ttu-id="1ee76-192">Список поставщиков Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-192">Power BI Vendor List</span></span>
- <span data-ttu-id="1ee76-193">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="1ee76-193">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="1ee76-194">Метки отчетов Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-194">Power BI Report Labels</span></span>

## <a name="web-services"></a><span data-ttu-id="1ee76-195">Веб-службы</span><span class="sxs-lookup"><span data-stu-id="1ee76-195">Web Services</span></span>
<span data-ttu-id="1ee76-196">Простой способ найти веб-службы — найти веб-службы в [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="1ee76-197">В списке проверьте, что установлен флажок "Опубликовать" для веб-служб, перечисленных выше.</span><span class="sxs-lookup"><span data-stu-id="1ee76-197">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1ee76-198">Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="1ee76-198">Troubleshooting</span></span>
<span data-ttu-id="1ee76-199">Панель мониторинга Power BI основана на опубликованных веб-службах, которые перечислены выше, и содержит данные демонстрационной организации или вашей организации, если вы импортировали данные из текущего финансового решения.</span><span class="sxs-lookup"><span data-stu-id="1ee76-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="1ee76-200">Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.</span><span class="sxs-lookup"><span data-stu-id="1ee76-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="1ee76-201">Неверное название организации</span><span class="sxs-lookup"><span data-stu-id="1ee76-201">Incorrect Company Name</span></span>  
<span data-ttu-id="1ee76-202">Распространенной ошибкой является ввод отображаемого имени организации вместо названия организации.</span><span class="sxs-lookup"><span data-stu-id="1ee76-202">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="1ee76-203">Чтобы найти название организации, найдите **Организации**.</span><span class="sxs-lookup"><span data-stu-id="1ee76-203">To find the company name search for **Companies**.</span></span> <span data-ttu-id="1ee76-204">Затем в поле **Название** введите название организации.</span><span class="sxs-lookup"><span data-stu-id="1ee76-204">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="1ee76-205">Неверные имя пользователя и пароль</span><span class="sxs-lookup"><span data-stu-id="1ee76-205">Incorrect User Name and Password</span></span>  
<span data-ttu-id="1ee76-206">Имя пользователя и пароль, используемые для подключения, аналогичны используемым для подключения к учетной записи Microsoft Office 365.</span><span class="sxs-lookup"><span data-stu-id="1ee76-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="1ee76-207">Также для пакетов содержимого требуется наличие учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="1ee76-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="1ee76-208">После ввода учетных данных будут автоматически обнаружены все арендаторы Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], к которым у вас есть доступ.</span><span class="sxs-lookup"><span data-stu-id="1ee76-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="1ee76-209">Если у вас нет лицензированной или пробной учетной записи Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)], вы получите сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="1ee76-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="1ee76-210">Ключ не соответствует ни одной из строк в таблице</span><span class="sxs-lookup"><span data-stu-id="1ee76-210">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="1ee76-211">Если ввести недействительное имя организации в процессе подключения, можно получить сообщение об ошибке "Ключ не соответствует ни одной из строк в таблице".</span><span class="sxs-lookup"><span data-stu-id="1ee76-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="1ee76-212">Укажите правильное название организации и попробуйте подключиться снова.</span><span class="sxs-lookup"><span data-stu-id="1ee76-212">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="1ee76-213">См. также</span><span class="sxs-lookup"><span data-stu-id="1ee76-213">See Also</span></span>
[<span data-ttu-id="1ee76-214">Начало работы с Power BI</span><span class="sxs-lookup"><span data-stu-id="1ee76-214">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
[<span data-ttu-id="1ee76-215">Power BI — основные понятия</span><span class="sxs-lookup"><span data-stu-id="1ee76-215">Power BI - Basic Concepts</span></span>](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)  
[<span data-ttu-id="1ee76-216">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="1ee76-216">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="1ee76-217">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="1ee76-217">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="1ee76-218">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="1ee76-218">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="1ee76-219">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="1ee76-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="1ee76-220">Финансы</span><span class="sxs-lookup"><span data-stu-id="1ee76-220">Finance</span></span>](finance.md)  
<span data-ttu-id="1ee76-221">[Настройка отчетов для [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="1ee76-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  

