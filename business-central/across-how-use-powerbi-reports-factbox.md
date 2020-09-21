---
title: Отображение пользовательских отчетов Power BI для данных Business Central | Документация Майкрософт
description: Можно использовать отчеты Power BI для сбора дополнительных сведений о данных в списках.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 04/01/2020
ms.author: jswymer
ms.openlocfilehash: 5d3acaf05952a61845eb8bb72b2556f2e54f8208
ms.sourcegitcommit: aeaa0dc64e54432a70c4b0e1faf325cd17d01389
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2020
ms.locfileid: "3697702"
---
# <a name="creating-power-bi-reports-for-displaying-list-data-in-prodshort"></a><span data-ttu-id="f3d2c-103">Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prodshort](includes/prodshort.md)]</span><span class="sxs-lookup"><span data-stu-id="f3d2c-103">Creating Power BI Reports for Displaying List Data in [!INCLUDE[prodshort](includes/prodshort.md)]</span></span>

[!INCLUDE[prodlong](includes/prodlong.md)] <span data-ttu-id="f3d2c-104">включает элемент управления информационной панелью на нескольких ключевых страницах списков, который предоставляет дополнительные сведения о данных в списке.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-104">includes a FactBox control element on a number of key list pages that provide additional insight into the data in the list.</span></span> <span data-ttu-id="f3d2c-105">При перемещении между строками в списке отчет обновляется и фильтруется в соответствии с выбранной операцией.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-105">As you move between rows in the list, the report is updated and filtered for the selected entry.</span></span> <span data-ttu-id="f3d2c-106">Вы можете создавать пользовательские отчеты для отображения в этом элементе управления.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-106">You can create custom reports to display in this control.</span></span> <span data-ttu-id="f3d2c-107">Однако есть несколько правил, которым нужно следовать, чтобы отчеты работали должным образом.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-107">However, there are a few rules to follow to ensure that reports work as expected.</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="f3d2c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f3d2c-108">Prerequisites</span></span>

- <span data-ttu-id="f3d2c-109">Учетная запись Power BI.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-109">A Power BI account.</span></span>
- <span data-ttu-id="f3d2c-110">Power BI Desktop.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-110">Power BI Desktop.</span></span>

<span data-ttu-id="f3d2c-111">Дополнительные сведения о начале работы см. в разделе [Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источник данных Power BI](across-how-use-financials-data-source-powerbi.md).</span><span class="sxs-lookup"><span data-stu-id="f3d2c-111">For more information about getting started, see [Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md).</span></span>

## <a name="defining-the-report-data-set"></a><span data-ttu-id="f3d2c-112">Определение набора данных отчета</span><span class="sxs-lookup"><span data-stu-id="f3d2c-112">Defining the report data set</span></span>

<span data-ttu-id="f3d2c-113">Укажите источник данных, содержащий данные, относящиеся к списку.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-113">Specify the data source that contains the data related to the list.</span></span> <span data-ttu-id="f3d2c-114">Например, чтобы создать отчет для списка продаж, убедитесь, что набор данных содержит информацию, связанную с продажами.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-114">For example, to create a report for the Sales List, ensure the data set contains information related to sales.</span></span>  

## <a name="defining-the-report-filter"></a><span data-ttu-id="f3d2c-115">Определение фильтра отчета</span><span class="sxs-lookup"><span data-stu-id="f3d2c-115">Defining the report filter</span></span>

<span data-ttu-id="f3d2c-116">Чтобы обновить данные для выбранной записи в списке, вы добавляете фильтр в отчет.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-116">To make the data update to the selected record in the list, you add a filter to the report.</span></span> <span data-ttu-id="f3d2c-117">Фильтр должен включать поле источника данных, которое используется в качестве *первичного ключа*.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-117">The filter must include a field of the data source that's used as the *primary key*.</span></span> <span data-ttu-id="f3d2c-118">В большинстве случаев первичным ключом для списка является **Номер**.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-118">In most cases, the primary key for a list is the **No.**</span></span> <span data-ttu-id="f3d2c-119">.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-119">field.</span></span>

<span data-ttu-id="f3d2c-120">Для определения фильтра для отчета выберите первичный ключ из списка доступных полей, а затем перетащите это поле в раздел **Фильтр отчета**.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-120">To define a filter for the report, select the primary key from the list of available fields, and then drag and drop that field into the **Report Filter** section.</span></span> <span data-ttu-id="f3d2c-121">Фильтр должен быть основным фильтром отчета.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-121">The filter must be basic report filter.</span></span> <span data-ttu-id="f3d2c-122">Это не может быть страничный, визуальный или расширенный фильтр.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-122">It can't be page, visual, or advanced filter.</span></span> 

![Настройка фильтра отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-filter.png)

## <a name="setting-the-report-size-and-color"></a><span data-ttu-id="f3d2c-124">Настройка размера и цвета отчета</span><span class="sxs-lookup"><span data-stu-id="f3d2c-124">Setting the report size and color</span></span>

<span data-ttu-id="f3d2c-125">Отчет должен иметь размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-125">The size of the report must be set to 325 pixels by 310 pixels.</span></span> <span data-ttu-id="f3d2c-126">Этот размер обеспечивает правильное масштабирование отчета в доступном пространстве элемента управления информационной панелью Power BI в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f3d2c-126">This size provides the proper scaling of the report in the available space of the Power BI FactBox control in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f3d2c-127">Чтобы определить размер отчета, поместите фокус вне области макета отчета, а затем щелкните значок валика.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-127">To define the size of the report, place focus outside of the report layout area, and then choose the paint roller icon.</span></span>

![Настройка ширины и высоты отчета для отчета "Активность счетов продаж"](./media/across-how-use-powerbi-reports-factbox/financials-powerbi-report-sizing.png)

<span data-ttu-id="f3d2c-129">Можно изменить ширину и высоту отчета, выбрав значение **Пользовательский** в поле **Тип**.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-129">You can change the width and height of the report by choosing **Custom** in the **Type** field.</span></span>

<span data-ttu-id="f3d2c-130">Если необходимо, чтобы фон отчета смешивался с цветом фона элемента управления информационной панелью Power BI, задайте пользовательский цвет фона отчета как *#FFFFFF*.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-130">If you want the background of the report to blend with the background color of the Power BI FactBox control, set report background color to *#FFFFFF*.</span></span> 

## <a name="using-reports-with-multiple-pages"></a><span data-ttu-id="f3d2c-131">Использование отчета с несколькими страницами</span><span class="sxs-lookup"><span data-stu-id="f3d2c-131">Using reports with multiple pages</span></span>

<span data-ttu-id="f3d2c-132">В Power BI можно создать один отчет с несколькими страницами.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-132">With Power BI, you can create a single report with multiple pages.</span></span> <span data-ttu-id="f3d2c-133">Однако для отчетов, которые будут отображаться со страницами списков, мы не рекомендуем иметь более одной страницы.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-133">However, for reports that will display with list pages, we don't recommend that they have more than one page.</span></span> <span data-ttu-id="f3d2c-134">На информационной панели Power BI отображается только первая страница вашего отчета.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-134">The Power BI FactBox will only show the first page of your report.</span></span>

## <a name="naming-the-report"></a><span data-ttu-id="f3d2c-135">Задание имени отчета</span><span class="sxs-lookup"><span data-stu-id="f3d2c-135">Naming the report</span></span>

<span data-ttu-id="f3d2c-136">Задайте отчету имя, содержащее имя страницы списка, связанной с отчетом.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-136">Give the report a name that contains the name of the list page associated with the report.</span></span> <span data-ttu-id="f3d2c-137">Например, если отчет предназначен для страницы списка **Поставщик**, включите слово *поставщик* где-то в названии.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-137">For example, if the report is for the **Vendor** list page, include the word *vendor* somewhere in the name.</span></span>  

<span data-ttu-id="f3d2c-138">Это соглашение об именах не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-138">This naming convention isn't a requirement.</span></span> <span data-ttu-id="f3d2c-139">Однако это делает выбор отчетов в [!INCLUDE[d365fin](includes/d365fin_md.md)] быстрее.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-139">However, it makes selecting reports in [!INCLUDE[d365fin](includes/d365fin_md.md)] quicker.</span></span> <span data-ttu-id="f3d2c-140">Когда страница выбора отчета открывается со страницы списка, она автоматически фильтруется на основе имени страницы.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-140">When the report selection page opens from a list page, it's automatically filtered based on the page name.</span></span> <span data-ttu-id="f3d2c-141">Эта фильтрация выполняется для ограничения отображаемых отчетов.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-141">This filtering is done to limit the reports that are displayed.</span></span> <span data-ttu-id="f3d2c-142">Пользователи могут удалить фильтр, чтобы получить полный список доступных отчетов в Power BI.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-142">Users can clear the filter to get a full list of reports available in Power BI.</span></span>  

## <a name="fixing-problems"></a><span data-ttu-id="f3d2c-143">Устранение проблем</span><span class="sxs-lookup"><span data-stu-id="f3d2c-143">Fixing problems</span></span>

<span data-ttu-id="f3d2c-144">В этом разделе приводится обходное решение для большинства типичных проблем, которые могут возникнуть при создании отчета Power BI.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-144">This section provides a workaround for the most typical problems that can occur when you create the Power BI report.</span></span>  

#### <a name="you-cant-see-a-report-on-the-select-report-page"></a><span data-ttu-id="f3d2c-145">Вы не можете увидеть отчет на странице выбора отчета</span><span class="sxs-lookup"><span data-stu-id="f3d2c-145">You can't see a report on the Select Report page</span></span>

<span data-ttu-id="f3d2c-146">Вероятно, это потому, что в названии отчета нет названия страницы списка.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-146">It's probably because the report's name doesn't contain the name of the list page.</span></span> <span data-ttu-id="f3d2c-147">Очистите фильтр, чтобы получить полный список доступных отчетов Power BI.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-147">Clear the filter to get a full list of Power BI reports available.</span></span>  

#### <a name="report-is-loaded-but-blank-not-filtered-or-filtered-incorrectly"></a><span data-ttu-id="f3d2c-148">Отчет загружен, но пуст, не отфильтрован или неправильно отфильтрован</span><span class="sxs-lookup"><span data-stu-id="f3d2c-148">Report is loaded but blank, not filtered or filtered incorrectly</span></span>

<span data-ttu-id="f3d2c-149">Убедитесь, что фильтр отчета содержит правильный первичный ключ.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-149">Verify that the report filter contains the right primary key.</span></span> <span data-ttu-id="f3d2c-150">В большинстве случаев это поле **Номер**,</span><span class="sxs-lookup"><span data-stu-id="f3d2c-150">In most cases, this field is the **No.**</span></span> <span data-ttu-id="f3d2c-151">но в таблице **Операция ГК**, например, следует использовать поле **Номер операции**.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-151">field, but in the **G/L Entry** table, for example, you must use the **Entry No.** field.</span></span>

#### <a name="report-is-loaded-but-it-shows-a-page-you-didnt-expect"></a><span data-ttu-id="f3d2c-152">Отчет загружен, но показывает страницу, которую вы не ожидали</span><span class="sxs-lookup"><span data-stu-id="f3d2c-152">Report is loaded, but it shows a page you didn't expect</span></span>

<span data-ttu-id="f3d2c-153">Убедитесь, что страница, которую вы хотите отобразить, является первой страницей в вашем отчете.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-153">Verify that the page you want displayed is the first page in your report.</span></span>  

#### <a name="report-appears-with-an-unwanted-gray-boarder-or-its-too-small-or-too-large"></a><span data-ttu-id="f3d2c-154">В отчетах отображаются ненужная серая граница, отчет слишком мал или слишком большой</span><span class="sxs-lookup"><span data-stu-id="f3d2c-154">Report appears with an unwanted gray boarder, or it's too small or too large</span></span>

<span data-ttu-id="f3d2c-155">Проверьте, что отчет имеет размер 325 х 310 пикселей.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-155">Verify that the report size is set to 325 pixels x 310 pixels.</span></span> <span data-ttu-id="f3d2c-156">Сохраните отчет, а затем обновите страницу списка.</span><span class="sxs-lookup"><span data-stu-id="f3d2c-156">Save the report, and then refresh the list page.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="f3d2c-157">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="f3d2c-157">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="f3d2c-158">См. также</span><span class="sxs-lookup"><span data-stu-id="f3d2c-158">See Also</span></span>

[<span data-ttu-id="f3d2c-159">Включение бизнес-данных для Power BI</span><span class="sxs-lookup"><span data-stu-id="f3d2c-159">Enabling Your Business Data for Power BI</span></span>](admin-powerbi.md)  
<span data-ttu-id="f3d2c-160">[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="f3d2c-160">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as a Power BI Data Source](across-how-use-financials-data-source-powerbi.md)</span></span>  
[<span data-ttu-id="f3d2c-161">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="f3d2c-161">Getting Started</span></span>](product-get-started.md)  
<span data-ttu-id="f3d2c-162">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="f3d2c-162">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="f3d2c-163">Финансы</span><span class="sxs-lookup"><span data-stu-id="f3d2c-163">Finance</span></span>](finance.md)  
