---
title: "Сортировка, поиск и фильтрация списков | Документы Майкрософт"
description: "Работайте в списках эффективно, выполняя поиск в своих данных, сортируя столбцы и уточняя результаты с помощью мощных символов фильтров и сочетаний клавиш."
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: f0cdb045d314a630e795ec744f2f4470d930835a
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="sorting-searching-and-filtering-lists"></a><span data-ttu-id="1fb8f-103">Сортировка, поиск и фильтрация списков</span><span class="sxs-lookup"><span data-stu-id="1fb8f-103">Sorting, Searching, and Filtering Lists</span></span>
<span data-ttu-id="1fb8f-104">Есть несколько вещей, которые могут помочь сканировать, искать и ограничивать записи в списке.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-104">There are a few things that you can do that will help you scan, find, and limit records in a list.</span></span> <span data-ttu-id="1fb8f-105">Сюда входят сортировка, поиск и фильтрация.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-105">These include sorting, searching and filtering.</span></span> <span data-ttu-id="1fb8f-106">Некоторые или все из них можно применить одновременно для быстрого поиска или анализа данных.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

> [!TIP]
> <span data-ttu-id="1fb8f-107">При просмотре ваших данных в виде плиток можно осуществлять поиск и использовать основную фильтрацию.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-107">When viewing your data as tiles, you can search and use basic filtering.</span></span> <span data-ttu-id="1fb8f-108">Чтобы использовать полный набор мощных функций для сортировки, поиска и фильтрации, выберите значок ![Показать как список](media/ui_show_as_list_icon.png "Показать как список стрелка влево") для отображения в виде списка.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-108">To use the full set of powerful features for sorting, searching and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to show as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="1fb8f-109">Сортировка</span><span class="sxs-lookup"><span data-stu-id="1fb8f-109">Sorting</span></span>
<span data-ttu-id="1fb8f-110">Сортировка позволяет быстро и легко получить общее представление о данных.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-110">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="1fb8f-111">При наличии большого числа клиентов, например, можно сортировать их по полю **Номер клиента**, **Учетная группа клиента**, **Код валюты**, **Код страны/региона** или **ИНН**, чтобы получить нужный обзор.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-111">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="1fb8f-112">Для сортировки списка можно либо выбрать текст заголовка столбца для переключения между порядком по возрастания или по убыванию, либо выбрать небольшую стрелку вниз в заголовке столбца, затем выбрать **По возрастанию** или **По убыванию**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-112">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small down arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="1fb8f-113">Не поддерживается сортировка изображений, полей BLOB, полей FlowFilter и полей, которые не принадлежат таблице.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-113">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="1fb8f-114">Поиск</span><span class="sxs-lookup"><span data-stu-id="1fb8f-114">Searching</span></span>
<span data-ttu-id="1fb8f-115"><!--## Searching by using the Quick Filter --> Вверху каждой страницы списке имеется значок ![Поиск в списке](media/ui-search/search-list.png "Значок поиска в списке") **Поиск**, который обеспечивает быстрый и простой способ уменьшения числа записей в списке и отображения только тех записей, которые содержат только интересующие вас данные.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-115"><!--## Searching by using the Quick Filter --> At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** icon that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span></span>

<span data-ttu-id="1fb8f-116">Для поиска просто выберите значок поиска, затем в поле введите текст, который требуется найти.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-116">To search, simply select the search icon, and then in the box, type the text that you are looking for.</span></span> <span data-ttu-id="1fb8f-117">Можно ввести буквы, цифры и другие символы.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-117">You can enter letters, numbers, and other symbols.</span></span>

### <a name="fine-tune-the-search"></a><span data-ttu-id="1fb8f-118">Уточнение поиска</span><span class="sxs-lookup"><span data-stu-id="1fb8f-118">Fine-tune the search</span></span>
<span data-ttu-id="1fb8f-119">В целом, поиск попытается найти текст во всех полях; он не различает символы верхнего и нижнего регистров (другие словами, нечувствителен к регистру), и будет находить текст в любом месте поля (в начале, в конце либо в центре).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-119">In general, search will attempt to match text across all fields; it does not distinguish between uppercase and lowercase characters (in other words, case insensitive), and will match text placed anwhere in the field (at the beginning, end, or in the middle).</span></span>

<span data-ttu-id="1fb8f-120">Однако можно выполнять более точный поиск с использованием следующих специальных знаков:</span><span class="sxs-lookup"><span data-stu-id="1fb8f-120">However, you can make a more exact search by using the following special characters:</span></span>

- <span data-ttu-id="1fb8f-121">Чтобы найти только значения полей, которые точно совпадают со всем текстом и регистром, заключите искомый текст в одинарные кавычки `''` (например, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-121">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="1fb8f-122">Чтобы найти только значения полей, которые начинаются с определенного текста с совпадающим регистром, поместите `*` после искомого текста (например, `man*`).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-122">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="1fb8f-123">Чтобы найти только значения полей, которые заканчиваются определенным текстом с учетом регистра, поместите `*` перед искомым текстом (например, `*man`).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-123">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="1fb8f-124">При использовании `''` или `*` поиск учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-124">When using  `''` or `*`, the search is case sensitive.</span></span> <span data-ttu-id="1fb8f-125">Если требуется делать поиск нечувствительным к регистру, установите `@` перед искомым текстом (например, `@man*`).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-125">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="1fb8f-126">В следующей таблице приведены некоторые примеры для объяснения как можно использовать поиск.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-126">The following table provides some examples to explain how you can use the search.</span></span>


<!--
In search criteria you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.-->

<!--
The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options. Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.  

* If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.  
* If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.
-->
<!--

|Search Criteria|Interpreted as...|Finds...|
|---------------|----------------|----------|
|`man`<br />or <br />`Man`|Contains the text; case insensitive|All records with fields that contain the text **man**, regardless of the case.|
|`'Man'`|Entire text match; case sensitive.|All records with fields that only contain **Man** exactly.|
|`Man*`|Starts with the text; case sensitive.|All records with fields that start with the text <b>Man</b> exactly.|
|`@Man*`|Starts with the text; case insensitive.|All records with fields that start with **man**, regardless of the case.|
|`@*man`|Ends with the text; case insensitive.|All records that end with **man**, regardless of the case.|
-->

|<span data-ttu-id="1fb8f-127">Критерии поиска</span><span class="sxs-lookup"><span data-stu-id="1fb8f-127">Search Criteria</span></span>|<span data-ttu-id="1fb8f-128">Находит...</span><span class="sxs-lookup"><span data-stu-id="1fb8f-128">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="1fb8f-129">или</span><span class="sxs-lookup"><span data-stu-id="1fb8f-129">or</span></span> <br />`Man`|<span data-ttu-id="1fb8f-130">Все записи с полями, которые содержат текст **man** независимо от регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-130">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="1fb8f-131">Например, **Manchester**, **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-131">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="1fb8f-132">Все записи с полями, которые содержат только **Man** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-132">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="1fb8f-133">Все записи с полями, которые начинаются с текста <b>Man</b> с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-133">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="1fb8f-134">Например, **Manchester**, но не **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-134">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="1fb8f-135">Все записи с полями, которые начинаются с текста **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-135">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="1fb8f-136">Например, **Manchester** и **manual**, но не **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-136">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="1fb8f-137">Все записи с полями, которые заканчиваются на **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-137">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="1fb8f-138">Например, **Sportsman**, но не **Manchester** или **manual**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-138">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|

> [!TIP]
> <span data-ttu-id="1fb8f-139">Можно нажать клавишу F3 для активации и деактивации поля поиска.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-139">You can press F3 to activate and deactivate the search box.</span></span> <span data-ttu-id="1fb8f-140">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-140">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

## <a name="filtering"></a><span data-ttu-id="1fb8f-141">Фильтрация</span><span class="sxs-lookup"><span data-stu-id="1fb8f-141">Filtering</span></span>
<span data-ttu-id="1fb8f-142">Фильтрация обеспечивает более широкие и разнообразные способы контроля того, как записи должны отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-142">Filtering provides a more advanced and versatile way of controlling which records display in a list.</span></span> <span data-ttu-id="1fb8f-143">Имеется два основных отличия между поиском и фильтрацией, как описано в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-143">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="1fb8f-144">**Поиск**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-144">**Searching**</span></span> | <span data-ttu-id="1fb8f-145">**фильтрация;**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-145">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="1fb8f-146">**Применимые поля**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-146">**Applicable fields**</span></span> | <span data-ttu-id="1fb8f-147">Производится поиск по всем полям, видимым на странице.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-147">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="1fb8f-148">Фильтрует одно или несколько полей по отдельности, выбирая из любого поля в таблице, включая поля, которые не отображаются на странице.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-148">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span></span> |
| <span data-ttu-id="1fb8f-149">**Соответствие**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-149">**Matching**</span></span> | <span data-ttu-id="1fb8f-150">Отображаются записи с полями, которые соответствуют тексту поиска, независимо от регистра или местоположения этого текста.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-150">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span></span> | <span data-ttu-id="1fb8f-151">Отображаются записи, в которых поле соответствует фильтру точно с учетом регистра, если не введены специальные символы фильтра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-151">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span></span>

<span data-ttu-id="1fb8f-152">Фильтрация позволяет отобразить записи для определенных организаций или клиентов, дат, сумм и иной информации путем определения критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-152">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="1fb8f-153">При этом отображаются только те записи, которые соответствуют заданным критериям.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-153">Only records that match the criteria are displayed.</span></span> <span data-ttu-id="1fb8f-154">Если критерии заданы для нескольких полей, отображаются только записи, которые соответствуют этим критериям.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-154">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

### <a name="working-in-the-filter-pane"></a><span data-ttu-id="1fb8f-155">Работа в области фильтров</span><span class="sxs-lookup"><span data-stu-id="1fb8f-155">Working in the filter pane</span></span>
<span data-ttu-id="1fb8f-156">Область фильтров показывает текущие фильтры для списка и позволяет задать собственные настраиваемые фильтры для одного или нескольких полей.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-156">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields.</span></span> <span data-ttu-id="1fb8f-157">На приведенном ниже рисунке показан пример области фильтров для списка предложений по продаже.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-157">The following figure shows an example filter pane for a Sales Quotes list.</span></span>

<span data-ttu-id="1fb8f-158">![Обзор области фильтров](media/filter-pane-overview.png "Значок фильтра")</span><span class="sxs-lookup"><span data-stu-id="1fb8f-158">![Filter pane overview ](media/filter-pane-overview.png "Filter icon")</span></span>

<span data-ttu-id="1fb8f-159">Для отображения области фильтров используйте сочетание клавиш **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-159">To display the filter pane, use the **Shift+F3** keyboard shortcut.</span></span> <span data-ttu-id="1fb8f-160">Для списков в ролевом центре можно также выбрать стрелку вниз рядом с заголовком страницы в навигационной панели над списком, затем выбрать **Показать область фильтров**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-160">For lists within the Role Center, you can also choose the down arrow near the page title in the navigation bar above the list, and then choose **Show filter pane**.</span></span>

<span data-ttu-id="1fb8f-161">![Показать область фильтров](media/open-filter-pane.png "Показать область фильтров")</span><span class="sxs-lookup"><span data-stu-id="1fb8f-161">![Show filter pane](media/open-filter-pane.png "Show filter pane")</span></span>

<span data-ttu-id="1fb8f-162">Область фильтров разделена на три раздела: **Представления**, **Фильтровать список по** и **Фильтровать итоги по**:</span><span class="sxs-lookup"><span data-stu-id="1fb8f-162">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="1fb8f-163">**Представления**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-163">**Views**</span></span>

  <span data-ttu-id="1fb8f-164">Некоторые списки включают раздел **Представления**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-164">Some lists will include the **Views** section.</span></span> <span data-ttu-id="1fb8f-165">Представления являются вариациями списка, которые были заранее настроены с помощью фильтров.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-165">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="1fb8f-166">Чтобы перейти к другому представлению списка просто выберите другую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-166">To switch to a different view of your list, simply select another link.</span></span> <span data-ttu-id="1fb8f-167">Можно временно изменить фильтры в представлении, но изменения не будут сохраняться постоянно.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-167">You can temporarily change the filters on a view, but the changes will not be permanently saved.</span></span>

- <span data-ttu-id="1fb8f-168">**Фильтровать список по**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-168">**Filter list by**</span></span>

  <span data-ttu-id="1fb8f-169">В разделе **Фильтровать список по** можно добавлять фильтры по конкретным полям для сокращения числа отображаемых записей.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-169">The **Filter list by** section is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="1fb8f-170">Для добавления фильтра выберите **+ Фильтр**, выберите поле, которое необходимо фильтровать из любого поля в таблице, затем введите критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-170">To add a filter, select **+ Filter**, select the field that you want to filter from any field in the table, and then enter filter criteria in the box.</span></span>

- <span data-ttu-id="1fb8f-171">**Фильтровать итоги по**</span><span class="sxs-lookup"><span data-stu-id="1fb8f-171">**Filter totals by**</span></span>

  <span data-ttu-id="1fb8f-172">Некоторые списки, в которых отображаются вычисляемые поля, такие как суммы и количества, будут содержать раздел **Фильтровать итоги по** для изменения различных измерений, воздействующих на расчеты.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-172">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="1fb8f-173">Например, можно быстро анализировать план счетов, фильтруя суммы за определенный период, или можно просмотреть итоги только для заказов на продажу с определенного склада.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-173">For example, you can quickly analyze your chart of accounts by filtering amounts to a specific period, or you can view the totals for sales orders only from a specific warehouse.</span></span>

  <span data-ttu-id="1fb8f-174">Для добавления фильтра выберите **+ Фильтр**, выберите одно из предопределенных измерений, затем добавьте критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-174">To add a filter, select **+ Filter**, select one of the predefined dimensions, and then add the filter criteria in the box.</span></span>

  > [!NOTE]
  > <span data-ttu-id="1fb8f-175">Фильтры в разделе **Фильтровать итоги по** управляются элементами FlowFilter в дизайне страницы.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-175">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="1fb8f-176">Технические сведения см. в разделе [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-176">For technical information, see [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>


### <a name="entering-filter-criteria-in-the-filter-pane"></a><span data-ttu-id="1fb8f-177">Ввод критериев фильтра в области фильтров</span><span class="sxs-lookup"><span data-stu-id="1fb8f-177">Entering filter criteria in the filter pane</span></span>
<span data-ttu-id="1fb8f-178">Чтобы выбрать поле для фильтра, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="1fb8f-178">To select a field to filter, do one of the following:</span></span>
  - <span data-ttu-id="1fb8f-179">В области фильтров выберите **+ Поле**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-179">In the filter pane, choose **+ Field**.</span></span> <span data-ttu-id="1fb8f-180">Введите название поля, которое необходимо фильтровать, или выберите поле в меню, в котором отображаются все поля в таблице.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-180">Type the name of the field you wish to filter, or pick a field from the menu that displays all fields in the table.</span></span>

  - <span data-ttu-id="1fb8f-181">Выберите в заголовке столбца стрелку вниз, затем выберите **Фильтр...**. Это приведет к открытию область фильтров и добавит столбец в область фильтров.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-181">In a column heading, choose the down arrow, and then choose **Filter...**. This will open the filter pane and add the column to the filter pane.</span></span>

<span data-ttu-id="1fb8f-182">Теперь можно ввести или выбрать критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-182">You can now type or select your filter criteria in the box.</span></span> <span data-ttu-id="1fb8f-183">Тип фильтруемого поля определяет, какие критерии можно ввести.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-183">The type of field you filter determines which criteria you can enter.</span></span> <span data-ttu-id="1fb8f-184">Например, при фильтрации поля, которое имеет фиксированные значения, можно выбирать только из этих значений.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-184">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="1fb8f-185">Дополнительные сведения об особенных знаках фильтров см. в разделах [Критерии фильтра](#FilterCriteria) и [Токены фильтра](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-185">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="1fb8f-186">Столбцы, которые уже содержат фильтры, обозначаются ![Значок фильтра](media/ui-search/filter-icon.png "Значок фильтра") в заголовке столбцов.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-186">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") in the column heading.</span></span> <span data-ttu-id="1fb8f-187">Чтобы снять фильтр, выберите заголовок столбца и выберите **Очистить фильтр**.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-187">To remove a filter, select the column heading, then choose **Clear Filter**.</span></span>


### <a name="entering-filter-criteria-without-the-filter-pane"></a><span data-ttu-id="1fb8f-188">Ввод критериев фильтра без области фильтров</span><span class="sxs-lookup"><span data-stu-id="1fb8f-188">Entering filter criteria without the filter pane</span></span>
<span data-ttu-id="1fb8f-189">Можно определить простые фильтры непосредственно в списке без использования области фильтров.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-189">You can specify simple filters directly within the list without having to use the filter pane.</span></span>
<span data-ttu-id="1fb8f-190">С любым полем, выбранным в строке, используйте сочетание клавиш **Alt+F3** для отображения только записей, имеющих это же значение.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-190">With any field selected on a row, use the **Alt+F3** keyboard shortcut to display only the records having that same value.</span></span> <span data-ttu-id="1fb8f-191">Затем можно выбрать другое поле и снова использовать это же сочетание клавиш, чтобы продолжить уточнять фильтры.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-191">You can then select another field and use the same shortcut again to continue refining your filters.</span></span> <span data-ttu-id="1fb8f-192">Если выбрано поле уже содержит фильтр, при использовании **Alt+F3** этот фильтр очищается.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-192">If the selected field is already filtered, using **Alt+F3** will clear that filter.</span></span>

> [!TIP]
> <span data-ttu-id="1fb8f-193">Ускорьте поиск и анализ данных с помощью сочетаний клавиш.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-193">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="1fb8f-194">Например, выберите поле, используйте **Shift+Alt+F3** для добавления этого поля к области фильтров, введите критерии фильтра, используйте **Ctrl+Enter** для возврата в строки, выберите другое поле, используйте **Alt+F3** для фильтрации по этому значению.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-194">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span>
<span data-ttu-id="1fb8f-195">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-195">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>


## <span data-ttu-id="1fb8f-196"><a name="FilterCriteria"> </a>Критерии фильтра и символы</span><span class="sxs-lookup"><span data-stu-id="1fb8f-196"><a name="FilterCriteria"> </a>Filter criteria and symbols</span></span>
<span data-ttu-id="1fb8f-197">В процессе установки критериев фильтра можно использовать все цифры и буквы, которые обычно вводятся в поле.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-197">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="1fb8f-198">Кроме того, для дополнительной фильтрации результатов можно использовать специальные символы.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-198">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="1fb8f-199">В следующих таблицах приведены символы, которые могут быть использованы в фильтрах.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-199">The following tables show the symbols which can be used in filters.</span></span> <span data-ttu-id="1fb8f-200">Для дат и времени также можно получить более подробную информацию в разделе [Работа с датами и временем в календаре](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-200">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="1fb8f-201">Могут быть ситуации, когда значения поля содержит эти символы, и требуется фильтрация по ним.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-201">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="1fb8f-202">Чтобы это сделать, необходимо включить выражение фильтра, которое содержит данный символ в кавычках (").</span><span class="sxs-lookup"><span data-stu-id="1fb8f-202">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="1fb8f-203">Например, если необходимо фильтровать записи, которые начинаются с текста *S&R*, выражение фильтра имеет вид `'S&R*'`.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-203">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span></span>  

### <a name="-interval"></a><span data-ttu-id="1fb8f-204">(..) Диапазон</span><span class="sxs-lookup"><span data-stu-id="1fb8f-204">(..) Interval</span></span>

|<span data-ttu-id="1fb8f-205">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-205">Sample Expression</span></span>|<span data-ttu-id="1fb8f-206">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-206">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="1fb8f-207">Номера от 1 100 до 2 100</span><span class="sxs-lookup"><span data-stu-id="1fb8f-207">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="1fb8f-208">До 2500, включительно</span><span class="sxs-lookup"><span data-stu-id="1fb8f-208">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="1fb8f-209">Даты по 31.12.00 включительно</span><span class="sxs-lookup"><span data-stu-id="1fb8f-209">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="1fb8f-210">Информация для 8-го учетного периода и позже.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-210">Information for accounting period 8 and thereafter</span></span>|  
|`..23`|<span data-ttu-id="1fb8f-211">С даты начала по 23 число текущего месяца текущего года до 23:59:59</span><span class="sxs-lookup"><span data-stu-id="1fb8f-211">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="1fb8f-212">с 23 текущего месяца текущего года 00:00:00 до конца</span><span class="sxs-lookup"><span data-stu-id="1fb8f-212">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="1fb8f-213">с 22 текущего месяца текущего года 0:00:00 по 23 текущего месяца текущего года 23:59:59</span><span class="sxs-lookup"><span data-stu-id="1fb8f-213">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

### <a name="124-eitheror"></a><span data-ttu-id="1fb8f-214">(&#124;) Либо/или</span><span class="sxs-lookup"><span data-stu-id="1fb8f-214">(&#124;) Either/or</span></span>  

|<span data-ttu-id="1fb8f-215">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-215">Sample Expression</span></span>|<span data-ttu-id="1fb8f-216">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-216">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="1fb8f-217">\`1200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-217">\`1200</span></span>|<span data-ttu-id="1fb8f-218">1300\`</span><span class="sxs-lookup"><span data-stu-id="1fb8f-218">1300\`</span></span>|<span data-ttu-id="1fb8f-219">Номера со значением 1 200 или 1 300</span><span class="sxs-lookup"><span data-stu-id="1fb8f-219">Numbers with 1200 or 1300</span></span>|  

### <a name="-not-equal-to"></a><span data-ttu-id="1fb8f-220">(<>) Не равно</span><span class="sxs-lookup"><span data-stu-id="1fb8f-220">(<>) Not equal to</span></span>  

|<span data-ttu-id="1fb8f-221">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-221">Sample Expression</span></span>|<span data-ttu-id="1fb8f-222">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="1fb8f-223">Все числа, кроме 0</span><span class="sxs-lookup"><span data-stu-id="1fb8f-223">All numbers except 0</span></span><br /><br /> <span data-ttu-id="1fb8f-224">Возможность использования Microsoft SQL Server позволяет комбинировать данный символ со знаками подстановки.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-224">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="1fb8f-225">Например, <>A\* означает несоответствие любым текстам, начинающимся с А.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-225">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

### <a name="-greater-than"></a><span data-ttu-id="1fb8f-226">(>) Больше чем</span><span class="sxs-lookup"><span data-stu-id="1fb8f-226">(>) Greater than</span></span>  

|<span data-ttu-id="1fb8f-227">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-227">Sample Expression</span></span>|<span data-ttu-id="1fb8f-228">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-228">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="1fb8f-229">Числа больше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-229">Numbers greater than 1200</span></span>|  

### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="1fb8f-230">(>=) Больше чем или равно</span><span class="sxs-lookup"><span data-stu-id="1fb8f-230">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="1fb8f-231">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-231">Sample Expression</span></span>|<span data-ttu-id="1fb8f-232">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="1fb8f-233">Номера больше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-233">Numbers greater than or equal to 1200</span></span>|  

### <a name="-less-than"></a><span data-ttu-id="1fb8f-234">(<) Меньше чем</span><span class="sxs-lookup"><span data-stu-id="1fb8f-234">(<) Less than</span></span>  

|<span data-ttu-id="1fb8f-235">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-235">Sample Expression</span></span>|<span data-ttu-id="1fb8f-236">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-236">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="1fb8f-237">Номера меньше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-237">Numbers less than 1200</span></span>|  

### <a name="-less-than-or-equal-to"></a><span data-ttu-id="1fb8f-238">(<=) Меньше или равно</span><span class="sxs-lookup"><span data-stu-id="1fb8f-238">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="1fb8f-239">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-239">Sample Expression</span></span>|<span data-ttu-id="1fb8f-240">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-240">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="1fb8f-241">Номера меньше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-241">Numbers less than or equal to 1200</span></span>|  

### <a name="-and"></a><span data-ttu-id="1fb8f-242">(&) И</span><span class="sxs-lookup"><span data-stu-id="1fb8f-242">(&) And</span></span>  

|<span data-ttu-id="1fb8f-243">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-243">Sample Expression</span></span>|<span data-ttu-id="1fb8f-244">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-244">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="1fb8f-245">Числа больше 200 и меньше 1200</span><span class="sxs-lookup"><span data-stu-id="1fb8f-245">Numbers greater than 200 and less than 1200</span></span>|  

### <a name="-an-exact-character-match"></a><span data-ttu-id="1fb8f-246">('') Точное совпадение символа</span><span class="sxs-lookup"><span data-stu-id="1fb8f-246">('') An exact character match</span></span>  

|<span data-ttu-id="1fb8f-247">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-247">Sample Expression</span></span>|<span data-ttu-id="1fb8f-248">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-248">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="1fb8f-249">Текст, точно соответствующий man с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-249">Text that matches man exactly and is case sensitive.</span></span>|  

### <a name="-case-insensitive"></a><span data-ttu-id="1fb8f-250">(@) Без учета регистра</span><span class="sxs-lookup"><span data-stu-id="1fb8f-250">(@) Case insensitive</span></span>  

|<span data-ttu-id="1fb8f-251">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-251">Sample Expression</span></span>|<span data-ttu-id="1fb8f-252">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-252">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="1fb8f-253">Текст, начинающийся с man без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-253">Text that starts with man and is case insensitive.</span></span>|  

### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="1fb8f-254">(\*) Неопределенное количество неизвестных символов</span><span class="sxs-lookup"><span data-stu-id="1fb8f-254">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="1fb8f-255">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-255">Sample Expression</span></span>|<span data-ttu-id="1fb8f-256">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-256">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="1fb8f-257">Текст, который содержит "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-257">Text that contains "Co" and is case sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="1fb8f-258">Текст, который заканчивается на "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-258">Text that ends with "Co" and is case sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="1fb8f-259">Текст, который начинается с "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-259">Text that begins with "Co" and is case sensitive.</span></span>|  

> [!NOTE]  
>   <span data-ttu-id="1fb8f-260">Нельзя использовать `*` при фильтрации в полях параметров (перечислений), например в поле **Статус** заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-260">You cannot use `*` when filtering on option (enumeration) fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="1fb8f-261">Чтобы ввести фильтр для данного типа поля, можно ввести в качестве параметра фильтра числовое значение.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-261">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="1fb8f-262">Например, в поле **Статус** в заказе на продажу, которое имеет значения **Открыть**, **Выпущено**, **Ожидает утверждения** и **Ожидает предоплаты**, используйте значения `0`, `1`, `2` и `3` для фильтрации этих параметров.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-262">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values `0`, `1`, `2`, and `3` to filter for these options.</span></span>

### <a name="-one-unknown-character"></a><span data-ttu-id="1fb8f-263">(?) Один неизвестный символ</span><span class="sxs-lookup"><span data-stu-id="1fb8f-263">(?) One unknown character</span></span>  

|<span data-ttu-id="1fb8f-264">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-264">Sample Expression</span></span>|<span data-ttu-id="1fb8f-265">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-265">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="1fb8f-266">Такой текст, как «Стул» или «Стол»</span><span class="sxs-lookup"><span data-stu-id="1fb8f-266">Text such as Hansen or Hanson</span></span>|  

### <a name="combined-format-expressions"></a><span data-ttu-id="1fb8f-267">Объединенные выражения форматов</span><span class="sxs-lookup"><span data-stu-id="1fb8f-267">Combined format expressions</span></span>  

|<span data-ttu-id="1fb8f-268">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-268">Sample Expression</span></span>|<span data-ttu-id="1fb8f-269">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-269">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="1fb8f-270">\`5999</span><span class="sxs-lookup"><span data-stu-id="1fb8f-270">\`5999</span></span>|<span data-ttu-id="1fb8f-271">8100..8490\`</span><span class="sxs-lookup"><span data-stu-id="1fb8f-271">8100..8490\`</span></span>|<span data-ttu-id="1fb8f-272">Включает все записи с номером 5999 или номерами от 8100 до 8490.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-272">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="1fb8f-273">\`..1299</span><span class="sxs-lookup"><span data-stu-id="1fb8f-273">\`..1299</span></span>|<span data-ttu-id="1fb8f-274">1400..\`</span><span class="sxs-lookup"><span data-stu-id="1fb8f-274">1400..\`</span></span>|<span data-ttu-id="1fb8f-275">Все записи с номером меньше или равно 1299 или номером от 1400 или больше (все номера, кроме от 1300 до 1399).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-275">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="1fb8f-276">Все записи с номерами больше 50 и меньше 100 (номера от 51 до 99).</span><span class="sxs-lookup"><span data-stu-id="1fb8f-276">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  


## <span data-ttu-id="1fb8f-277"><a name="FilterTokens"> </a>Токены фильтра</span><span class="sxs-lookup"><span data-stu-id="1fb8f-277"><a name="FilterTokens"> </a>Filter tokens</span></span>
<span data-ttu-id="1fb8f-278">При указании критериев фильтра можно также вводить слова, которые имеют специальное значение, называемые токенами фильтра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-278">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="1fb8f-279">После ввода слова токена это слово заменяется значением или значениями, которые оно представляет.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-279">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="1fb8f-280">Это упрощает фильтрацию благодаря снижению потребности перехода между страницами для поиска значений, которые требуется добавить в фильтр.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-280">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="1fb8f-281">В таблицах ниже описаны некоторые из токенов, которые можно вводить в качестве критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-281">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="1fb8f-282">Ваша организация может использовать настраиваемые токены.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-282">Your organization may use custom tokens.</span></span> <span data-ttu-id="1fb8f-283">Для получения полного набора токенов, доступных вам, или для добавления дополнительных настраиваемых токенов обращайтесь к администратору.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-283">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="1fb8f-284">Технические сведения см. в разделе [Добавление токенов фильтров](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens)</span><span class="sxs-lookup"><span data-stu-id="1fb8f-284">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens)</span></span>


### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="1fb8f-285">(%me или %userid) Записи, назначенные вам</span><span class="sxs-lookup"><span data-stu-id="1fb8f-285">(%me or %userid) Records assigned to you</span></span>

<span data-ttu-id="1fb8f-286">Используйте `%me` или `%userid` с поля фильтра, которые содержат код пользователя, например поле **Назначено коду пользователя** для отображения всех записей, которые назначены вам.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-286">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="1fb8f-287">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-287">Sample Expression</span></span>|<span data-ttu-id="1fb8f-288">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-288">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="1fb8f-289">или</span><span class="sxs-lookup"><span data-stu-id="1fb8f-289">or</span></span><br />`%userid`|<span data-ttu-id="1fb8f-290">Записи, которые назначены вашей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-290">Records the are assigned to your user account.</span></span> |  

### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="1fb8f-291">(%mycustomers) Клиенты в "Мои клиенты"</span><span class="sxs-lookup"><span data-stu-id="1fb8f-291">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="1fb8f-292">Используйте `%mycustomers` в поле **№** клиента для отображения всех записей для клиентов, которые входят в список **Мои клиенты** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-292">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="1fb8f-293">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-293">Sample Expression</span></span>|<span data-ttu-id="1fb8f-294">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-294">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="1fb8f-295">Клиенты в списке **Мои клиенты** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-295">Customers in the **My Customers** on your Role Center.</span></span> |  

### <a name="myitems-items-in-my-items"></a><span data-ttu-id="1fb8f-296">(%myitems) Товары в списке "Мои товары"</span><span class="sxs-lookup"><span data-stu-id="1fb8f-296">(%myitems) Items in My Items</span></span>

<span data-ttu-id="1fb8f-297">Используйте `%myitems` в поле **№** товара для отображения всех записей для товаров, которые входят в список **Мои товары** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-297">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="1fb8f-298">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-298">Sample Expression</span></span>|<span data-ttu-id="1fb8f-299">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-299">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="1fb8f-300">Товары в списке **Мои товары** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-300">Items in the **My Items** on your Role Center.</span></span> |  

### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="1fb8f-301">(%myvendors) Поставщики в списке "Мои поставщики"</span><span class="sxs-lookup"><span data-stu-id="1fb8f-301">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="1fb8f-302">Используйте `%myvendors` в поле **№** поставщика для отображения всех записей для поставщиков, которые входят в список **Мои поставщики** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-302">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="1fb8f-303">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="1fb8f-303">Sample Expression</span></span>|<span data-ttu-id="1fb8f-304">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="1fb8f-304">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="1fb8f-305">Поставщики в списке **Мои поставщики** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="1fb8f-305">Venders in the **My Vendors** on your Role Center.</span></span> |  


## <a name="see-also"></a><span data-ttu-id="1fb8f-306">См. также</span><span class="sxs-lookup"><span data-stu-id="1fb8f-306">See Also</span></span>
<span data-ttu-id="1fb8f-307">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1fb8f-307">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="1fb8f-308">Общие вопросы и поиске и фильтрации</span><span class="sxs-lookup"><span data-stu-id="1fb8f-308">Common questions about Searching and Filtering</span></span>](ui-search-filter-faq.md)

