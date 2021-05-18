---
title: Сортировка, поиск и фильтрация списков | Документация Майкрософт
description: Работайте в списках эффективно, выполняя поиск в своих данных, сортируя столбцы и уточняя результаты с помощью символов фильтров и сочетаний клавиш.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: a27556350851de61bd31504d0c29ef60df6d890a
ms.sourcegitcommit: 921f0c4043dcda2fb8fc35df1b64310bf32270d7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2021
ms.locfileid: "6017178"
---
# <a name="sorting-searching-and-filtering"></a><span data-ttu-id="d078f-103">Сортировка, поиск и фильтрация</span><span class="sxs-lookup"><span data-stu-id="d078f-103">Sorting, Searching, and Filtering</span></span>

<span data-ttu-id="d078f-104">Существует несколько приемов, которые помогают просматривать, искать и ограничивать записи в списке, отчете или XMLport.</span><span class="sxs-lookup"><span data-stu-id="d078f-104">There are a few things that you can do that will help you scan, find, and limit records on a list or in a report or XMLport.</span></span> <span data-ttu-id="d078f-105">К ним относятся сортировка, поиск и фильтрация.</span><span class="sxs-lookup"><span data-stu-id="d078f-105">These include sorting, searching, and filtering.</span></span> <span data-ttu-id="d078f-106">Некоторые или все из них можно применить одновременно для быстрого поиска или анализа данных.</span><span class="sxs-lookup"><span data-stu-id="d078f-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

<span data-ttu-id="d078f-107">В отчетах и XMLport, как в списках, можно устанавливать фильтры, чтобы определить, какие данные включить в отчет или XMLport, однако выполнять сортировку и поиск в них нельзя.</span><span class="sxs-lookup"><span data-stu-id="d078f-107">For reports and XMLports, as on lists, you can set filters to delimit which data to include in the report or XMLport, but you can't sort and search.</span></span>

> [!TIP]
> <span data-ttu-id="d078f-108">При просмотре ваших данных в виде плиток можно осуществлять поиск и использовать фильтрацию.</span><span class="sxs-lookup"><span data-stu-id="d078f-108">When viewing your data as tiles, you can search and use filtering.</span></span> <span data-ttu-id="d078f-109">Чтобы использовать полный набор мощных функций для сортировки, поиска и фильтрации, выберите значок ![Показать как список](media/ui_show_as_list_icon.png "Показать как список стрелка влево") для отображения записей в виде списка.</span><span class="sxs-lookup"><span data-stu-id="d078f-109">To use the full set of powerful features for sorting, searching, and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to view the records as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria, you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="d078f-110">Сортировка</span><span class="sxs-lookup"><span data-stu-id="d078f-110">Sorting</span></span>

<span data-ttu-id="d078f-111">Сортировка позволяет быстро и легко получить общее представление о данных.</span><span class="sxs-lookup"><span data-stu-id="d078f-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="d078f-112">Например, при наличии большого числа клиентов, можно сортировать их по полю **Номер клиента**, **Код валюты** или **Код страны/региона**, чтобы получить нужный обзор.</span><span class="sxs-lookup"><span data-stu-id="d078f-112">For example, if you have many customers,  you could sort them by **Customer No.**, **Currency Code**, or **Country Region Code** to get the overview you need.</span></span>

<span data-ttu-id="d078f-113">Чтобы отсортировать список, вы можете:</span><span class="sxs-lookup"><span data-stu-id="d078f-113">To sort a list, you can either:</span></span>

- <span data-ttu-id="d078f-114">Выбрать текст заголовка столбца для переключения между возрастающим и убывающим порядком, или</span><span class="sxs-lookup"><span data-stu-id="d078f-114">Choose a column heading text to toggle between ascending and descending order, or</span></span>
- <span data-ttu-id="d078f-115">Выбрать стрелку раскрывающегося списка в заголовке столбца, затем выбрать действие **По возрастанию** или **По убыванию**.</span><span class="sxs-lookup"><span data-stu-id="d078f-115">Choose the drop-down arrow in the column heading, then choose the **Ascending** or **Descending** action.</span></span>  

> [!NOTE]  
> <span data-ttu-id="d078f-116">Не поддерживается сортировка изображений, полей BLOB, полей FlowFilter и полей, которые не принадлежат таблице.</span><span class="sxs-lookup"><span data-stu-id="d078f-116">Sorting isn't supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="d078f-117">Поиск</span><span class="sxs-lookup"><span data-stu-id="d078f-117">Searching</span></span>

<!--## Searching by using the Quick Filter -->
<span data-ttu-id="d078f-118">Вверху каждой страницы списке имеется действие ![Поиск в списке](media/ui-search/search-list.png "Значок поиска в списке") **Поиск**, которое представляет собой быстрый и простой способ уменьшить количество записей в списке и отобразить только те записи, которые содержат интересующие вас данные.</span><span class="sxs-lookup"><span data-stu-id="d078f-118">At the top of each list page, there's a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** action that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you're interested in seeing.</span></span>

<span data-ttu-id="d078f-119">Для поиска просто выберите действие **Поиск**, а затем в поле введите текст, который требуется найти.</span><span class="sxs-lookup"><span data-stu-id="d078f-119">To search, just choose the **Search** action, and then in the box, type the text that you're looking for.</span></span> <span data-ttu-id="d078f-120">Можно ввести буквы, цифры и другие символы.</span><span class="sxs-lookup"><span data-stu-id="d078f-120">You can enter letters, numbers, and other symbols.</span></span>

<span data-ttu-id="d078f-121">Как правило, поиск пытается найти искомый текст во всех полях.</span><span class="sxs-lookup"><span data-stu-id="d078f-121">In general, search will attempt to match text across all fields.</span></span> <span data-ttu-id="d078f-122">Поиск не различает символы верхнего и нижнего регистров (не чувствителен к регистру) и находит текст в любом месте поля (в начале, в конце либо в середине).</span><span class="sxs-lookup"><span data-stu-id="d078f-122">It doesn't distinguish between uppercase and lowercase characters (case insensitive) and will match text placed anywhere in the field, at the beginning, end, or in the middle.</span></span>

> [!TIP]
> <span data-ttu-id="d078f-123">Можно нажать клавишу **F3** для активации и деактивации поля поиска.</span><span class="sxs-lookup"><span data-stu-id="d078f-123">You can press **F3** to activate and deactivate the search box.</span></span> <span data-ttu-id="d078f-124">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="d078f-124">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

> [!NOTE]  
> <span data-ttu-id="d078f-125">Поиск не будет сопоставлять значения в изображениях, полях BLOB, FlowFilters, FlowFields и других полях, которые не являются частью таблицы.</span><span class="sxs-lookup"><span data-stu-id="d078f-125">Search won't match values in images, BLOB fields, FlowFilters, FlowFields, and other fields that aren't part of a table.</span></span>


### <a name="fine-tuning-the-search-with-filter-criteria"></a><span data-ttu-id="d078f-126">Точная настройка поиска с помощью критериев фильтра</span><span class="sxs-lookup"><span data-stu-id="d078f-126">Fine-tuning the Search with Filter criteria</span></span>

<span data-ttu-id="d078f-127">Вы можете выполнить более точный поиск, используя операторы фильтра, выражения и токены фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-127">You can make a more exact search by using filter operators, expressions, and filter tokens.</span></span> <span data-ttu-id="d078f-128">В отличие от фильтрации, они применяются ко всем полям при использовании в поле поиска, что делает их менее эффективными, чем фильтрация.</span><span class="sxs-lookup"><span data-stu-id="d078f-128">Unlike filtering, these are applied across all fields when used in the search box, making them less efficient than filtering.</span></span>

- <span data-ttu-id="d078f-129">Чтобы найти только значения полей, которые точно совпадают со всем текстом и регистром, заключите искомый текст в одинарные кавычки `''` (например, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="d078f-129">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="d078f-130">Чтобы найти только значения полей, которые начинаются с определенного текста с совпадающим регистром, поместите `*` после искомого текста (например, `man*`).</span><span class="sxs-lookup"><span data-stu-id="d078f-130">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="d078f-131">Чтобы найти только значения полей, которые заканчиваются определенным текстом с учетом регистра, поместите `*` перед искомым текстом (например, `*man`).</span><span class="sxs-lookup"><span data-stu-id="d078f-131">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="d078f-132">При использовании `''` или `*` поиск учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="d078f-132">When using  `''` or `*`, the search is case-sensitive.</span></span> <span data-ttu-id="d078f-133">Если требуется делать поиск нечувствительным к регистру, установите `@` перед искомым текстом (например, `@man*`).</span><span class="sxs-lookup"><span data-stu-id="d078f-133">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="d078f-134">В следующей таблице приведены некоторые примеры для объяснения как можно использовать поиск.</span><span class="sxs-lookup"><span data-stu-id="d078f-134">The following table provides some examples to explain how you can use the search.</span></span>

|<span data-ttu-id="d078f-135">Критерии поиска</span><span class="sxs-lookup"><span data-stu-id="d078f-135">Search Criteria</span></span>|<span data-ttu-id="d078f-136">Находит...</span><span class="sxs-lookup"><span data-stu-id="d078f-136">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="d078f-137">или</span><span class="sxs-lookup"><span data-stu-id="d078f-137">or</span></span> <br />`Man`|<span data-ttu-id="d078f-138">Все записи с полями, которые содержат текст **man** независимо от регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-138">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="d078f-139">Например, **Manchester**, **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="d078f-139">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="d078f-140">Все записи с полями, которые содержат только **Man** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-140">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="d078f-141">Все записи с полями, которые начинаются с текста <b>Man</b> с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-141">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="d078f-142">Например, **Manchester**, но не **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="d078f-142">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="d078f-143">Все записи с полями, которые начинаются с текста **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-143">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="d078f-144">Например, **Manchester** и **manual**, но не **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="d078f-144">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="d078f-145">Все записи с полями, которые заканчиваются на **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-145">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="d078f-146">Например, **Sportsman**, но не **Manchester** или **manual**.</span><span class="sxs-lookup"><span data-stu-id="d078f-146">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|


## <a name="filtering"></a><a name="filtering"></a><span data-ttu-id="d078f-147">Фильтрация</span><span class="sxs-lookup"><span data-stu-id="d078f-147">Filtering</span></span>

<span data-ttu-id="d078f-148">Фильтрация обеспечивает более широкие и разнообразные способы контроля того, какие записи включаются в список, отчет или XMLport.</span><span class="sxs-lookup"><span data-stu-id="d078f-148">Filtering provides a more advanced and versatile way to control which records are included in a list, report, or XMLport.</span></span> <span data-ttu-id="d078f-149">Имеется два основных отличия между поиском и фильтрацией, как описано в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="d078f-149">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="d078f-150">**Поиск**</span><span class="sxs-lookup"><span data-stu-id="d078f-150">**Searching**</span></span> | <span data-ttu-id="d078f-151">**Фильтрация**</span><span class="sxs-lookup"><span data-stu-id="d078f-151">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="d078f-152">**Применимые поля**</span><span class="sxs-lookup"><span data-stu-id="d078f-152">**Applicable Fields**</span></span> | <span data-ttu-id="d078f-153">Производится поиск по всем полям, видимым на странице.</span><span class="sxs-lookup"><span data-stu-id="d078f-153">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="d078f-154">Фильтрует одно или несколько полей по отдельности, выбирая из любого поля в таблице, включая поля, которые не отображаются на странице.</span><span class="sxs-lookup"><span data-stu-id="d078f-154">Filters one or more fields individually, selecting from any field on the table, including fields that aren't visible on the page.</span></span> |
| <span data-ttu-id="d078f-155">**Соответствие**</span><span class="sxs-lookup"><span data-stu-id="d078f-155">**Matching**</span></span> | <span data-ttu-id="d078f-156">Отображаются записи с полями, которые соответствуют тексту поиска, независимо от регистра текста или его местоположения в поле.</span><span class="sxs-lookup"><span data-stu-id="d078f-156">Displays records with fields that match the search text, no matter the text's case or placement in the field.</span></span> | <span data-ttu-id="d078f-157">Отображаются записи, в которых поле точно соответствует фильтру, включая регистр текста, если не введены специальные символы фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-157">Displays records where the field exactly matches the filter, including the text's case, unless special filter symbols are entered.</span></span>

<span data-ttu-id="d078f-158">Фильтрация позволяет отобразить записи для определенных организаций или клиентов, дат, сумм и иной информации путем определения критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-158">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="d078f-159">Только записи, которые соответствуют критериям, отображаются в списке или включаются в отчет, пакетное задание или XMLport.</span><span class="sxs-lookup"><span data-stu-id="d078f-159">Only records that match the criteria are displayed on the list or included in the report, batch job, or XMLport.</span></span> <span data-ttu-id="d078f-160">Если критерии заданы для нескольких полей, отображаются только записи, которые соответствуют этим критериям.</span><span class="sxs-lookup"><span data-stu-id="d078f-160">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

<span data-ttu-id="d078f-161">В случае списков фильтры отображаются в области фильтров, которая появляется слева от списка, когда вы активируете его.</span><span class="sxs-lookup"><span data-stu-id="d078f-161">For lists, the filters are displayed on a filter pane that appears to the left of the list when you activate it.</span></span> <span data-ttu-id="d078f-162">В случае отчетов, пакетных заданий и XMLport фильтры отображаются непосредственно на странице запроса.</span><span class="sxs-lookup"><span data-stu-id="d078f-162">For reports, batch jobs, and XMLports, the filters are visible directly on the request page.</span></span>

### <a name="filtering-with-option-fields"></a><span data-ttu-id="d078f-163">Фильтрация с помощью полей параметров</span><span class="sxs-lookup"><span data-stu-id="d078f-163">Filtering with Option Fields</span></span>

<span data-ttu-id="d078f-164">Для "обычных" полей, которые содержат данные, установленную дату или бизнес-данные, вы можете установить фильтры как путем выбора данных, так и путем ввода значений фильтров, а также использовать символы для определения расширенных критериев фильтрации.</span><span class="sxs-lookup"><span data-stu-id="d078f-164">For "ordinary" fields that hold data, setup date, or business data, you can set filters both by selecting data and by typing filter values, and you can use symbols to define advanced filter criteria.</span></span> <span data-ttu-id="d078f-165">Дополнительные сведения см. в разделе [Ввод критериев в фильтрах](ui-enter-criteria-filters.md#entering-filter-criteria).</span><span class="sxs-lookup"><span data-stu-id="d078f-165">For more information, see [Entering Filter Criteria](ui-enter-criteria-filters.md#entering-filter-criteria).</span></span>

<span data-ttu-id="d078f-166">В случае полей типа **Параметр**, однако, установить фильтр можно только путем выбора одного из нескольких параметров из раскрывающегося списка возможных параметров.</span><span class="sxs-lookup"><span data-stu-id="d078f-166">For fields of type **Option**, however, you can only set a filter by selecting one or more options from a drop-down list of the available options.</span></span> <span data-ttu-id="d078f-167">Пример поля параметров — поле **Состояние** на странице **Заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="d078f-167">An example of an option field is the **Status** field on the **Sales Orders** page.</span></span>

> [!NOTE]
> <span data-ttu-id="d078f-168">Когда вы выбираете несколько параметров в качестве значения фильтра, связь между параметрами определяется как *ИЛИ*.</span><span class="sxs-lookup"><span data-stu-id="d078f-168">When you select multiple options as a filter value, the relationship between the options is defined as *OR*.</span></span> <span data-ttu-id="d078f-169">Например, если установить и флажок **Открыто**, и флажок **Выпущено** в поле фильтра **Состояние** на странице **Заказы на продажу**, будут отображены заказы на продажу, которые открыты или выпущены.</span><span class="sxs-lookup"><span data-stu-id="d078f-169">For example, if you select both the **Open** and the **Released** check box in the **Status** filter field on the **Sales Orders** page, it means that sales orders that are either open or released are displayed.</span></span>

### <a name="setting-filters-on-lists"></a><span data-ttu-id="d078f-170">Установка фильтров в списках</span><span class="sxs-lookup"><span data-stu-id="d078f-170">Setting Filters on Lists</span></span>

<span data-ttu-id="d078f-171">В списках фильтры устанавливаются с помощью области фильтров.</span><span class="sxs-lookup"><span data-stu-id="d078f-171">On lists, you set filters by using the filter pane.</span></span> <span data-ttu-id="d078f-172">Чтобы отобразить панель фильтров для списка, выберите стрелку раскрывающегося списка рядом с именем страницы, а затем выберите действие **Показать область фильтров**.</span><span class="sxs-lookup"><span data-stu-id="d078f-172">To display the filter pane for a list, choose the drop-down arrow next to the name of the page, and then choose the **Show filter pane** action.</span></span> <span data-ttu-id="d078f-173">Также можно нажать **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="d078f-173">Alternatively, press **Shift+F3**.</span></span>

<span data-ttu-id="d078f-174">Чтобы отобразить область фильтров для столбца в списке, выберите стрелку раскрывающегося списка, а затем выберите действие **Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-174">To display the filter pane for a column on a list, choose the drop-down arrow, and then choose the **Filter** action.</span></span> <span data-ttu-id="d078f-175">Также можно нажать **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="d078f-175">Alternatively, press **Shift+F3**.</span></span> <span data-ttu-id="d078f-176">Откроется область фильтров с выбранным столбцом, отображаемым в качестве поля фильтра в разделе **Фильтровать список по**.</span><span class="sxs-lookup"><span data-stu-id="d078f-176">The filter pane opens with the selected column shown as a filter field in the **Filter list by** section.</span></span>

<span data-ttu-id="d078f-177">В области фильтров отображаются текущие фильтры для списка, и в ней вы можете установить собственные настраиваемые фильтры для одного или нескольких полей, выбрав действие **+ Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-177">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields by choosing the **+ Filter** action.</span></span>

 <span data-ttu-id="d078f-178">Область фильтров разделена на три раздела: **Представления**, **Фильтровать список по** и **Фильтровать итоги по**:</span><span class="sxs-lookup"><span data-stu-id="d078f-178">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="d078f-179">**Представления**</span><span class="sxs-lookup"><span data-stu-id="d078f-179">**Views**</span></span>

  <span data-ttu-id="d078f-180">Некоторые списки включают раздел **Представления**.</span><span class="sxs-lookup"><span data-stu-id="d078f-180">Some lists include the **Views** section.</span></span> <span data-ttu-id="d078f-181">Представления — это вариации списка, которые были ранее настроены с помощью фильтров.</span><span class="sxs-lookup"><span data-stu-id="d078f-181">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="d078f-182">Вы можете определить и сохранить столько представлений, сколько хотите, для каждого списка.</span><span class="sxs-lookup"><span data-stu-id="d078f-182">You can define and save as many views as you want per list.</span></span> <span data-ttu-id="d078f-183">Представления будут доступны вам на любом устройстве, в которое вы войдете.</span><span class="sxs-lookup"><span data-stu-id="d078f-183">The views will be available to you on any device you sign into.</span></span> <span data-ttu-id="d078f-184">Дополнительные сведения см. в разделе [Сохранение и персонализация представлений списков](ui-views.md).</span><span class="sxs-lookup"><span data-stu-id="d078f-184">For more information, see [Save and Personalize List Views](ui-views.md).</span></span>

- <span data-ttu-id="d078f-185">**Фильтровать список по**</span><span class="sxs-lookup"><span data-stu-id="d078f-185">**Filter list by**</span></span>

  <span data-ttu-id="d078f-186">В этом разделе можно добавлять фильтры по конкретным полям для сокращения числа отображаемых записей.</span><span class="sxs-lookup"><span data-stu-id="d078f-186">This section is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="d078f-187">Чтобы добавить фильтр, выберите действие **+ Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-187">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="d078f-188">Затем введите имя поля, по которому вы хотите отфильтровать список, или выберите поле в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="d078f-188">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span></span>

- <span data-ttu-id="d078f-189">**Фильтровать итоги по**</span><span class="sxs-lookup"><span data-stu-id="d078f-189">**Filter totals by**</span></span>

  <span data-ttu-id="d078f-190">Некоторые списки, в которых отображаются вычисляемые поля, такие как суммы и количества, будут содержать раздел **Фильтровать итоги по** для изменения различных измерений, воздействующих на расчеты.</span><span class="sxs-lookup"><span data-stu-id="d078f-190">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="d078f-191">Чтобы добавить фильтр, выберите действие **+ Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-191">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="d078f-192">Затем введите имя поля, по которому вы хотите отфильтровать список, или выберите поле в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="d078f-192">Then, type the name of the field that you want to filter the list by or pick a field from the drop-down list.</span></span>

  > [!NOTE]
  > <span data-ttu-id="d078f-193">Фильтры в разделе **Фильтровать итоги по** управляются элементами FlowFilter в дизайне страницы.</span><span class="sxs-lookup"><span data-stu-id="d078f-193">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="d078f-194">Технические сведения см. в разделе [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="d078f-194">For technical information, see [FlowFilters](/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>

<span data-ttu-id="d078f-195">Вы можете установить простой фильтр непосредственно в списке, не используя область фильтров, а именно фильтр, который отображает только записи с тем же значением, что и в выбранной ячейке.</span><span class="sxs-lookup"><span data-stu-id="d078f-195">You can set a simple filter directly on a list within using the filter pane, namely a filter that displays only records with the same value as in the selected cell.</span></span> <span data-ttu-id="d078f-196">Выберите ячейку в списке, выберите стрелку раскрывающегося списка, а затем выберите действие **Фильтровать до этого значения**.</span><span class="sxs-lookup"><span data-stu-id="d078f-196">Select a cell on the list, choose the drop-down arrow, and then choose the **Filter to This Value** action.</span></span> <span data-ttu-id="d078f-197">Также можно нажать **Alt+F3**.</span><span class="sxs-lookup"><span data-stu-id="d078f-197">Alternatively, press **Alt+F3**.</span></span>

### <a name="setting-filters-in-reports-batch-jobs-and-xmlports"></a><span data-ttu-id="d078f-198">Установка фильтров в отчетах, пакетных заданиях и XMLport</span><span class="sxs-lookup"><span data-stu-id="d078f-198">Setting Filters in Reports, Batch Jobs, and XMLports</span></span>

<span data-ttu-id="d078f-199">В случае отчетов и XMLport фильтры отображаются непосредственно на странице запроса.</span><span class="sxs-lookup"><span data-stu-id="d078f-199">For reports and XMLports, the filters are visible directly on the request page.</span></span> <span data-ttu-id="d078f-200">На странице запроса отображаются последние использованные фильтры в соответствии с тем, что выбрано в поле **Использовать значения по умолчанию из**.</span><span class="sxs-lookup"><span data-stu-id="d078f-200">The request page displays the last used filters according to your selection in the **Use default values from** field.</span></span> <span data-ttu-id="d078f-201">Дополнительные сведения см. в разделе [Использование сохраненных параметров](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="d078f-201">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

<span data-ttu-id="d078f-202">В главном разделе **Фильтр** отображаются поля фильтра по умолчанию, используемые для определения того, какие записи включаются в отчет или XMLport.</span><span class="sxs-lookup"><span data-stu-id="d078f-202">The main **Filter** section shows the default filter fields that you use to delimit which records to include in the report or XMLport.</span></span> <span data-ttu-id="d078f-203">Чтобы добавить фильтр, выберите действие **+ Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-203">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="d078f-204">Затем введите имя поля, по которому вы хотите фильтровать, или выберите поле в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="d078f-204">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

<span data-ttu-id="d078f-205">В разделе **Фильтровать итоги по** можно откорректировать различные измерения, которые влияют на расчеты в отчете или XMLport.</span><span class="sxs-lookup"><span data-stu-id="d078f-205">In the **Filter totals by** section, you can adjust various dimensions that influence calculations in the report or XMLport.</span></span> <span data-ttu-id="d078f-206">Чтобы добавить фильтр, выберите действие **+ Фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-206">To add a filter, choose the **+ Filter** action.</span></span> <span data-ttu-id="d078f-207">Затем введите имя поля, по которому вы хотите фильтровать, или выберите поле в раскрывающемся списке.</span><span class="sxs-lookup"><span data-stu-id="d078f-207">Then, type the name of the field that you want to filter by, or pick a field from the drop-down list.</span></span>

## <a name="entering-filter-criteria"></a><span data-ttu-id="d078f-208">Ввод критериев фильтрации</span><span class="sxs-lookup"><span data-stu-id="d078f-208">Entering Filter Criteria</span></span>

<span data-ttu-id="d078f-209">И в области фильтров, и на странице запроса критерии фильтрации вводятся в поле под полем фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-209">Both in the filter pane and on a request page, you enter your filter criteria in the box under the filter field.</span></span>

<span data-ttu-id="d078f-210">Тип поля фильтра определяет, какие критерии можно ввести.</span><span class="sxs-lookup"><span data-stu-id="d078f-210">The type of the filter field determines which criteria you can enter.</span></span> <span data-ttu-id="d078f-211">Например, при фильтрации поля, которое имеет фиксированные значения, можно выбирать только из этих значений.</span><span class="sxs-lookup"><span data-stu-id="d078f-211">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="d078f-212">Дополнительные сведения об особенных знаках фильтров см. в разделах [Критерии фильтра](#FilterCriteria) и [Токены фильтра](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="d078f-212">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="d078f-213">Столбцы, которые уже содержат фильтры, обозначаются значком ![Значок фильтра](media/ui-search/filter-icon.png "Значок фильтра") в заголовке столбца.</span><span class="sxs-lookup"><span data-stu-id="d078f-213">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") icon in the column heading.</span></span> <span data-ttu-id="d078f-214">Чтобы удалить фильтр, щелкните стрелку раскрывающегося списка, а затем выберите **Очистить фильтр**.</span><span class="sxs-lookup"><span data-stu-id="d078f-214">To remove a filter, choose the drop-down arrow, and then choose the **Clear Filter** action.</span></span>

> [!TIP]
> <span data-ttu-id="d078f-215">Ускорьте поиск и анализ данных с помощью сочетаний клавиш.</span><span class="sxs-lookup"><span data-stu-id="d078f-215">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="d078f-216">Например, выберите поле, используйте **Shift+Alt+F3** для добавления этого поля к области фильтров, введите критерии фильтра, используйте **Ctrl+Enter** для возврата в строки, выберите другое поле, используйте **Alt+F3** для фильтрации по этому значению.</span><span class="sxs-lookup"><span data-stu-id="d078f-216">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span> <span data-ttu-id="d078f-217">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="d078f-217">For more information, see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

### <a name="filter-criteria-and-operators"></a><span data-ttu-id="d078f-218"><a name="FilterCriteria"> </a>Критерии фильтра и операторы</span><span class="sxs-lookup"><span data-stu-id="d078f-218"><a name="FilterCriteria"> </a>Filter Criteria and Operators</span></span>

<span data-ttu-id="d078f-219">В процессе установки критериев фильтра можно использовать все цифры и буквы, которые обычно вводятся в поле.</span><span class="sxs-lookup"><span data-stu-id="d078f-219">When you enter criteria, you can use all the numbers and letters that you normally use in the field.</span></span> <span data-ttu-id="d078f-220">Но есть также набор специальных символов, которые вы можете использовать в качестве операторов для дальнейшей фильтрации результатов.</span><span class="sxs-lookup"><span data-stu-id="d078f-220">But there's also a set of special symbols that you can use as operators to further filter the results.</span></span> <span data-ttu-id="d078f-221">В следующих разделах описаны эти символы и их использование в качестве операторов в фильтрах.</span><span class="sxs-lookup"><span data-stu-id="d078f-221">The following sections describe these symbols and how to use them as operators in filters.</span></span>

> [!TIP]
> <span data-ttu-id="d078f-222">Дополнительные сведения о фильтрации значений дат и времени см. в разделе [Работа с календарными датами и значениями времени](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="d078f-222">For more information about filtering dates and times, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

> [!IMPORTANT]
> - <span data-ttu-id="d078f-223">Могут быть ситуации, когда значение, которое вы хотите отфильтровать, содержит символ, являющийся оператором.</span><span class="sxs-lookup"><span data-stu-id="d078f-223">There may be situations where the value that you want to filter on contains a symbol that's an operator.</span></span> <span data-ttu-id="d078f-224">Дополнительные сведения об обработке этих ситуаций см. в разделе [Фильтрация значений, содержащих символы](#symbols) для получения дополнительных инструкций по работе в этой ситуации.</span><span class="sxs-lookup"><span data-stu-id="d078f-224">For more information about handling these situtions, see [Filtering on Values That Contain Symbols](#symbols) for more instructions about handling this situation.</span></span>
>
> - <span data-ttu-id="d078f-225">Если в одном фильтре более 200 операторов, система автоматически сгруппирует некоторые выражения в скобки `()` с целью обработки.</span><span class="sxs-lookup"><span data-stu-id="d078f-225">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span></span> <span data-ttu-id="d078f-226">Это не влияет на фильтр или результаты.</span><span class="sxs-lookup"><span data-stu-id="d078f-226">This has no effect on the filter or the results.</span></span>  

#### <a name="-interval"></a><span data-ttu-id="d078f-227">(..) Диапазон</span><span class="sxs-lookup"><span data-stu-id="d078f-227">(..) Interval</span></span>

|<span data-ttu-id="d078f-228">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-228">Sample Expression</span></span>|<span data-ttu-id="d078f-229">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-229">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="d078f-230">Номера от 1 100 до 2 100</span><span class="sxs-lookup"><span data-stu-id="d078f-230">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="d078f-231">До 2500, включительно</span><span class="sxs-lookup"><span data-stu-id="d078f-231">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="d078f-232">Даты по 31.12.00 включительно</span><span class="sxs-lookup"><span data-stu-id="d078f-232">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="d078f-233">Информация для 8-го учетного периода и позже</span><span class="sxs-lookup"><span data-stu-id="d078f-233">Information for accounting period 8 and after</span></span>|  
|`..23`|<span data-ttu-id="d078f-234">С даты начала по 23 число текущего месяца текущего года до 23:59:59</span><span class="sxs-lookup"><span data-stu-id="d078f-234">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="d078f-235">с 23 текущего месяца текущего года 00:00:00 до конца</span><span class="sxs-lookup"><span data-stu-id="d078f-235">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="d078f-236">с 22 текущего месяца текущего года 0:00:00 по 23 текущего месяца текущего года 23:59:59</span><span class="sxs-lookup"><span data-stu-id="d078f-236">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

#### <a name="124-eitheror"></a><span data-ttu-id="d078f-237">(&#124;) Или/или</span><span class="sxs-lookup"><span data-stu-id="d078f-237">(&#124;) Either/or</span></span>

|<span data-ttu-id="d078f-238">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-238">Sample Expression</span></span>|<span data-ttu-id="d078f-239">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-239">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1200|1300`|<span data-ttu-id="d078f-240">Номера со значением 1 200 или 1 300</span><span class="sxs-lookup"><span data-stu-id="d078f-240">Numbers with 1200 or 1300</span></span>|  

#### <a name="-not-equal-to"></a><span data-ttu-id="d078f-241">(<>) Не равно</span><span class="sxs-lookup"><span data-stu-id="d078f-241">(<>) Not equal to</span></span>  

|<span data-ttu-id="d078f-242">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-242">Sample Expression</span></span>|<span data-ttu-id="d078f-243">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-243">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="d078f-244">Все числа, кроме 0</span><span class="sxs-lookup"><span data-stu-id="d078f-244">All numbers except 0</span></span><br /><br /> <span data-ttu-id="d078f-245">Возможность использования Microsoft SQL Server позволяет комбинировать данный символ со знаками подстановки.</span><span class="sxs-lookup"><span data-stu-id="d078f-245">The SQL Server Option allows you to combine this symbol with a wild-card expression.</span></span> <span data-ttu-id="d078f-246">Например, <>A\* означает несоответствие любым текстам, начинающимся с А.</span><span class="sxs-lookup"><span data-stu-id="d078f-246">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

#### <a name="-greater-than"></a><span data-ttu-id="d078f-247">(>) Больше чем</span><span class="sxs-lookup"><span data-stu-id="d078f-247">(>) Greater than</span></span>  

|<span data-ttu-id="d078f-248">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-248">Sample Expression</span></span>|<span data-ttu-id="d078f-249">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-249">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="d078f-250">Числа больше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="d078f-250">Numbers greater than 1200</span></span>|  

#### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="d078f-251">(>=) Больше чем или равно</span><span class="sxs-lookup"><span data-stu-id="d078f-251">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="d078f-252">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-252">Sample Expression</span></span>|<span data-ttu-id="d078f-253">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-253">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="d078f-254">Номера больше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="d078f-254">Numbers greater than or equal to 1200</span></span>|  

#### <a name="-less-than"></a><span data-ttu-id="d078f-255">(<) Меньше чем</span><span class="sxs-lookup"><span data-stu-id="d078f-255">(<) Less than</span></span>  

|<span data-ttu-id="d078f-256">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-256">Sample Expression</span></span>|<span data-ttu-id="d078f-257">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-257">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="d078f-258">Номера меньше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="d078f-258">Numbers less than 1200</span></span>|  

#### <a name="-less-than-or-equal-to"></a><span data-ttu-id="d078f-259">(<=) Меньше или равно</span><span class="sxs-lookup"><span data-stu-id="d078f-259">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="d078f-260">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-260">Sample Expression</span></span>|<span data-ttu-id="d078f-261">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-261">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="d078f-262">Номера меньше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="d078f-262">Numbers less than or equal to 1200</span></span>|  

#### <a name="-and"></a><span data-ttu-id="d078f-263">(&) И</span><span class="sxs-lookup"><span data-stu-id="d078f-263">(&) And</span></span>  

|<span data-ttu-id="d078f-264">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-264">Sample Expression</span></span>|<span data-ttu-id="d078f-265">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-265">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="d078f-266">Числа больше 200 и меньше 1200</span><span class="sxs-lookup"><span data-stu-id="d078f-266">Numbers greater than 200 and less than 1200</span></span>|  

#### <a name="-an-exact-character-match"></a><span data-ttu-id="d078f-267">('') Точное совпадение символа</span><span class="sxs-lookup"><span data-stu-id="d078f-267">('') An exact character match</span></span>  

|<span data-ttu-id="d078f-268">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-268">Sample Expression</span></span>|<span data-ttu-id="d078f-269">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-269">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="d078f-270">Текст, точно соответствующий **man** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-270">Text that matches **man** exactly and is case-sensitive.</span></span>|  

#### <a name="-case-insensitive"></a><span data-ttu-id="d078f-271">(@) Без учета регистра</span><span class="sxs-lookup"><span data-stu-id="d078f-271">(@) Case insensitive</span></span>  

|<span data-ttu-id="d078f-272">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-272">Sample Expression</span></span>|<span data-ttu-id="d078f-273">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-273">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="d078f-274">Текст, начинающийся с **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-274">Text that starts with **man** and is case insensitive.</span></span>|  

#### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="d078f-275">(\*) Неопределенное количество неизвестных символов</span><span class="sxs-lookup"><span data-stu-id="d078f-275">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="d078f-276">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-276">Sample Expression</span></span>|<span data-ttu-id="d078f-277">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-277">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="d078f-278">Текст, который содержит **Co** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-278">Text that contains **Co** and is case-sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="d078f-279">Текст, который заканчивается на **Co** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-279">Text that ends with **Co"** and is case-sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="d078f-280">Текст, который начинается с **Co** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="d078f-280">Text that begins with **Co** and is case-sensitive.</span></span>|  

#### <a name="-one-unknown-character"></a><span data-ttu-id="d078f-281">(?) Один неизвестный символ</span><span class="sxs-lookup"><span data-stu-id="d078f-281">(?) One unknown character</span></span>  

|<span data-ttu-id="d078f-282">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-282">Sample Expression</span></span>|<span data-ttu-id="d078f-283">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-283">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="d078f-284">Такой текст, как **Hansen** или **Hanson**</span><span class="sxs-lookup"><span data-stu-id="d078f-284">Text such as **Hansen** or **Hanson**</span></span>|  

#### <a name="combined-format-expressions"></a><span data-ttu-id="d078f-285">Объединенные выражения форматов</span><span class="sxs-lookup"><span data-stu-id="d078f-285">Combined Format Expressions</span></span>  

|<span data-ttu-id="d078f-286">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-286">Sample Expression</span></span>|<span data-ttu-id="d078f-287">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-287">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`5999|8100..8490`|<span data-ttu-id="d078f-288">Включает все записи с номером 5999 или номерами от 8100 до 8490.</span><span class="sxs-lookup"><span data-stu-id="d078f-288">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|`..1299|1400..`|<span data-ttu-id="d078f-289">Все записи с номером меньше или равно 1299 или номером от 1400 или больше (все номера, кроме от 1300 до 1399).</span><span class="sxs-lookup"><span data-stu-id="d078f-289">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="d078f-290">Все записи с номерами больше 50 и меньше 100 (номера от 51 до 99).</span><span class="sxs-lookup"><span data-stu-id="d078f-290">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  

### <a name="filtering-on-values-that-contain-symbols"></a><a name="symbols"></a><span data-ttu-id="d078f-291">Фильтрация значений, содержащих символы</span><span class="sxs-lookup"><span data-stu-id="d078f-291">Filtering on Values That Contain Symbols</span></span>

<span data-ttu-id="d078f-292">Могут быть случаи, когда значения полей содержат один из следующих символов:</span><span class="sxs-lookup"><span data-stu-id="d078f-292">There may be cases where field values contain the one of the following symbols:</span></span>

- &
- <span data-ttu-id="d078f-293">(</span><span class="sxs-lookup"><span data-stu-id="d078f-293">(</span></span>
- <span data-ttu-id="d078f-294">)</span><span class="sxs-lookup"><span data-stu-id="d078f-294">)</span></span>
- =
- <span data-ttu-id="d078f-295">&#124;</span><span class="sxs-lookup"><span data-stu-id="d078f-295">&#124;</span></span>

<span data-ttu-id="d078f-296">Если вы хотите фильтровать по любому из этих символов, заключите выражение фильтра в одинарные кавычки (`'<expression with symbol>'`).</span><span class="sxs-lookup"><span data-stu-id="d078f-296">If you want to filter on any of these symbols, place the filter expression in single quotes (`'<expression with symbol>'`).</span></span> <span data-ttu-id="d078f-297">Например, если необходимо фильтровать записи, которые начинаются с текста *J & V*, выражение фильтра может имеет вид `'J & V*'`.</span><span class="sxs-lookup"><span data-stu-id="d078f-297">For example, if you wanted to filter on records that start with the text *J & V*, the filter expression would be `'J & V*'`.</span></span>

<span data-ttu-id="d078f-298">Для других символов это требование не требуется.</span><span class="sxs-lookup"><span data-stu-id="d078f-298">This requirement isn't necessary for other symbols.</span></span>

### <a name="filter-tokens"></a><span data-ttu-id="d078f-299"><a name="FilterTokens"> </a>Токены фильтра</span><span class="sxs-lookup"><span data-stu-id="d078f-299"><a name="FilterTokens"> </a>Filter Tokens</span></span>

<span data-ttu-id="d078f-300">При указании критериев фильтра можно также вводить слова, которые имеют специальное значение, называемые токенами фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-300">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="d078f-301">После ввода слова токена это слово заменяется значением или значениями, которые оно представляет.</span><span class="sxs-lookup"><span data-stu-id="d078f-301">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="d078f-302">Токены фильтра упрощают фильтрацию благодаря снижению потребности перехода между страницами для поиска значений, которые требуется добавить в фильтр.</span><span class="sxs-lookup"><span data-stu-id="d078f-302">Filter tokens make filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="d078f-303">В таблицах ниже описаны некоторые из токенов, которые можно вводить в качестве критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="d078f-303">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="d078f-304">Ваша организация может использовать настраиваемые токены.</span><span class="sxs-lookup"><span data-stu-id="d078f-304">Your organization may use custom tokens.</span></span> <span data-ttu-id="d078f-305">Для получения полного набора токенов, доступных вам, или для добавления дополнительных настраиваемых токенов обращайтесь к администратору.</span><span class="sxs-lookup"><span data-stu-id="d078f-305">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="d078f-306">Технические сведения см. в разделе [Добавление токенов фильтров](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span><span class="sxs-lookup"><span data-stu-id="d078f-306">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span></span>

#### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="d078f-307">(%me или %userid) Записи, назначенные вам</span><span class="sxs-lookup"><span data-stu-id="d078f-307">(%me or %userid) Records Assigned to You</span></span>

<span data-ttu-id="d078f-308">Используйте `%me` или `%userid` с поля фильтра, которые содержат код пользователя, например поле **Назначено коду пользователя** для отображения всех записей, которые назначены вам.</span><span class="sxs-lookup"><span data-stu-id="d078f-308">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="d078f-309">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-309">Sample Expression</span></span>|<span data-ttu-id="d078f-310">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-310">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="d078f-311">или</span><span class="sxs-lookup"><span data-stu-id="d078f-311">or</span></span><br />`%userid`|<span data-ttu-id="d078f-312">Записи, которые назначены вашей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="d078f-312">Records that are assigned to your user account.</span></span> |  

#### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="d078f-313">(%mycustomers) Клиенты в "Мои клиенты"</span><span class="sxs-lookup"><span data-stu-id="d078f-313">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="d078f-314">Используйте `%mycustomers` в поле **№** клиента для отображения всех записей для клиентов, которые входят в список **Мои клиенты** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="d078f-314">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="d078f-315">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-315">Sample Expression</span></span>|<span data-ttu-id="d078f-316">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-316">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="d078f-317">Клиенты в списке **Мои клиенты** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="d078f-317">Customers in the **My Customers** on your Role Center.</span></span> |  

#### <a name="myitems-items-in-my-items"></a><span data-ttu-id="d078f-318">(%myitems) Товары в списке "Мои товары"</span><span class="sxs-lookup"><span data-stu-id="d078f-318">(%myitems) Items in My Items</span></span>

<span data-ttu-id="d078f-319">Используйте `%myitems` в поле **№** товара для отображения всех записей для товаров, которые входят в список **Мои товары** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="d078f-319">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="d078f-320">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-320">Sample Expression</span></span>|<span data-ttu-id="d078f-321">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-321">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="d078f-322">Товары в списке **Мои товары** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="d078f-322">Items in the **My Items** on your Role Center.</span></span> |  

#### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="d078f-323">(%myvendors) Поставщики в списке "Мои поставщики"</span><span class="sxs-lookup"><span data-stu-id="d078f-323">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="d078f-324">Используйте `%myvendors` в поле **№** поставщика для отображения всех записей для поставщиков, которые входят в список **Мои поставщики** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="d078f-324">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="d078f-325">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="d078f-325">Sample Expression</span></span>|<span data-ttu-id="d078f-326">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="d078f-326">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="d078f-327">Поставщики в списке **Мои поставщики** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="d078f-327">Vendors in the **My Vendors** on your Role Center.</span></span> |  

## <a name="see-also"></a><span data-ttu-id="d078f-328">См. также</span><span class="sxs-lookup"><span data-stu-id="d078f-328">See Also</span></span>

[<span data-ttu-id="d078f-329">Вопросы и ответы по поиску и фильтрации</span><span class="sxs-lookup"><span data-stu-id="d078f-329">Searching and Filtering FAQ</span></span>](ui-search-filter-faq.yml)  
[<span data-ttu-id="d078f-330">Сохранение и персонализация представлений списков</span><span class="sxs-lookup"><span data-stu-id="d078f-330">Save and Personalize List Views</span></span>](ui-views.md)  
<span data-ttu-id="d078f-331">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d078f-331">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]