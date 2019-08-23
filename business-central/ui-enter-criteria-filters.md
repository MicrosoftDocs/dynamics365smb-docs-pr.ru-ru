---
title: Сортировка, поиск и фильтрация списков | Документы Майкрософт
description: Работайте в списках эффективно, выполняя поиск в своих данных, сортируя столбцы и уточняя результаты с помощью мощных символов фильтров и сочетаний клавиш.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter, totals, limit, advanced
ms.date: 06/13/2019
ms.author: sgroespe
ms.openlocfilehash: 5f3bab58a2387f5bf21042da782756f7b36d4792
ms.sourcegitcommit: f5050fd209b8d66722c81abe48c4c0a6f749a1f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "1740506"
---
# <a name="sorting-searching-and-filtering-lists"></a><span data-ttu-id="77ff9-103">Сортировка, поиск и фильтрация списков</span><span class="sxs-lookup"><span data-stu-id="77ff9-103">Sorting, Searching, and Filtering Lists</span></span>
<span data-ttu-id="77ff9-104">Есть несколько вещей, которые могут помочь сканировать, искать и ограничивать записи в списке.</span><span class="sxs-lookup"><span data-stu-id="77ff9-104">There are a few things that you can do that will help you scan, find, and limit records in a list.</span></span> <span data-ttu-id="77ff9-105">Сюда входят сортировка, поиск и фильтрация.</span><span class="sxs-lookup"><span data-stu-id="77ff9-105">These include sorting, searching and filtering.</span></span> <span data-ttu-id="77ff9-106">Некоторые или все из них можно применить одновременно для быстрого поиска или анализа данных.</span><span class="sxs-lookup"><span data-stu-id="77ff9-106">You can apply some or all of these simultaneously to quickly find or analyze your data.</span></span>

> [!TIP]
> <span data-ttu-id="77ff9-107">При просмотре ваших данных в виде плиток можно осуществлять поиск и использовать основную фильтрацию.</span><span class="sxs-lookup"><span data-stu-id="77ff9-107">When viewing your data as tiles, you can search and use basic filtering.</span></span> <span data-ttu-id="77ff9-108">Чтобы использовать полный набор мощных функций для сортировки, поиска и фильтрации, выберите значок ![Показать как список](media/ui_show_as_list_icon.png "Показать как список стрелка влево") для отображения в виде списка.</span><span class="sxs-lookup"><span data-stu-id="77ff9-108">To use the full set of powerful features for sorting, searching and filtering, choose the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to show as a list.</span></span>

<!--
When you want to search for data, such as customer names, addresses, or product groups, you enter criteria. In search criteria you can use all the numbers and letters that you normally use in the specific field. In addition, you can use special symbols to further filter the results. There are two ways to search: using the Quick Filter or column filters.
-->

## <a name="sorting"></a><span data-ttu-id="77ff9-109">Сортировка</span><span class="sxs-lookup"><span data-stu-id="77ff9-109">Sorting</span></span>
<span data-ttu-id="77ff9-110">Сортировка позволяет быстро и легко получить общее представление о данных.</span><span class="sxs-lookup"><span data-stu-id="77ff9-110">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="77ff9-111">При наличии большого числа клиентов, например, можно сортировать их по полю **Номер клиента**, **Учетная группа клиента**, **Код валюты**, **Код страны/региона** или **ИНН**, чтобы получить нужный обзор.</span><span class="sxs-lookup"><span data-stu-id="77ff9-111">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="77ff9-112">Для сортировки списка можно либо выбрать текст заголовка столбца для переключения между порядком по возрастания или по убыванию, либо выбрать небольшую стрелку вниз в заголовке столбца, затем выбрать **По возрастанию** или **По убыванию**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-112">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small down arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="77ff9-113">Не поддерживается сортировка изображений, полей BLOB, полей FlowFilter и полей, которые не принадлежат таблице.</span><span class="sxs-lookup"><span data-stu-id="77ff9-113">Sorting is not supported on images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching"></a><span data-ttu-id="77ff9-114">Поиск</span><span class="sxs-lookup"><span data-stu-id="77ff9-114">Searching</span></span>
<!--## Searching by using the Quick Filter -->
<span data-ttu-id="77ff9-115">Вверху каждой страницы списке имеется значок ![Поиск в списке](media/ui-search/search-list.png "Значок поиска в списке") **Поиск**, который обеспечивает быстрый и простой способ уменьшения числа записей в списке и отображения только тех записей, которые содержат только интересующие вас данные.</span><span class="sxs-lookup"><span data-stu-id="77ff9-115">At the top of each list page, there is a ![Search list](media/ui-search/search-list.png "Search list icon") **Search** icon that provides a quick and easy way to reduce the records in a list and display only those records that contain the data that you are interested in seeing.</span></span>

<span data-ttu-id="77ff9-116">Для поиска просто выберите значок поиска, затем в поле введите текст, который требуется найти.</span><span class="sxs-lookup"><span data-stu-id="77ff9-116">To search, simply select the search icon, and then in the box, type the text that you are looking for.</span></span> <span data-ttu-id="77ff9-117">Можно ввести буквы, цифры и другие символы.</span><span class="sxs-lookup"><span data-stu-id="77ff9-117">You can enter letters, numbers, and other symbols.</span></span>

### <a name="fine-tuning-the-search"></a><span data-ttu-id="77ff9-118">Уточнение поиска</span><span class="sxs-lookup"><span data-stu-id="77ff9-118">Fine-tuning the Search</span></span>
<span data-ttu-id="77ff9-119">В целом, поиск попытается найти текст во всех полях; он не различает символы верхнего и нижнего регистров (другие словами, нечувствителен к регистру), и будет находить текст в любом месте поля (в начале, в конце либо в центре).</span><span class="sxs-lookup"><span data-stu-id="77ff9-119">In general, search will attempt to match text across all fields; it does not distinguish between uppercase and lowercase characters (in other words, case insensitive), and will match text placed anywhere in the field (at the beginning, end, or in the middle).</span></span>

<span data-ttu-id="77ff9-120">Однако можно выполнять более точный поиск с использованием следующих специальных знаков:</span><span class="sxs-lookup"><span data-stu-id="77ff9-120">However, you can make a more exact search by using the following special characters:</span></span>

- <span data-ttu-id="77ff9-121">Чтобы найти только значения полей, которые точно совпадают со всем текстом и регистром, заключите искомый текст в одинарные кавычки `''` (например, `'man'`).</span><span class="sxs-lookup"><span data-stu-id="77ff9-121">To find only field values that match the entire text and case exactly, place the search text between single quotes `''` (for example, `'man'`).</span></span>

- <span data-ttu-id="77ff9-122">Чтобы найти только значения полей, которые начинаются с определенного текста с совпадающим регистром, поместите `*` после искомого текста (например, `man*`).</span><span class="sxs-lookup"><span data-stu-id="77ff9-122">To find field values that start with a certain text and match the case, place `*` after the search text (for example `man*`).</span></span>

- <span data-ttu-id="77ff9-123">Чтобы найти только значения полей, которые заканчиваются определенным текстом с учетом регистра, поместите `*` перед искомым текстом (например, `*man`).</span><span class="sxs-lookup"><span data-stu-id="77ff9-123">To find field values that end with a certain text and match the case, place `*` before the search text (for example `*man`).</span></span>

- <span data-ttu-id="77ff9-124">При использовании `''` или `*` поиск учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="77ff9-124">When using  `''` or `*`, the search is case sensitive.</span></span> <span data-ttu-id="77ff9-125">Если требуется делать поиск нечувствительным к регистру, установите `@` перед искомым текстом (например, `@man*`).</span><span class="sxs-lookup"><span data-stu-id="77ff9-125">If you want to make the search case insensitive, place `@` before the search text (for example `@man*`).</span></span>

<span data-ttu-id="77ff9-126">В следующей таблице приведены некоторые примеры для объяснения как можно использовать поиск.</span><span class="sxs-lookup"><span data-stu-id="77ff9-126">The following table provides some examples to explain how you can use the search.</span></span>

|<span data-ttu-id="77ff9-127">Критерии поиска</span><span class="sxs-lookup"><span data-stu-id="77ff9-127">Search Criteria</span></span>|<span data-ttu-id="77ff9-128">Находит...</span><span class="sxs-lookup"><span data-stu-id="77ff9-128">Finds...</span></span>|
|---------------|----------|
|`man`<br /><span data-ttu-id="77ff9-129">или</span><span class="sxs-lookup"><span data-stu-id="77ff9-129">or</span></span> <br />`Man`|<span data-ttu-id="77ff9-130">Все записи с полями, которые содержат текст **man** независимо от регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-130">All records with fields that contain the text **man**, regardless of the case.</span></span> <span data-ttu-id="77ff9-131">Например, **Manchester**, **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-131">For example, **Manchester**, **manual**, or **Sportsman**.</span></span> |
|`'Man'`|<span data-ttu-id="77ff9-132">Все записи с полями, которые содержат только **Man** с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-132">All records with fields that contain only **Man**, matching the case.</span></span>|
|`Man*`|<span data-ttu-id="77ff9-133">Все записи с полями, которые начинаются с текста <b>Man</b> с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-133">All records with fields that start with the text <b>Man</b>, matching the case.</span></span> <span data-ttu-id="77ff9-134">Например, **Manchester**, но не **manual** или **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-134">For example, **Manchester** but not **manual** or **Sportsman**.</span></span>|
|`@Man*`|<span data-ttu-id="77ff9-135">Все записи с полями, которые начинаются с текста **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-135">All records with fields that start with **man**, regardless of the case.</span></span> <span data-ttu-id="77ff9-136">Например, **Manchester** и **manual**, но не **Sportsman**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-136">For example, **Manchester** and **manual**, but not **Sportsman**.</span></span>|
|`@*man`|<span data-ttu-id="77ff9-137">Все записи с полями, которые заканчиваются на **man** без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-137">All records that end with **man**, regardless of the case.</span></span> <span data-ttu-id="77ff9-138">Например, **Sportsman**, но не **Manchester** или **manual**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-138">For example **Sportsman**, but not **Manchester** or **manual**.</span></span>|

> [!TIP]
> <span data-ttu-id="77ff9-139">Можно нажать клавишу F3 для активации и деактивации поля поиска.</span><span class="sxs-lookup"><span data-stu-id="77ff9-139">You can press F3 to activate and deactivate the search box.</span></span> <span data-ttu-id="77ff9-140">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="77ff9-140">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>

## <span data-ttu-id="77ff9-141"><a name="Filtering"> </a>Фильтрация</span><span class="sxs-lookup"><span data-stu-id="77ff9-141"><a name="Filtering"> </a>Filtering</span></span>
<span data-ttu-id="77ff9-142">Фильтрация обеспечивает более широкие и разнообразные способы контроля того, как записи должны отображаться в списке.</span><span class="sxs-lookup"><span data-stu-id="77ff9-142">Filtering provides a more advanced and versatile way of controlling which records display in a list.</span></span> <span data-ttu-id="77ff9-143">Имеется два основных отличия между поиском и фильтрацией, как описано в таблице ниже.</span><span class="sxs-lookup"><span data-stu-id="77ff9-143">There are two major differences between searching and filtering, as described in the table below.</span></span>

|| <span data-ttu-id="77ff9-144">**Поиск**</span><span class="sxs-lookup"><span data-stu-id="77ff9-144">**Searching**</span></span> | <span data-ttu-id="77ff9-145">**фильтрация;**</span><span class="sxs-lookup"><span data-stu-id="77ff9-145">**Filtering**</span></span> |
|--|----------|------------|
| <span data-ttu-id="77ff9-146">**Применимые поля**</span><span class="sxs-lookup"><span data-stu-id="77ff9-146">**Applicable fields**</span></span> | <span data-ttu-id="77ff9-147">Производится поиск по всем полям, видимым на странице.</span><span class="sxs-lookup"><span data-stu-id="77ff9-147">Searches across all fields that are visible on the page.</span></span> | <span data-ttu-id="77ff9-148">Фильтрует одно или несколько полей по отдельности, выбирая из любого поля в таблице, включая поля, которые не отображаются на странице.</span><span class="sxs-lookup"><span data-stu-id="77ff9-148">Filters one or more fields individually, selecting from any field on the table, including fields that are not visible on the page.</span></span> |
| <span data-ttu-id="77ff9-149">**Соответствие**</span><span class="sxs-lookup"><span data-stu-id="77ff9-149">**Matching**</span></span> | <span data-ttu-id="77ff9-150">Отображаются записи с полями, которые соответствуют тексту поиска, независимо от регистра или местоположения этого текста.</span><span class="sxs-lookup"><span data-stu-id="77ff9-150">Displays records with fields that match the search text, irrespective of casing or placement of that text.</span></span> | <span data-ttu-id="77ff9-151">Отображаются записи, в которых поле соответствует фильтру точно с учетом регистра, если не введены специальные символы фильтра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-151">Displays records where the field matches the filter exactly and is case sensitive, unless special filter symbols are entered.</span></span>

<span data-ttu-id="77ff9-152">Фильтрация позволяет отобразить записи для определенных организаций или клиентов, дат, сумм и иной информации путем определения критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-152">Filtering enables you to display records for specific accounts or customers, dates, amounts, and other information by specifying filter criteria.</span></span> <span data-ttu-id="77ff9-153">При этом отображаются только те записи, которые соответствуют заданным критериям.</span><span class="sxs-lookup"><span data-stu-id="77ff9-153">Only records that match the criteria are displayed.</span></span> <span data-ttu-id="77ff9-154">Если критерии заданы для нескольких полей, отображаются только записи, которые соответствуют этим критериям.</span><span class="sxs-lookup"><span data-stu-id="77ff9-154">If you specify criteria for multiple fields, then only records that match all criteria will be displayed.</span></span>

### <a name="working-in-the-filter-pane"></a><span data-ttu-id="77ff9-155">Работа в области фильтров</span><span class="sxs-lookup"><span data-stu-id="77ff9-155">Working in the Filter Pane</span></span>

<span data-ttu-id="77ff9-156">Для отображения области фильтров выберите ![Значок области фильтрации](media/open-filter-pane-icon.png "Значок области фильтрации") вверху списка или нажмите клавиши **Shift+F3**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-156">To display the filter pane, select ![Filter pane icon](media/open-filter-pane-icon.png "Filter pane icon") at the top of the list or press **Shift+F3**.</span></span> <span data-ttu-id="77ff9-157">Для списков в ролевом центре можно также выбрать стрелку вниз рядом с заголовком страницы в навигационной панели над списком, затем выбрать **Показать область фильтров**, как показано здесь:</span><span class="sxs-lookup"><span data-stu-id="77ff9-157">For lists within the Role Center, you can also choose the down arrow near the page title in the navigation bar above the list, and then choose **Show filter pane** as shown here:</span></span>

<span data-ttu-id="77ff9-158">![Показать область фильтров](media/open-filter-pane.png "Показать область фильтров")</span><span class="sxs-lookup"><span data-stu-id="77ff9-158">![Show filter pane](media/open-filter-pane.png "Show filter pane")</span></span>

<span data-ttu-id="77ff9-159">Область фильтров показывает текущие фильтры для списка и позволяет задать собственные настраиваемые фильтры для одного или нескольких полей.</span><span class="sxs-lookup"><span data-stu-id="77ff9-159">The filter pane displays the current filters for a list, and enables you to set your own custom filters on one or more fields.</span></span> <span data-ttu-id="77ff9-160">На приведенном ниже рисунке показан пример области фильтров для списка предложений по продаже.</span><span class="sxs-lookup"><span data-stu-id="77ff9-160">The following figure shows an example filter pane for a Sales Quotes list.</span></span>

<span data-ttu-id="77ff9-161">![Обзор области фильтров](media/filter-pane-overview.png "Значок фильтра")</span><span class="sxs-lookup"><span data-stu-id="77ff9-161">![Filter pane overview ](media/filter-pane-overview.png "Filter icon")</span></span>

<span data-ttu-id="77ff9-162">Область фильтров разделена на три раздела: **Представления**, **Фильтровать список по** и **Фильтровать итоги по**:</span><span class="sxs-lookup"><span data-stu-id="77ff9-162">A filter pane is divided in three sections: **Views**, **Filter list by**, and **Filter totals by**:</span></span>

- <span data-ttu-id="77ff9-163">**Представления**</span><span class="sxs-lookup"><span data-stu-id="77ff9-163">**Views**</span></span>

  <span data-ttu-id="77ff9-164">Некоторые списки включают раздел **Представления**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-164">Some lists will include the **Views** section.</span></span> <span data-ttu-id="77ff9-165">Представления являются вариациями списка, которые были заранее настроены с помощью фильтров.</span><span class="sxs-lookup"><span data-stu-id="77ff9-165">Views are variations of the list that have been preconfigured with filters.</span></span> <span data-ttu-id="77ff9-166">Чтобы перейти к другому представлению списка просто выберите другую ссылку.</span><span class="sxs-lookup"><span data-stu-id="77ff9-166">To switch to a different view of your list, simply select another link.</span></span> <span data-ttu-id="77ff9-167">Можно временно изменить фильтры в представлении, но изменения не будут сохраняться постоянно.</span><span class="sxs-lookup"><span data-stu-id="77ff9-167">You can temporarily change the filters on a view, but the changes will not be permanently saved.</span></span>

- <span data-ttu-id="77ff9-168">**Фильтровать список по**</span><span class="sxs-lookup"><span data-stu-id="77ff9-168">**Filter list by**</span></span>

  <span data-ttu-id="77ff9-169">В разделе **Фильтровать список по** можно добавлять фильтры по конкретным полям для сокращения числа отображаемых записей.</span><span class="sxs-lookup"><span data-stu-id="77ff9-169">The **Filter list by** section is where you add filters on specific fields to reduce the number of displayed records.</span></span> <span data-ttu-id="77ff9-170">Для добавления фильтра выберите **+ Фильтр**, выберите поле, которое необходимо фильтровать из любого поля в таблице, затем введите критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="77ff9-170">To add a filter, select **+ Filter**, select the field that you want to filter from any field in the table, and then enter filter criteria in the box.</span></span>

- <span data-ttu-id="77ff9-171">**Фильтровать итоги по**</span><span class="sxs-lookup"><span data-stu-id="77ff9-171">**Filter totals by**</span></span>

  <span data-ttu-id="77ff9-172">Некоторые списки, в которых отображаются вычисляемые поля, такие как суммы и количества, будут содержать раздел **Фильтровать итоги по** для изменения различных измерений, воздействующих на расчеты.</span><span class="sxs-lookup"><span data-stu-id="77ff9-172">Some lists that display calculated fields, such as amounts and quantities, will include the **Filter totals by** section where you can adjust various dimensions that influence calculations.</span></span> <span data-ttu-id="77ff9-173">Например, можно быстро анализировать план счетов, фильтруя суммы за определенный период, или можно просмотреть итоги только для заказов на продажу с определенного склада.</span><span class="sxs-lookup"><span data-stu-id="77ff9-173">For example, you can quickly analyze your chart of accounts by filtering amounts to a specific period, or you can view the totals for sales orders only from a specific warehouse.</span></span>

  <span data-ttu-id="77ff9-174">Для добавления фильтра выберите **+ Фильтр**, выберите одно из предопределенных измерений, затем добавьте критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="77ff9-174">To add a filter, select **+ Filter**, select one of the predefined dimensions, and then add the filter criteria in the box.</span></span>

  > [!NOTE]
  > <span data-ttu-id="77ff9-175">Фильтры в разделе **Фильтровать итоги по** управляются элементами FlowFilter в дизайне страницы.</span><span class="sxs-lookup"><span data-stu-id="77ff9-175">Filters in the **Filter totals by** section are controlled by FlowFilters on the page design.</span></span> <span data-ttu-id="77ff9-176">Технические сведения см. в разделе [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span><span class="sxs-lookup"><span data-stu-id="77ff9-176">For technical information, see [FlowFilters](https://docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/developer/devenv-flowfilter-overview).</span></span>


### <a name="entering-filter-criteria-in-the-filter-pane"></a><span data-ttu-id="77ff9-177">Ввод критериев фильтра в области фильтров</span><span class="sxs-lookup"><span data-stu-id="77ff9-177">Entering Filter Criteria in the Filter Pane</span></span>
<span data-ttu-id="77ff9-178">Чтобы выбрать поле для фильтра, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="77ff9-178">To select a field to filter, do one of the following:</span></span>
  - <span data-ttu-id="77ff9-179">В области фильтров выберите **+ Поле**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-179">In the filter pane, choose **+ Field**.</span></span> <span data-ttu-id="77ff9-180">Введите название поля, которое необходимо фильтровать, или выберите поле в меню, в котором отображаются все поля в таблице.</span><span class="sxs-lookup"><span data-stu-id="77ff9-180">Type the name of the field you wish to filter, or pick a field from the menu that displays all fields in the table.</span></span>

  - <span data-ttu-id="77ff9-181">Выберите в заголовке столбца стрелку вниз, затем выберите **Фильтр...**. Это приведет к открытию область фильтров и добавит столбец в область фильтров.</span><span class="sxs-lookup"><span data-stu-id="77ff9-181">In a column heading, choose the down arrow, and then choose **Filter...**. This will open the filter pane and add the column to the filter pane.</span></span>

<span data-ttu-id="77ff9-182">Теперь можно ввести или выбрать критерии фильтра в поле.</span><span class="sxs-lookup"><span data-stu-id="77ff9-182">You can now type or select your filter criteria in the box.</span></span> <span data-ttu-id="77ff9-183">Тип фильтруемого поля определяет, какие критерии можно ввести.</span><span class="sxs-lookup"><span data-stu-id="77ff9-183">The type of field you filter determines which criteria you can enter.</span></span> <span data-ttu-id="77ff9-184">Например, при фильтрации поля, которое имеет фиксированные значения, можно выбирать только из этих значений.</span><span class="sxs-lookup"><span data-stu-id="77ff9-184">For example, filtering a field that has fixed values will only let you choose from those values.</span></span> <span data-ttu-id="77ff9-185">Дополнительные сведения об особенных знаках фильтров см. в разделах [Критерии фильтра](#FilterCriteria) и [Токены фильтра](#FilterTokens).</span><span class="sxs-lookup"><span data-stu-id="77ff9-185">For more information about special filter symbols, see [Filter criteria](#FilterCriteria) and [Filter tokens](#FilterTokens).</span></span>

<span data-ttu-id="77ff9-186">Столбцы, которые уже содержат фильтры, обозначаются ![Значок фильтра](media/ui-search/filter-icon.png "Значок фильтра") в заголовке столбцов.</span><span class="sxs-lookup"><span data-stu-id="77ff9-186">Columns that already have filters are indicated by the ![Filter icon](media/ui-search/filter-icon.png "Filter icon") in the column heading.</span></span> <span data-ttu-id="77ff9-187">Чтобы снять фильтр, выберите заголовок столбца и выберите **Очистить фильтр**.</span><span class="sxs-lookup"><span data-stu-id="77ff9-187">To remove a filter, select the column heading, then choose **Clear Filter**.</span></span>


### <a name="entering-filter-criteria-without-using-the-filter-pane"></a><span data-ttu-id="77ff9-188">Ввод критериев фильтра без использования области фильтров</span><span class="sxs-lookup"><span data-stu-id="77ff9-188">Entering Filter Criteria Without Using the Filter Pane</span></span>
<span data-ttu-id="77ff9-189">Можно определить простые фильтры непосредственно в списке без использования области фильтров.</span><span class="sxs-lookup"><span data-stu-id="77ff9-189">You can specify simple filters directly within the list without having to use the filter pane.</span></span>
<span data-ttu-id="77ff9-190">С любым полем, выбранным в строке, используйте сочетание клавиш **Alt+F3** для отображения только записей, имеющих это же значение.</span><span class="sxs-lookup"><span data-stu-id="77ff9-190">With any field selected on a row, use the **Alt+F3** keyboard shortcut to display only the records having that same value.</span></span> <span data-ttu-id="77ff9-191">Затем можно выбрать другое поле и снова использовать это же сочетание клавиш, чтобы продолжить уточнять фильтры.</span><span class="sxs-lookup"><span data-stu-id="77ff9-191">You can then select another field and use the same shortcut again to continue refining your filters.</span></span> <span data-ttu-id="77ff9-192">Если выбрано поле уже содержит фильтр, при использовании **Alt+F3** этот фильтр очищается.</span><span class="sxs-lookup"><span data-stu-id="77ff9-192">If the selected field is already filtered, using **Alt+F3** will clear that filter.</span></span>

> [!TIP]
> <span data-ttu-id="77ff9-193">Ускорьте поиск и анализ данных с помощью сочетаний клавиш.</span><span class="sxs-lookup"><span data-stu-id="77ff9-193">Accelerate finding and analyzing your data by using combinations of keyboard shortcuts.</span></span> <span data-ttu-id="77ff9-194">Например, выберите поле, используйте **Shift+Alt+F3** для добавления этого поля к области фильтров, введите критерии фильтра, используйте **Ctrl+Enter** для возврата в строки, выберите другое поле, используйте **Alt+F3** для фильтрации по этому значению.</span><span class="sxs-lookup"><span data-stu-id="77ff9-194">For example, select a field, use **Shift+Alt+F3** to add that field to the filter pane, type the filter criteria, use **Ctrl+Enter** to return to the rows, select another field, and use **Alt+F3** to filter to that value.</span></span>
<span data-ttu-id="77ff9-195">Дополнительные сведения см. в разделе [Сочетания клавиш](keyboard-shortcuts.md#KeyboardFilter).</span><span class="sxs-lookup"><span data-stu-id="77ff9-195">For more information see [Keyboard Shortcuts](keyboard-shortcuts.md#KeyboardFilter).</span></span>


## <span data-ttu-id="77ff9-196"><a name="FilterCriteria"> </a>Критерии фильтра и символы</span><span class="sxs-lookup"><span data-stu-id="77ff9-196"><a name="FilterCriteria"> </a>Filter Criteria and Symbols</span></span>
<span data-ttu-id="77ff9-197">В процессе установки критериев фильтра можно использовать все цифры и буквы, которые обычно вводятся в поле.</span><span class="sxs-lookup"><span data-stu-id="77ff9-197">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="77ff9-198">Кроме того, для дополнительной фильтрации результатов можно использовать специальные символы (или операторы).</span><span class="sxs-lookup"><span data-stu-id="77ff9-198">In addition, you can use special symbols (or operators) to further filter the results.</span></span> <span data-ttu-id="77ff9-199">В следующих таблицах приведены символы, которые могут быть использованы в фильтрах.</span><span class="sxs-lookup"><span data-stu-id="77ff9-199">The following tables show the symbols which can be used in filters.</span></span> <span data-ttu-id="77ff9-200">Для дат и времени также можно получить более подробную информацию в разделе [Работа с датами и временем в календаре](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="77ff9-200">For dates and times, you can also refer to [Working with Calendar Dates and Times](ui-enter-date-ranges.md) for more detailed information.</span></span>

> [!IMPORTANT]  
>  <span data-ttu-id="77ff9-201">Могут быть ситуации, когда значения поля содержит эти символы, и требуется фильтрация по ним.</span><span class="sxs-lookup"><span data-stu-id="77ff9-201">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="77ff9-202">Чтобы это сделать, необходимо включить выражение фильтра, которое содержит данный символ в кавычках (").</span><span class="sxs-lookup"><span data-stu-id="77ff9-202">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="77ff9-203">Например, если необходимо фильтровать записи, которые начинаются с текста *S&R*, выражение фильтра имеет вид `'S&R*'`.</span><span class="sxs-lookup"><span data-stu-id="77ff9-203">For example, if you want to filter on records that start with the text *S&R*, the filter expression is `'S&R*'`.</span></span>

<span data-ttu-id="77ff9-204">В следующих разделах описано, как использовать различные операторы.</span><span class="sxs-lookup"><span data-stu-id="77ff9-204">The following sections describe how to use the different operators.</span></span>

> [!NOTE]
> <span data-ttu-id="77ff9-205">Если в одном фильтре более 200 операторов, система автоматически сгруппирует некоторые выражения в скобки `()` с целью обработки.</span><span class="sxs-lookup"><span data-stu-id="77ff9-205">If there are more than 200 operators in a single filter, the system will automatically group some expressions in parentheses `()` for the purpose of processing.</span></span> <span data-ttu-id="77ff9-206">Это не влияет на фильтр или результаты.</span><span class="sxs-lookup"><span data-stu-id="77ff9-206">This has no effect on the filter or the results.</span></span>  

### <a name="-interval"></a><span data-ttu-id="77ff9-207">(..) Диапазон</span><span class="sxs-lookup"><span data-stu-id="77ff9-207">(..) Interval</span></span>

|<span data-ttu-id="77ff9-208">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-208">Sample Expression</span></span>|<span data-ttu-id="77ff9-209">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-209">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1100..2100`|<span data-ttu-id="77ff9-210">Номера от 1 100 до 2 100</span><span class="sxs-lookup"><span data-stu-id="77ff9-210">Numbers 1100 through 2100</span></span>|  
|`..2500`|<span data-ttu-id="77ff9-211">До 2500, включительно</span><span class="sxs-lookup"><span data-stu-id="77ff9-211">Up to and including 2500</span></span>|  
|`..12 31 00`|<span data-ttu-id="77ff9-212">Даты по 31.12.00 включительно</span><span class="sxs-lookup"><span data-stu-id="77ff9-212">Dates up to and including 12 31 00</span></span>|  
|`P8..`|<span data-ttu-id="77ff9-213">Информация для 8-го учетного периода и позже.</span><span class="sxs-lookup"><span data-stu-id="77ff9-213">Information for accounting period 8 and thereafter</span></span>|  
|`..23`|<span data-ttu-id="77ff9-214">С даты начала по 23 число текущего месяца текущего года до 23:59:59</span><span class="sxs-lookup"><span data-stu-id="77ff9-214">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|`23..`|<span data-ttu-id="77ff9-215">с 23 текущего месяца текущего года 00:00:00 до конца</span><span class="sxs-lookup"><span data-stu-id="77ff9-215">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|`22..23`|<span data-ttu-id="77ff9-216">с 22 текущего месяца текущего года 0:00:00 по 23 текущего месяца текущего года 23:59:59</span><span class="sxs-lookup"><span data-stu-id="77ff9-216">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  

### <a name="124-eitheror"></a><span data-ttu-id="77ff9-217">(&#124;) Или/или</span><span class="sxs-lookup"><span data-stu-id="77ff9-217">(&#124;) Either/or</span></span> 

|<span data-ttu-id="77ff9-218">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-218">Sample Expression</span></span>|<span data-ttu-id="77ff9-219">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-219">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`1200|1300`|<span data-ttu-id="77ff9-220">Номера со значением 1 200 или 1 300</span><span class="sxs-lookup"><span data-stu-id="77ff9-220">Numbers with 1200 or 1300</span></span>|  

### <a name="-not-equal-to"></a><span data-ttu-id="77ff9-221">(<>) Не равно</span><span class="sxs-lookup"><span data-stu-id="77ff9-221">(<>) Not equal to</span></span>  

|<span data-ttu-id="77ff9-222">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-222">Sample Expression</span></span>|<span data-ttu-id="77ff9-223">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-223">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<>0`|<span data-ttu-id="77ff9-224">Все числа, кроме 0</span><span class="sxs-lookup"><span data-stu-id="77ff9-224">All numbers except 0</span></span><br /><br /> <span data-ttu-id="77ff9-225">Возможность использования Microsoft SQL Server позволяет комбинировать данный символ со знаками подстановки.</span><span class="sxs-lookup"><span data-stu-id="77ff9-225">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="77ff9-226">Например, <>A\* означает несоответствие любым текстам, начинающимся с А.</span><span class="sxs-lookup"><span data-stu-id="77ff9-226">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  

### <a name="-greater-than"></a><span data-ttu-id="77ff9-227">(>) Больше чем</span><span class="sxs-lookup"><span data-stu-id="77ff9-227">(>) Greater than</span></span>  

|<span data-ttu-id="77ff9-228">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-228">Sample Expression</span></span>|<span data-ttu-id="77ff9-229">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-229">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>1200`|<span data-ttu-id="77ff9-230">Числа больше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="77ff9-230">Numbers greater than 1200</span></span>|  

### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="77ff9-231">(>=) Больше чем или равно</span><span class="sxs-lookup"><span data-stu-id="77ff9-231">(>=) Greater than or equal to</span></span>  

|<span data-ttu-id="77ff9-232">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-232">Sample Expression</span></span>|<span data-ttu-id="77ff9-233">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-233">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>=1200`|<span data-ttu-id="77ff9-234">Номера больше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="77ff9-234">Numbers greater than or equal to 1200</span></span>|  

### <a name="-less-than"></a><span data-ttu-id="77ff9-235">(<) Меньше чем</span><span class="sxs-lookup"><span data-stu-id="77ff9-235">(<) Less than</span></span>  

|<span data-ttu-id="77ff9-236">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-236">Sample Expression</span></span>|<span data-ttu-id="77ff9-237">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-237">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<1200`|<span data-ttu-id="77ff9-238">Номера меньше, чем 1 200</span><span class="sxs-lookup"><span data-stu-id="77ff9-238">Numbers less than 1200</span></span>|  

### <a name="-less-than-or-equal-to"></a><span data-ttu-id="77ff9-239">(<=) Меньше или равно</span><span class="sxs-lookup"><span data-stu-id="77ff9-239">(<=) Less than or equal to</span></span>  

|<span data-ttu-id="77ff9-240">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-240">Sample Expression</span></span>|<span data-ttu-id="77ff9-241">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-241">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`<=1200`|<span data-ttu-id="77ff9-242">Номера меньше или равны 1 200</span><span class="sxs-lookup"><span data-stu-id="77ff9-242">Numbers less than or equal to 1200</span></span>|  

### <a name="-and"></a><span data-ttu-id="77ff9-243">(&) И</span><span class="sxs-lookup"><span data-stu-id="77ff9-243">(&) And</span></span>  

|<span data-ttu-id="77ff9-244">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-244">Sample Expression</span></span>|<span data-ttu-id="77ff9-245">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-245">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`>200&<1200`|<span data-ttu-id="77ff9-246">Числа больше 200 и меньше 1200</span><span class="sxs-lookup"><span data-stu-id="77ff9-246">Numbers greater than 200 and less than 1200</span></span>|  

### <a name="-an-exact-character-match"></a><span data-ttu-id="77ff9-247">('') Точное совпадение символа</span><span class="sxs-lookup"><span data-stu-id="77ff9-247">('') An exact character match</span></span>  

|<span data-ttu-id="77ff9-248">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-248">Sample Expression</span></span>|<span data-ttu-id="77ff9-249">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-249">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`'man'`|<span data-ttu-id="77ff9-250">Текст, точно соответствующий man с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-250">Text that matches man exactly and is case sensitive.</span></span>|  

### <a name="-case-insensitive"></a><span data-ttu-id="77ff9-251">(@) Без учета регистра</span><span class="sxs-lookup"><span data-stu-id="77ff9-251">(@) Case insensitive</span></span>  

|<span data-ttu-id="77ff9-252">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-252">Sample Expression</span></span>|<span data-ttu-id="77ff9-253">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-253">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`@man*`|<span data-ttu-id="77ff9-254">Текст, начинающийся с man без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-254">Text that starts with man and is case insensitive.</span></span>|  

### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="77ff9-255">(\*) Неопределенное количество неизвестных символов</span><span class="sxs-lookup"><span data-stu-id="77ff9-255">(\*) An indefinite number of unknown characters</span></span>

|<span data-ttu-id="77ff9-256">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-256">Sample Expression</span></span>|<span data-ttu-id="77ff9-257">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-257">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`*Co*`|<span data-ttu-id="77ff9-258">Текст, который содержит "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-258">Text that contains "Co" and is case sensitive.</span></span>|  
|`*Co`|<span data-ttu-id="77ff9-259">Текст, который заканчивается на "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-259">Text that ends with "Co" and is case sensitive.</span></span>|  
|`Co*`|<span data-ttu-id="77ff9-260">Текст, который начинается с "Ко" с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-260">Text that begins with "Co" and is case sensitive.</span></span>|  

> [!NOTE]  
>   <span data-ttu-id="77ff9-261">Нельзя использовать `*` при фильтрации в полях параметров (перечислений), например в поле **Статус** заказов на продажу.</span><span class="sxs-lookup"><span data-stu-id="77ff9-261">You cannot use `*` when filtering on option (enumeration) fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="77ff9-262">Чтобы ввести фильтр для данного типа поля, можно ввести в качестве параметра фильтра числовое значение.</span><span class="sxs-lookup"><span data-stu-id="77ff9-262">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="77ff9-263">Например, в поле **Статус** в заказе на продажу, которое имеет значения **Открыть**, **Выпущено**, **Ожидает утверждения** и **Ожидает предоплаты**, используйте значения `0`, `1`, `2` и `3` для фильтрации этих параметров.</span><span class="sxs-lookup"><span data-stu-id="77ff9-263">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values `0`, `1`, `2`, and `3` to filter for these options.</span></span>

### <a name="-one-unknown-character"></a><span data-ttu-id="77ff9-264">(?) Один неизвестный символ</span><span class="sxs-lookup"><span data-stu-id="77ff9-264">(?) One unknown character</span></span>  

|<span data-ttu-id="77ff9-265">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-265">Sample Expression</span></span>|<span data-ttu-id="77ff9-266">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-266">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`Hans?n`|<span data-ttu-id="77ff9-267">Такой текст, как «Стул» или «Стол»</span><span class="sxs-lookup"><span data-stu-id="77ff9-267">Text such as Hansen or Hanson</span></span>|  

### <a name="combined-format-expressions"></a><span data-ttu-id="77ff9-268">Объединенные выражения форматов</span><span class="sxs-lookup"><span data-stu-id="77ff9-268">Combined Format Expressions</span></span>  

|<span data-ttu-id="77ff9-269">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-269">Sample Expression</span></span>|<span data-ttu-id="77ff9-270">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-270">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`5999|8100..8490`|<span data-ttu-id="77ff9-271">Включает все записи с номером 5999 или номерами от 8100 до 8490.</span><span class="sxs-lookup"><span data-stu-id="77ff9-271">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|`..1299|1400..`|<span data-ttu-id="77ff9-272">Все записи с номером меньше или равно 1299 или номером от 1400 или больше (все номера, кроме от 1300 до 1399).</span><span class="sxs-lookup"><span data-stu-id="77ff9-272">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|`>50&<100`|<span data-ttu-id="77ff9-273">Все записи с номерами больше 50 и меньше 100 (номера от 51 до 99).</span><span class="sxs-lookup"><span data-stu-id="77ff9-273">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  


## <span data-ttu-id="77ff9-274"><a name="FilterTokens"> </a>Токены фильтра</span><span class="sxs-lookup"><span data-stu-id="77ff9-274"><a name="FilterTokens"> </a>Filter Tokens</span></span>
<span data-ttu-id="77ff9-275">При указании критериев фильтра можно также вводить слова, которые имеют специальное значение, называемые токенами фильтра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-275">When entering filter criteria, you can also type words that have special meaning, called filter tokens.</span></span> <span data-ttu-id="77ff9-276">После ввода слова токена это слово заменяется значением или значениями, которые оно представляет.</span><span class="sxs-lookup"><span data-stu-id="77ff9-276">After entering the token word, the word is replaced by the value or values that it represents.</span></span> <span data-ttu-id="77ff9-277">Это упрощает фильтрацию благодаря снижению потребности перехода между страницами для поиска значений, которые требуется добавить в фильтр.</span><span class="sxs-lookup"><span data-stu-id="77ff9-277">This makes filtering easier by reducing the need to navigate to other pages to look up values you want to add to your filter.</span></span> <span data-ttu-id="77ff9-278">В таблицах ниже описаны некоторые из токенов, которые можно вводить в качестве критериев фильтра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-278">The tables below describe some of the tokens you can type as filter criteria.</span></span>

> [!TIP]
> <span data-ttu-id="77ff9-279">Ваша организация может использовать настраиваемые токены.</span><span class="sxs-lookup"><span data-stu-id="77ff9-279">Your organization may use custom tokens.</span></span> <span data-ttu-id="77ff9-280">Для получения полного набора токенов, доступных вам, или для добавления дополнительных настраиваемых токенов обращайтесь к администратору.</span><span class="sxs-lookup"><span data-stu-id="77ff9-280">To learn about the complete set of tokens available to you or to add more custom tokens, talk to your administrator.</span></span> <span data-ttu-id="77ff9-281">Технические сведения см. в разделе [Добавление токенов фильтров](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span><span class="sxs-lookup"><span data-stu-id="77ff9-281">For technical information see [Adding Filter Tokens](/dynamics365/business-central/dev-itpro/developer/devenv-adding-filter-tokens).</span></span>


### <a name="me-or-userid-records-assigned-to-you"></a><span data-ttu-id="77ff9-282">(%me или %userid) Записи, назначенные вам</span><span class="sxs-lookup"><span data-stu-id="77ff9-282">(%me or %userid) Records Assigned to You</span></span>

<span data-ttu-id="77ff9-283">Используйте `%me` или `%userid` с поля фильтра, которые содержат код пользователя, например поле **Назначено коду пользователя** для отображения всех записей, которые назначены вам.</span><span class="sxs-lookup"><span data-stu-id="77ff9-283">Use `%me` or `%userid` when filtering fields that contain the user ID, such as **Assigned to User ID** field, to display all records that are assigned to you.</span></span>

|<span data-ttu-id="77ff9-284">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-284">Sample Expression</span></span>|<span data-ttu-id="77ff9-285">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-285">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%me`<br /><span data-ttu-id="77ff9-286">или</span><span class="sxs-lookup"><span data-stu-id="77ff9-286">or</span></span><br />`%userid`|<span data-ttu-id="77ff9-287">Записи, которые назначены вашей учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="77ff9-287">Records that are assigned to your user account.</span></span> |  

### <a name="mycustomers-customers-in-my-customers"></a><span data-ttu-id="77ff9-288">(%mycustomers) Клиенты в "Мои клиенты"</span><span class="sxs-lookup"><span data-stu-id="77ff9-288">(%mycustomers) Customers in My Customers</span></span>

<span data-ttu-id="77ff9-289">Используйте `%mycustomers` в поле **№** клиента для отображения всех записей для клиентов, которые входят в список **Мои клиенты** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="77ff9-289">Use `%mycustomers` in the customer **No** field to display all records for customers that are included in the **My Customers** list on your Role Center.</span></span>

|<span data-ttu-id="77ff9-290">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-290">Sample Expression</span></span>|<span data-ttu-id="77ff9-291">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-291">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%mycustomers`|<span data-ttu-id="77ff9-292">Клиенты в списке **Мои клиенты** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-292">Customers in the **My Customers** on your Role Center.</span></span> |  

### <a name="myitems-items-in-my-items"></a><span data-ttu-id="77ff9-293">(%myitems) Товары в списке "Мои товары"</span><span class="sxs-lookup"><span data-stu-id="77ff9-293">(%myitems) Items in My Items</span></span>

<span data-ttu-id="77ff9-294">Используйте `%myitems` в поле **№** товара для отображения всех записей для товаров, которые входят в список **Мои товары** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="77ff9-294">Use `%myitems` in the item **No** field to display all records for items that are included in the **My Items** list on your Role Center.</span></span>

|<span data-ttu-id="77ff9-295">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-295">Sample Expression</span></span>|<span data-ttu-id="77ff9-296">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-296">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myitems`|<span data-ttu-id="77ff9-297">Товары в списке **Мои товары** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-297">Items in the **My Items** on your Role Center.</span></span> |  

### <a name="myvendors-vendors-in-my-vendors"></a><span data-ttu-id="77ff9-298">(%myvendors) Поставщики в списке "Мои поставщики"</span><span class="sxs-lookup"><span data-stu-id="77ff9-298">(%myvendors) Vendors in My Vendors</span></span>

<span data-ttu-id="77ff9-299">Используйте `%myvendors` в поле **№** поставщика для отображения всех записей для поставщиков, которые входят в список **Мои поставщики** в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="77ff9-299">Use `%myvendors` in the vendor **No** field to display all records for vendors that are included in the **My Vendors** list on your Role Center.</span></span>

|<span data-ttu-id="77ff9-300">Образец выражения</span><span class="sxs-lookup"><span data-stu-id="77ff9-300">Sample Expression</span></span>|<span data-ttu-id="77ff9-301">Отображаемые записи</span><span class="sxs-lookup"><span data-stu-id="77ff9-301">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|`%myvendors`|<span data-ttu-id="77ff9-302">Поставщики в списке **Мои поставщики** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="77ff9-302">Vendors in the **My Vendors** on your Role Center.</span></span> |  


## <a name="see-also"></a><span data-ttu-id="77ff9-303">См. также</span><span class="sxs-lookup"><span data-stu-id="77ff9-303">See Also</span></span>
<span data-ttu-id="77ff9-304">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="77ff9-304">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="77ff9-305">Общие вопросы и поиске и фильтрации</span><span class="sxs-lookup"><span data-stu-id="77ff9-305">Common questions about Searching and Filtering</span></span>](ui-search-filter-faq.md)
