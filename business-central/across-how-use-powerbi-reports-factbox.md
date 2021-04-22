---
title: Отображение пользовательских отчетов Power BI для данных Business Central | Документация Майкрософт
description: Можно использовать отчеты Power BI для сбора дополнительных сведений о данных в списках.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a600b24e16172134d4f8e78cf47efa4e262cac09
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5777520"
---
# <a name="creating-power-bi-reports-for-displaying-list-data-in-prod_short"></a><span data-ttu-id="9cbed-103">Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prod_short](includes/prod_short.md)]</span><span class="sxs-lookup"><span data-stu-id="9cbed-103">Creating Power BI Reports for Displaying List Data in [!INCLUDE[prod_short](includes/prod_short.md)]</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="9cbed-104">включает элемент управления информационной панели Power BI на многих ключевых страницах списка.</span><span class="sxs-lookup"><span data-stu-id="9cbed-104">includes a Power BI FactBox control element on many key list pages.</span></span> <span data-ttu-id="9cbed-105">Цель этой информационной панели — отображать отчеты Power BI, которые связаны с записями в списках, обеспечивая дополнительное понимание данных.</span><span class="sxs-lookup"><span data-stu-id="9cbed-105">The purpose of this FactBox is to display Power BI reports that are related to records in the lists, providing extra insight into the data.</span></span> <span data-ttu-id="9cbed-106">Идея заключается в том, что при перемещении между строками в списке отчет обновляется и фильтруется в соответствии с выбранной операцией.</span><span class="sxs-lookup"><span data-stu-id="9cbed-106">The idea is that as you move between rows in the list, the report is updated and filtered for the selected entry.</span></span>

[!INCLUDE[prod_long](includes/prod_long.md)] <span data-ttu-id="9cbed-107">поставляется с некоторыми из этих отчетов.</span><span class="sxs-lookup"><span data-stu-id="9cbed-107">comes ready with some of these reports.</span></span> <span data-ttu-id="9cbed-108">Вы также можете создавать свои собственные пользовательские отчеты, которые будут отображаться на этой информационной панели.</span><span class="sxs-lookup"><span data-stu-id="9cbed-108">You can also create your own custom reports that display in this FactBox.</span></span> <span data-ttu-id="9cbed-109">Создание этих отчетов аналогично созданию других отчетов.</span><span class="sxs-lookup"><span data-stu-id="9cbed-109">Creating these reports is similar to other reports.</span></span> <span data-ttu-id="9cbed-110">Но есть несколько правил разработки, которым вы должны следовать, чтобы отчеты отображались должным образом.</span><span class="sxs-lookup"><span data-stu-id="9cbed-110">But there are a few design rules you'll have to follow to make sure the reports display as expected.</span></span> <span data-ttu-id="9cbed-111">Эти правила объясняются в этой статье.</span><span class="sxs-lookup"><span data-stu-id="9cbed-111">These rules are explained in this article.</span></span>

> [!NOTE]
> <span data-ttu-id="9cbed-112">Для получения общей информации о создании и публикации отчетов Power BI для Business Central см. раздел [Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md).</span><span class="sxs-lookup"><span data-stu-id="9cbed-112">For general information about creating and publishing Power BI reports for Business Central, see [Building Power BI Reports to Display [!INCLUDE [prod_long](includes/prod_long.md)] Data](across-how-use-financials-data-source-powerbi.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="9cbed-113">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="9cbed-113">Prerequisites</span></span>

- <span data-ttu-id="9cbed-114">Учетная запись Power BI.</span><span class="sxs-lookup"><span data-stu-id="9cbed-114">A Power BI account.</span></span>
- <span data-ttu-id="9cbed-115">Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="9cbed-115">Power BI Desktop.</span></span>

<!-- 
For more information about getting started, see [Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md).-->

## <a name="create-a-report-for-a-list-page"></a><span data-ttu-id="9cbed-116">Создание отчета для страницы со списком</span><span class="sxs-lookup"><span data-stu-id="9cbed-116">Create a report for a list page</span></span>

1. <span data-ttu-id="9cbed-117">Запустите Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="9cbed-117">Start Power BI Desktop.</span></span>
2. <span data-ttu-id="9cbed-118">Выберите **Получить данные** и начните выбирать источник данных для отчета.</span><span class="sxs-lookup"><span data-stu-id="9cbed-118">Select **Get Data**, and start choosing the data source for the report.</span></span>

    <span data-ttu-id="9cbed-119">На этом шаге вы указываете страницы списка Business Central, которые содержат данные, которые вы хотите включить в отчет.</span><span class="sxs-lookup"><span data-stu-id="9cbed-119">In this step, you specify the Business Central list pages that contain the data that you want in the report.</span></span> <span data-ttu-id="9cbed-120">Например, чтобы создать отчет для списка продаж, убедитесь, что набор данных содержит информацию, связанную с продажами.</span><span class="sxs-lookup"><span data-stu-id="9cbed-120">For example, to create a report for the Sales List, ensure the data set contains information related to sales.</span></span>

    <span data-ttu-id="9cbed-121">Для получения дополнительной информации следуйте инструкциям раздела [Добавление [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных в Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span><span class="sxs-lookup"><span data-stu-id="9cbed-121">For more information, follow the instructions [Add [!INCLUDE[prod_short](includes/prod_short.md)] as a data source in Power BI Desktop](across-how-use-financials-data-source-powerbi.md#getdata).</span></span>

3. <span data-ttu-id="9cbed-122">Задайте фильтр отчета.</span><span class="sxs-lookup"><span data-stu-id="9cbed-122">Set the report filter.</span></span>

    <span data-ttu-id="9cbed-123">Чтобы обновить данные для выбранной записи в списке, вы добавляете фильтр в отчет.</span><span class="sxs-lookup"><span data-stu-id="9cbed-123">To make the data update to the selected record in the list, you add a filter to the report.</span></span> <span data-ttu-id="9cbed-124">Фильтр должен включать поле источника данных, которое используется для уникальной идентификации каждой записи в списке.</span><span class="sxs-lookup"><span data-stu-id="9cbed-124">The filter must include a field of the data source that's used to uniquely identify each record in the list.</span></span> <span data-ttu-id="9cbed-125">С точки зрения разработчика это поле является *первичным ключом*.</span><span class="sxs-lookup"><span data-stu-id="9cbed-125">In developer terms, this field is the *primary key*.</span></span> <span data-ttu-id="9cbed-126">В большинстве случаев первичным ключом для списка является **Номер**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-126">In most cases, the primary key for a list is the **No.**</span></span> <span data-ttu-id="9cbed-127">.</span><span class="sxs-lookup"><span data-stu-id="9cbed-127">field.</span></span>

    <span data-ttu-id="9cbed-128">Чтобы установить фильтр, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="9cbed-128">To set the filter, do the following steps:</span></span>

    1. <span data-ttu-id="9cbed-129">В области **Фильтры** выберите поле первичного ключа из списка доступных полей.</span><span class="sxs-lookup"><span data-stu-id="9cbed-129">In the **Filters**, select the primary key field from the list of available fields.</span></span>
    2. <span data-ttu-id="9cbed-130">Перетащите это поле в область **Фильтры** и поместите в поле **Фильтры на всех страницах**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-130">Drag the field to **Filters** pane and drop it in the **Filters on all pages** box.</span></span>
    3. <span data-ttu-id="9cbed-131">Установите в параметре **Тип фильтра** значение **Простая фильтрация**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-131">Set the **Filter type** to **Basic filtering**.</span></span> <span data-ttu-id="9cbed-132">Это не может быть страничный, визуальный или расширенный фильтр.</span><span class="sxs-lookup"><span data-stu-id="9cbed-132">It can't be page, visual, or advanced filter.</span></span>

    ![Настройка фильтра отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-filter-v3.png)
4. <span data-ttu-id="9cbed-134">Разработайте макет отчета.</span><span class="sxs-lookup"><span data-stu-id="9cbed-134">Design the report layout.</span></span>

    <span data-ttu-id="9cbed-135">Создайте макет, перетаскивая поля и добавляя визуализации.</span><span class="sxs-lookup"><span data-stu-id="9cbed-135">Create the layout by dragging fields and adding visualizations.</span></span> <span data-ttu-id="9cbed-136">Дополнительные сведения см. в разделе [Работа с представлением отчета в Power BI Desktop](/power-bi/create-reports/desktop-report-view) в документации по Power BI.</span><span class="sxs-lookup"><span data-stu-id="9cbed-136">For more information, see, [Work with Report view in Power BI Desktop](/power-bi/create-reports/desktop-report-view) in the Power BI documentation.</span></span>

5. <span data-ttu-id="9cbed-137">См. следующие разделы об изменении размера отчета и использовании нескольких страниц.</span><span class="sxs-lookup"><span data-stu-id="9cbed-137">See the next sections about sizing the report and using multiple pages.</span></span>

6. <span data-ttu-id="9cbed-138">Сохраните отчет и назовите его.</span><span class="sxs-lookup"><span data-stu-id="9cbed-138">Save and name the report.</span></span>

    <span data-ttu-id="9cbed-139">Важно задать отчету имя, содержащее имя страницы списка, связанной с отчетом.</span><span class="sxs-lookup"><span data-stu-id="9cbed-139">It's important to give the report a name that contains the name of the list page associated with the report.</span></span> <span data-ttu-id="9cbed-140">Например, если отчет предназначен для страницы списка **Товары**, включите слово *товары* где-то в названии.</span><span class="sxs-lookup"><span data-stu-id="9cbed-140">For example, if the report is for the **Items** list page, include the word *items* somewhere in the name.</span></span>  

    <span data-ttu-id="9cbed-141">Это соглашение об именах не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9cbed-141">This naming convention isn't a requirement.</span></span> <span data-ttu-id="9cbed-142">Однако это делает выбор отчетов в [!INCLUDE[prod_short](includes/prod_short.md)] быстрее.</span><span class="sxs-lookup"><span data-stu-id="9cbed-142">However, it makes selecting reports in [!INCLUDE[prod_short](includes/prod_short.md)] quicker.</span></span> <span data-ttu-id="9cbed-143">Когда страница выбора отчета открывается со страницы списка, она автоматически фильтруется на основе имени страницы.</span><span class="sxs-lookup"><span data-stu-id="9cbed-143">When the report selection page opens from a list page, it's automatically filtered based on the page name.</span></span> <span data-ttu-id="9cbed-144">Эта фильтрация выполняется для ограничения отображаемых отчетов.</span><span class="sxs-lookup"><span data-stu-id="9cbed-144">This filtering is done to limit the reports that are displayed.</span></span> <span data-ttu-id="9cbed-145">Пользователи могут удалить фильтр, чтобы получить полный список доступных отчетов в Power BI.</span><span class="sxs-lookup"><span data-stu-id="9cbed-145">Users can clear the filter to get a full list of reports available in Power BI.</span></span>

7. <span data-ttu-id="9cbed-146">Когда вы закончите, опубликуйте отчет как обычно.</span><span class="sxs-lookup"><span data-stu-id="9cbed-146">When you're done, publish the report as usual.</span></span>

    <span data-ttu-id="9cbed-147">Для получения дополнительной информации см. раздел [Публикация отчета](across-how-use-financials-data-source-powerbi.md#publish-reports).</span><span class="sxs-lookup"><span data-stu-id="9cbed-147">For more information, see [Publishing a Report](across-how-use-financials-data-source-powerbi.md#publish-reports).</span></span>

8. <span data-ttu-id="9cbed-148">Протестируйте отчет.</span><span class="sxs-lookup"><span data-stu-id="9cbed-148">Test the report.</span></span>

    <span data-ttu-id="9cbed-149">После того как отчеты были опубликованы в вашей рабочей области, они должны быть доступны из информационной панели Power BI на странице списка в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9cbed-149">Once the reports been published to your workspace, it should be available from the Power BI FactBox on the list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

    <span data-ttu-id="9cbed-150">Чтобы протестировать его, выполните следующие шаги.</span><span class="sxs-lookup"><span data-stu-id="9cbed-150">To test it, do the following steps.</span></span>

    1. <span data-ttu-id="9cbed-151">Откройте [!INCLUDE[prod_short](includes/prod_short.md)] и перейдите на страницу списка.</span><span class="sxs-lookup"><span data-stu-id="9cbed-151">Open [!INCLUDE[prod_short](includes/prod_short.md)] and go to the list page.</span></span>
    2. <span data-ttu-id="9cbed-152">Если вы не видите информационную панель Power BI, перейдите на панель действий, затем выберите **Действия** > **Показать** > **Показать/скрыть отчеты Power BI**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-152">If you don't see the Power BI FactBox, go the action bar, then select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>
    3. <span data-ttu-id="9cbed-153">На информационной панели Power BI выберите **Выбрать отчеты**, выберите поле **Включить** для отчета, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-153">In the Power BI FactBox, select **Select Reports**, select the **Enable** box for the report, then select **OK**.</span></span>

    <span data-ttu-id="9cbed-154">Если отчет разработан правильно, он отображается.</span><span class="sxs-lookup"><span data-stu-id="9cbed-154">If designed correctly, the report displays.</span></span>  

## <a name="set-the-report-size-and-color"></a><span data-ttu-id="9cbed-155">Задание размера и цвета отчета</span><span class="sxs-lookup"><span data-stu-id="9cbed-155">Set the report size and color</span></span>

<span data-ttu-id="9cbed-156">Отчет должен иметь размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="9cbed-156">The size of the report must be set to 325 pixels by 310 pixels.</span></span> <span data-ttu-id="9cbed-157">Этот размер обеспечивает правильное масштабирование отчета в доступном пространстве элемента управления информационной панелью Power BI в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9cbed-157">This size provides the proper scaling of the report in the available space of the Power BI FactBox control in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="9cbed-158">Чтобы определить размер отчета, поместите фокус вне области макета отчета, а затем щелкните значок валика.</span><span class="sxs-lookup"><span data-stu-id="9cbed-158">To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.</span></span>

![Настройка ширины и высоты отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-sizing-v3.png)

<span data-ttu-id="9cbed-160">Можно изменить ширину и высоту отчета, выбрав значение **Пользовательский** в поле **Тип**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-160">You can change the width and height of the report by choosing **Custom** in the **Type** field.</span></span>

<span data-ttu-id="9cbed-161">Если необходимо, чтобы фон отчета смешивался с цветом фона элемента управления информационной панелью Power BI, задайте пользовательский цвет фона отчета как *#FFFFFF* (белый).</span><span class="sxs-lookup"><span data-stu-id="9cbed-161">If you want the background of the report to blend with the background color of the Power BI FactBox control, set report background color to *#FFFFFF* (white).</span></span> 

> [!TIP]
> <span data-ttu-id="9cbed-162">Используйте файл темы [!INCLUDE [prod_short](includes/prod_short.md)] для создания отчетов с тем же цветовым стилем, что и приложения [!INCLUDE [prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9cbed-162">Use the [!INCLUDE [prod_short](includes/prod_short.md)] theme file to build reports with the same color styling as the [!INCLUDE [prod_short](includes/prod_short.md)] apps.</span></span> <span data-ttu-id="9cbed-163">Дополнительные сведения см. в разделе [Использование темы отчета [!INCLUDE [prod_short](includes/prod_short.md)]](across-how-use-financials-data-source-powerbi.md#theme).</span><span class="sxs-lookup"><span data-stu-id="9cbed-163">For more information, see [Using the [!INCLUDE [prod_short](includes/prod_short.md)] report theme](across-how-use-financials-data-source-powerbi.md#theme).</span></span>

## <a name="reports-with-multiple-pages"></a><span data-ttu-id="9cbed-164">Отчеты с несколькими страницами</span><span class="sxs-lookup"><span data-stu-id="9cbed-164">Reports with multiple pages</span></span>

<span data-ttu-id="9cbed-165">В Power BI можно создать один отчет с несколькими страницами.</span><span class="sxs-lookup"><span data-stu-id="9cbed-165">With Power BI, you can create a single report with multiple pages.</span></span> <span data-ttu-id="9cbed-166">Однако для отчетов, которые будут отображаться со страницами списков, мы не рекомендуем иметь более одной страницы.</span><span class="sxs-lookup"><span data-stu-id="9cbed-166">However, for reports that will display with list pages, we don't recommend that they have more than one page.</span></span> <span data-ttu-id="9cbed-167">На информационной панели Power BI отображается только первая страница вашего отчета.</span><span class="sxs-lookup"><span data-stu-id="9cbed-167">The Power BI FactBox will only show the first page of your report.</span></span>

## <a name="fixing-problems"></a><span data-ttu-id="9cbed-168">Устранение проблем</span><span class="sxs-lookup"><span data-stu-id="9cbed-168">Fixing problems</span></span>

<span data-ttu-id="9cbed-169">В этом разделе приведены инструкции по устранению проблем, с которыми вы можете столкнуться при попытке просмотреть отчет Power BI для страницы списка в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9cbed-169">This section provides instructions about how to fix problems that you might run into when trying to view a Power BI report for a list page in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

### <a name="you-cant-see-the-power-bi-factbox-on-a-list-page"></a><span data-ttu-id="9cbed-170">Вы не видите информационную панель Power BI на странице списка</span><span class="sxs-lookup"><span data-stu-id="9cbed-170">You can't see the Power BI FactBox on a list page</span></span>

<span data-ttu-id="9cbed-171">По умолчанию информационная панель Power BI скрыт от просмотра.</span><span class="sxs-lookup"><span data-stu-id="9cbed-171">By default, the Power BI FactBox is hidden from view.</span></span> <span data-ttu-id="9cbed-172">Чтобы показать информационную панель на странице, на панели действий выберите **Действия** > **Показать** > **Показать/скрыть отчеты Power BI**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-172">To show the FactBox on a page, from the action bar, select **Actions** > **Display** > **Show/Hide Power BI Reports**.</span></span>

### <a name="you-cant-see-the-report-in-the-select-report-pane"></a><span data-ttu-id="9cbed-173">Вы не видите отчет на странице выбора отчета</span><span class="sxs-lookup"><span data-stu-id="9cbed-173">You can't see the report in the Select Report pane</span></span>

<span data-ttu-id="9cbed-174">Вероятно, это потому, что в названии отчета нет названия страницы списка, которая отображается.</span><span class="sxs-lookup"><span data-stu-id="9cbed-174">It's probably because the report's name doesn't contain the name of the list page that's being shown.</span></span> <span data-ttu-id="9cbed-175">Очистите фильтр, чтобы получить полный список доступных отчетов Power BI.</span><span class="sxs-lookup"><span data-stu-id="9cbed-175">Clear the filter to get a full list of Power BI reports available.</span></span>  

### <a name="report-is-loaded-but-blank-not-filtered-or-filtered-incorrectly"></a><span data-ttu-id="9cbed-176">Отчет загружен, но пуст, не отфильтрован или неправильно отфильтрован</span><span class="sxs-lookup"><span data-stu-id="9cbed-176">Report is loaded but blank, not filtered, or filtered incorrectly</span></span>

<span data-ttu-id="9cbed-177">Убедитесь, что фильтр отчета содержит правильный первичный ключ.</span><span class="sxs-lookup"><span data-stu-id="9cbed-177">Verify that the report filter contains the right primary key.</span></span> <span data-ttu-id="9cbed-178">В большинстве случаев это поле **Номер**,</span><span class="sxs-lookup"><span data-stu-id="9cbed-178">In most cases, this field is the **No.**</span></span> <span data-ttu-id="9cbed-179">но в таблице **Операция ГК**, например, следует использовать поле **Номер операции**.</span><span class="sxs-lookup"><span data-stu-id="9cbed-179">field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field.</span></span>

### <a name="report-is-loaded-but-it-shows-a-page-you-didnt-expect"></a><span data-ttu-id="9cbed-180">Отчет загружен, но показывает страницу, которую вы не ожидали</span><span class="sxs-lookup"><span data-stu-id="9cbed-180">Report is loaded, but it shows a page you didn't expect</span></span>

<span data-ttu-id="9cbed-181">Убедитесь, что страница, которую вы хотите отобразить, является первой страницей в вашем отчете.</span><span class="sxs-lookup"><span data-stu-id="9cbed-181">Verify that the page you want displayed is the first page in your report.</span></span>  

### <a name="report-appears-with-an-unwanted-gray-boarder-or-its-too-small-or-too-large"></a><span data-ttu-id="9cbed-182">В отчетах отображаются ненужная серая граница, отчет слишком мал или слишком большой</span><span class="sxs-lookup"><span data-stu-id="9cbed-182">Report appears with an unwanted gray boarder, or it's too small or too large</span></span>

<span data-ttu-id="9cbed-183">Проверьте, что отчет имеет размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="9cbed-183">Verify that the report size is set to 325 pixels x 310 pixels.</span></span> <span data-ttu-id="9cbed-184">Сохраните отчет, а затем обновите страницу списка.</span><span class="sxs-lookup"><span data-stu-id="9cbed-184">Save the report, and then refresh the list page.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="9cbed-185">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="9cbed-185">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="9cbed-186">См. также</span><span class="sxs-lookup"><span data-stu-id="9cbed-186">See Also</span></span>

[<span data-ttu-id="9cbed-187">Включение бизнес-данных для Power BI</span><span class="sxs-lookup"><span data-stu-id="9cbed-187">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
<span data-ttu-id="9cbed-188">[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="9cbed-188">[Using [!INCLUDE[prod_short](includes/prod_short.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
[<span data-ttu-id="9cbed-189">Подготовьтесь к ведению бизнеса</span><span class="sxs-lookup"><span data-stu-id="9cbed-189">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="9cbed-190">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="9cbed-190">[Setting Up [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)</span></span>  
[<span data-ttu-id="9cbed-191">Финансы</span><span class="sxs-lookup"><span data-stu-id="9cbed-191">Finance</span></span>](finance.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]