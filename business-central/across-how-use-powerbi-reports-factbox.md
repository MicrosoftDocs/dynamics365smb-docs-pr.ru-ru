---
title: Отображение пользовательских отчетов Power BI для данных Business Central
description: Можно использовать отчеты Power BI для сбора дополнительных сведений о данных в списках.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/26/2021
ms.author: jswymer
ms.openlocfilehash: d2ce2588604ae676ba8b2cb73878a2d8dfd32b63
ms.sourcegitcommit: 652e4b0e1a09bff265014d9f8eb3b038ab0db79e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2021
ms.locfileid: "6087698"
---
# <a name="creating-power-bi-reports-for-displaying-list-data-in-prod_short"></a><span data-ttu-id="52392-103">Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="52392-103">Creating Power BI Reports for Displaying List Data in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="52392-104">включает элемент управления информационной панели Power BI на многих ключевых страницах списка.</span><span class="sxs-lookup"><span data-stu-id="52392-104">includes a Power BI FactBox control element on many key list pages.</span></span> <span data-ttu-id="52392-105">Цель этой информационной панели — отображать отчеты Power BI, которые связаны с записями в списках, обеспечивая дополнительное понимание данных.</span><span class="sxs-lookup"><span data-stu-id="52392-105">The purpose of this FactBox is to display Power BI reports that are related to records in the lists, providing extra insight into the data.</span></span> <span data-ttu-id="52392-106">Идея заключается в том, что при перемещении между строками в списке отчет обновляется в соответствии с выбранной операцией.</span><span class="sxs-lookup"><span data-stu-id="52392-106">The idea is that as you move between rows in the list, the report updates for the selected entry.</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="52392-107">поставляется с некоторыми из этих отчетов.</span><span class="sxs-lookup"><span data-stu-id="52392-107">comes ready with some of these reports.</span></span> <span data-ttu-id="52392-108">Вы также можете создавать свои собственные пользовательские отчеты, которые будут отображаться на этой информационной панели.</span><span class="sxs-lookup"><span data-stu-id="52392-108">You can also create your own custom reports that display in this FactBox.</span></span> <span data-ttu-id="52392-109">Создание этих отчетов аналогично созданию других отчетов.</span><span class="sxs-lookup"><span data-stu-id="52392-109">Creating these reports is similar to other reports.</span></span> <span data-ttu-id="52392-110">Но есть несколько правил разработки, которым вы должны следовать, чтобы отчеты отображались должным образом.</span><span class="sxs-lookup"><span data-stu-id="52392-110">But there are a few design rules you'll have to follow to make sure the reports display as expected.</span></span> <span data-ttu-id="52392-111">Эти правила объясняются в этой статье.</span><span class="sxs-lookup"><span data-stu-id="52392-111">These rules are explained in this article.</span></span>

> [!NOTE]
> <span data-ttu-id="52392-112">Для получения общей информации о создании и публикации отчетов Power BI для Business Central см. раздел [Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md).</span><span class="sxs-lookup"><span data-stu-id="52392-112">For general information about creating and publishing Power BI reports for Business Central, see [Building Power BI Reports to Display [!INCLUDE [prod_long](includes/prod_long.md)] Data](across-how-use-financials-data-source-powerbi.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="52392-113">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="52392-113">Prerequisites</span></span>

- <span data-ttu-id="52392-114">Учетная запись Power BI.</span><span class="sxs-lookup"><span data-stu-id="52392-114">A Power BI account.</span></span>
- <span data-ttu-id="52392-115">Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="52392-115">Power BI Desktop.</span></span>

<!-- 
For more information about getting started, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md).-->

## <a name="create-a-report-for-a-list-page"></a><span data-ttu-id="52392-116">Создание отчета для страницы со списком</span><span class="sxs-lookup"><span data-stu-id="52392-116">Create a report for a list page</span></span>

1. <span data-ttu-id="52392-117">Запустите Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="52392-117">Start Power BI Desktop.</span></span>
2. <span data-ttu-id="52392-118">Выберите **Получить данные** и начните выбирать источник данных для отчета.</span><span class="sxs-lookup"><span data-stu-id="52392-118">Select **Get Data**, and start choosing the data source for the report.</span></span>

    <span data-ttu-id="52392-119">Укажите страницы списка Business Central, которые содержат данные, которые вы хотите включить в отчет.</span><span class="sxs-lookup"><span data-stu-id="52392-119">Specify the Business Central list pages that contain the data that you want in the report.</span></span> <span data-ttu-id="52392-120">Например, чтобы создать отчет для списка **Счета продажи**, включите страницы, относящиеся к продажам.</span><span class="sxs-lookup"><span data-stu-id="52392-120">For example, to create a report for the **Sales Invoices** list, include pages related to sales.</span></span>

    <span data-ttu-id="52392-121">Для получения дополнительной информации следуйте инструкциям раздела [Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span><span class="sxs-lookup"><span data-stu-id="52392-121">For more information, follow the instructions [Add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span></span>

3. <span data-ttu-id="52392-122">Задайте фильтр отчета.</span><span class="sxs-lookup"><span data-stu-id="52392-122">Set the report filter.</span></span>

    <span data-ttu-id="52392-123">Чтобы обновить данные для выбранной записи в списке, вы добавляете фильтр в отчет.</span><span class="sxs-lookup"><span data-stu-id="52392-123">To make the data update to the selected record in the list, you add a filter to the report.</span></span> <span data-ttu-id="52392-124">Фильтр должен включать поле источника данных, которое используется для уникальной идентификации каждой записи в списке.</span><span class="sxs-lookup"><span data-stu-id="52392-124">The filter must include a field of the data source that's used to uniquely identify each record in the list.</span></span> <span data-ttu-id="52392-125">С точки зрения разработчика это поле является *первичным ключом*.</span><span class="sxs-lookup"><span data-stu-id="52392-125">In developer terms, this field is the *primary key*.</span></span> <span data-ttu-id="52392-126">В большинстве случаев первичным ключом для списка является **Номер**.</span><span class="sxs-lookup"><span data-stu-id="52392-126">In most cases, the primary key for a list is the **No.**</span></span> <span data-ttu-id="52392-127">.</span><span class="sxs-lookup"><span data-stu-id="52392-127">field.</span></span>

    <span data-ttu-id="52392-128">Чтобы установить фильтр, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="52392-128">To set the filter, do the following steps:</span></span>

    1. <span data-ttu-id="52392-129">В области **Фильтры** выберите поле первичного ключа из списка доступных полей.</span><span class="sxs-lookup"><span data-stu-id="52392-129">In the **Filters**, select the primary key field from the list of available fields.</span></span>
    2. <span data-ttu-id="52392-130">Перетащите это поле в область **Фильтры** и поместите в поле **Фильтры на всех страницах**.</span><span class="sxs-lookup"><span data-stu-id="52392-130">Drag the field to **Filters** pane and drop it in the **Filters on all pages** box.</span></span>
    3. <span data-ttu-id="52392-131">Установите в параметре **Тип фильтра** значение **Простая фильтрация**.</span><span class="sxs-lookup"><span data-stu-id="52392-131">Set the **Filter type** to **Basic filtering**.</span></span> <span data-ttu-id="52392-132">Это не может быть страничный, визуальный или расширенный фильтр.</span><span class="sxs-lookup"><span data-stu-id="52392-132">It can't be page, visual, or advanced filter.</span></span>

    ![Настройка фильтра отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-filter-v3.png)
4. <span data-ttu-id="52392-134">Разработайте макет отчета.</span><span class="sxs-lookup"><span data-stu-id="52392-134">Design the report layout.</span></span>

    <span data-ttu-id="52392-135">Создайте макет, перетаскивая поля и добавляя визуализации.</span><span class="sxs-lookup"><span data-stu-id="52392-135">Create the layout by dragging fields and adding visualizations.</span></span> <span data-ttu-id="52392-136">Дополнительные сведения см. в разделе [Работа с представлением отчета в Power BI Desktop](/power-bi/create-reports/desktop-report-view) в документации по Power BI.</span><span class="sxs-lookup"><span data-stu-id="52392-136">For more information, see, [Work with Report view in Power BI Desktop](/power-bi/create-reports/desktop-report-view) in the Power BI documentation.</span></span>

5. <span data-ttu-id="52392-137">См. следующие разделы об изменении размера отчета и использовании нескольких страниц.</span><span class="sxs-lookup"><span data-stu-id="52392-137">See the next sections about sizing the report and using multiple pages.</span></span>

6. <span data-ttu-id="52392-138">Сохраните отчет и назовите его.</span><span class="sxs-lookup"><span data-stu-id="52392-138">Save and name the report.</span></span>

    <span data-ttu-id="52392-139">Дайте отчету имя, содержащее имя страницы списка, связанной с отчетом, как это сделано в клиенте.</span><span class="sxs-lookup"><span data-stu-id="52392-139">Give the report a name that contains the name of the list page associated with the report, as it is in the client.</span></span> <span data-ttu-id="52392-140">В имени регистр не учитывается.</span><span class="sxs-lookup"><span data-stu-id="52392-140">The name isn't case-sensitive though.</span></span> <span data-ttu-id="52392-141">Предположим, отчет предназначен для страницы списка **Счета продажи**.</span><span class="sxs-lookup"><span data-stu-id="52392-141">Suppose the report is for the **Sales Invoices** list page.</span></span> <span data-ttu-id="52392-142">В этом случае добавьте слова **счета продажи** где-нибудь в названии, например **my sales invoices.pbix** или **my_Sales Invoices_list.pbix**.</span><span class="sxs-lookup"><span data-stu-id="52392-142">In this case, include the words **sales invoices** somewhere in the name, like **my sales invoices.pbix** or **my_Sales Invoices_list.pbix**.</span></span>

    <span data-ttu-id="52392-143">Это соглашение об именах не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="52392-143">This naming convention isn't a requirement.</span></span> <span data-ttu-id="52392-144">Однако это делает выбор отчетов в [!INCLUDE[prod_short](includes/prod_short.md)] быстрее.</span><span class="sxs-lookup"><span data-stu-id="52392-144">However, it makes selecting reports in [!INCLUDE[prod_short](includes/prod_short.md)] quicker.</span></span> <span data-ttu-id="52392-145">Когда страница выбора отчета открывается со страницы списка, она автоматически применяет фильтр на основе имени страницы.</span><span class="sxs-lookup"><span data-stu-id="52392-145">When the report selection page opens from a list page, it's automatically applied a filter based on the page name.</span></span> <span data-ttu-id="52392-146">Синтаксис фильтра: `@*<caption>*`, как `@*Sales Invoices*`.</span><span class="sxs-lookup"><span data-stu-id="52392-146">The filter has the syntax: `@*<caption>*`,  like `@*Sales Invoices*`.</span></span> <span data-ttu-id="52392-147">Эта фильтрация выполняется для ограничения отображаемых отчетов.</span><span class="sxs-lookup"><span data-stu-id="52392-147">This filtering is done to limit the reports that are displayed.</span></span> <span data-ttu-id="52392-148">Пользователи могут удалить фильтр, чтобы получить полный список доступных отчетов в Power BI.</span><span class="sxs-lookup"><span data-stu-id="52392-148">Users can clear the filter to get a full list of reports available in Power BI.</span></span>

7. <span data-ttu-id="52392-149">Когда вы закончите, опубликуйте отчет как обычно.</span><span class="sxs-lookup"><span data-stu-id="52392-149">When you're done, publish the report as usual.</span></span>

    <span data-ttu-id="52392-150">Для получения дополнительной информации см. раздел [Публикация отчета](across-how-use-financials-data-source-powerbi.md#publish-reports).</span><span class="sxs-lookup"><span data-stu-id="52392-150">For more information, see [Publishing a Report](across-how-use-financials-data-source-powerbi.md#publish-reports).</span></span>

8. <span data-ttu-id="52392-151">Протестируйте отчет.</span><span class="sxs-lookup"><span data-stu-id="52392-151">Test the report.</span></span>

    <span data-ttu-id="52392-152">После того как отчет был опубликован в вашей рабочей области, он должен быть доступен на информационной панели Power BI на странице списка в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="52392-152">Once the report's been published to your workspace, it should be available from the Power BI FactBox on the list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

    <span data-ttu-id="52392-153">Чтобы протестировать его, выполните следующие шаги.</span><span class="sxs-lookup"><span data-stu-id="52392-153">To test it, do the following steps.</span></span>

    1. <span data-ttu-id="52392-154">Откройте [!INCLUDE[prod_short](includes/prod_short.md)] и перейдите на страницу списка.</span><span class="sxs-lookup"><span data-stu-id="52392-154">Open [!INCLUDE[prod_short](includes/prod_short.md)] and go to the list page.</span></span>
    2. <span data-ttu-id="52392-155">Если вы не видите информационную панель Power BI, перейдите на панель действий, затем выберите **Действия** > **Показать** > **Показать/скрыть отчеты Power BI**.</span><span class="sxs-lookup"><span data-stu-id="52392-155">If you don't see the Power BI FactBox, go the action bar, then select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>
    3. <span data-ttu-id="52392-156">На информационной панели Power BI выберите **Выбрать отчеты**, выберите поле **Включить** для отчета, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="52392-156">In the Power BI FactBox, select **Select Reports**, select the **Enable** box for the report, then select **OK**.</span></span>

    <span data-ttu-id="52392-157">Если отчет разработан правильно, он отображается.</span><span class="sxs-lookup"><span data-stu-id="52392-157">If designed correctly, the report displays.</span></span>  

## <a name="set-the-report-size-and-color"></a><span data-ttu-id="52392-158">Задание размера и цвета отчета</span><span class="sxs-lookup"><span data-stu-id="52392-158">Set the report size and color</span></span>

<span data-ttu-id="52392-159">Отчет должен иметь размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="52392-159">The size of the report must be set to 325 pixels by 310 pixels.</span></span> <span data-ttu-id="52392-160">Этот размер обеспечивает правильное масштабирование отчета в доступном пространстве элемента управления информационной панелью Power BI в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="52392-160">This size provides the proper scaling of the report in the available space of the Power BI FactBox control in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="52392-161">Чтобы определить размер отчета, поместите фокус вне области макета отчета, а затем щелкните значок валика.</span><span class="sxs-lookup"><span data-stu-id="52392-161">To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.</span></span>

![Настройка ширины и высоты отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-sizing-v3.png)

<span data-ttu-id="52392-163">Можно изменить ширину и высоту отчета, выбрав значение **Пользовательский** в поле **Тип**.</span><span class="sxs-lookup"><span data-stu-id="52392-163">You can change the width and height of the report by choosing **Custom** in the **Type** field.</span></span>

<span data-ttu-id="52392-164">Если необходимо, чтобы фон отчета смешивался с цветом фона элемента управления информационной панелью Power BI, задайте пользовательский цвет фона отчета как *#FFFFFF* (белый).</span><span class="sxs-lookup"><span data-stu-id="52392-164">If you want the background of the report to blend with the background color of the Power BI FactBox control, set report background color to *#FFFFFF* (white).</span></span> 

> [!TIP]
> <span data-ttu-id="52392-165">Используйте файл темы [!INCLUDE [prod_short](includes/prod_short.md)] для создания отчетов с тем же цветовым стилем, что и приложения [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="52392-165">Use the [!INCLUDE [prod_short](includes/prod_short.md)] theme file to build reports with the same color styling as the [!INCLUDE [prod_short](includes/prod_short.md)] apps.</span></span> <span data-ttu-id="52392-166">Дополнительные сведения см. в разделе [Использование темы отчета [!INCLUDE [prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-powerbi.md#theme).</span><span class="sxs-lookup"><span data-stu-id="52392-166">For more information, see [Using the [!INCLUDE [prod_short](includes/prod_short.md)] report theme](across-how-use-financials-data-source-powerbi.md#theme).</span></span>

## <a name="reports-with-multiple-pages"></a><span data-ttu-id="52392-167">Отчеты с несколькими страницами</span><span class="sxs-lookup"><span data-stu-id="52392-167">Reports with multiple pages</span></span>

<span data-ttu-id="52392-168">В Power BI можно создать один отчет с несколькими страницами.</span><span class="sxs-lookup"><span data-stu-id="52392-168">With Power BI, you can create a single report with multiple pages.</span></span> <span data-ttu-id="52392-169">Однако для отчетов, которые будут отображаться со страницами списков, мы не рекомендуем создавать более одной страницы.</span><span class="sxs-lookup"><span data-stu-id="52392-169">However, for reports that will display with list pages, we recommend that they don't have more than one page.</span></span> <span data-ttu-id="52392-170">На информационной панели Power BI отображается только первая страница вашего отчета.</span><span class="sxs-lookup"><span data-stu-id="52392-170">The Power BI FactBox will only show the first page of your report.</span></span>

## <a name="fixing-problems"></a><span data-ttu-id="52392-171">Устранение проблем</span><span class="sxs-lookup"><span data-stu-id="52392-171">Fixing problems</span></span>

<span data-ttu-id="52392-172">В этом разделе объясняется, как устранять проблемы, с которыми вы можете столкнуться при попытке просмотреть отчет Power BI для страницы списка в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="52392-172">This section explains how to fix problems that you might run into when you try to view a Power BI report for a list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

### <a name="you-cant-see-the-power-bi-factbox-on-a-list-page"></a><span data-ttu-id="52392-173">Вы не видите информационную панель Power BI на странице списка</span><span class="sxs-lookup"><span data-stu-id="52392-173">You can't see the Power BI FactBox on a list page</span></span>

<span data-ttu-id="52392-174">По умолчанию информационная панель Power BI скрыт от просмотра.</span><span class="sxs-lookup"><span data-stu-id="52392-174">By default, the Power BI FactBox is hidden from view.</span></span> <span data-ttu-id="52392-175">Чтобы показать информационную панель на странице, на панели действий выберите **Действия** > **Показать** > **Показать/скрыть отчеты Power BI**.</span><span class="sxs-lookup"><span data-stu-id="52392-175">To show the FactBox on a page, from the action bar, select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>

### <a name="you-cant-see-the-report-in-the-select-report-pane"></a><span data-ttu-id="52392-176">Вы не видите отчет на странице выбора отчета</span><span class="sxs-lookup"><span data-stu-id="52392-176">You can't see the report in the Select Report pane</span></span>

<span data-ttu-id="52392-177">В названии отчета нет названия страницы списка, которая отображается.</span><span class="sxs-lookup"><span data-stu-id="52392-177">The report's name doesn't contain the name of the list page that's being shown.</span></span> <span data-ttu-id="52392-178">Очистите фильтр, чтобы получить полный список доступных отчетов Power BI.</span><span class="sxs-lookup"><span data-stu-id="52392-178">Clear the filter to get a full list of Power BI reports available.</span></span>  

### <a name="report-is-loaded-but-blank-not-filtered-or-filtered-incorrectly"></a><span data-ttu-id="52392-179">Отчет загружен, но пуст, не отфильтрован или неправильно отфильтрован</span><span class="sxs-lookup"><span data-stu-id="52392-179">Report is loaded but blank, not filtered, or filtered incorrectly</span></span>

<span data-ttu-id="52392-180">Убедитесь, что фильтр отчета содержит правильный первичный ключ.</span><span class="sxs-lookup"><span data-stu-id="52392-180">Verify the report filter contains the right primary key.</span></span> <span data-ttu-id="52392-181">В большинстве случаев это поле **Номер**,</span><span class="sxs-lookup"><span data-stu-id="52392-181">In most cases, this field is the **No.**</span></span> <span data-ttu-id="52392-182">но в таблице **Операция ГК**, например, следует использовать поле **Номер операции**.</span><span class="sxs-lookup"><span data-stu-id="52392-182">field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field.</span></span>

### <a name="report-is-loaded-but-it-shows-a-page-you-didnt-expect"></a><span data-ttu-id="52392-183">Отчет загружен, но показывает страницу, которую вы не ожидали</span><span class="sxs-lookup"><span data-stu-id="52392-183">Report is loaded, but it shows a page you didn't expect</span></span>

<span data-ttu-id="52392-184">Убедитесь, что страница, которую вы хотите отобразить, является первой страницей в вашем отчете.</span><span class="sxs-lookup"><span data-stu-id="52392-184">Verify that the page you want displayed is the first page in your report.</span></span>  

### <a name="report-appears-with-an-unwanted-gray-boarder-or-its-too-small-or-too-large"></a><span data-ttu-id="52392-185">В отчетах отображаются ненужная серая граница, отчет слишком мал или слишком большой</span><span class="sxs-lookup"><span data-stu-id="52392-185">Report appears with an unwanted gray boarder, or it's too small or too large</span></span>

<span data-ttu-id="52392-186">Проверьте, что отчет имеет размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="52392-186">Verify that the report size is set to 325 pixels x 310 pixels.</span></span> <span data-ttu-id="52392-187">Сохраните отчет, а затем обновите страницу списка.</span><span class="sxs-lookup"><span data-stu-id="52392-187">Save the report, and then refresh the list page.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="52392-188">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="52392-188">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="52392-189">См. также</span><span class="sxs-lookup"><span data-stu-id="52392-189">See Also</span></span>

[<span data-ttu-id="52392-190">Включение бизнес-данных для Power BI</span><span class="sxs-lookup"><span data-stu-id="52392-190">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
<span data-ttu-id="52392-191">[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="52392-191">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
[<span data-ttu-id="52392-192">Подготовьтесь к ведению бизнеса</span><span class="sxs-lookup"><span data-stu-id="52392-192">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="52392-193">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="52392-193">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
[<span data-ttu-id="52392-194">Финансы</span><span class="sxs-lookup"><span data-stu-id="52392-194">Finance</span></span>](finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]