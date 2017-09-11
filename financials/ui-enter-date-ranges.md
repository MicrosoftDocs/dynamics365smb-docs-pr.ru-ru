---
title: "Настройка диапазонов дат в Dynamics 365 for Financials | Документы Майкрософт"
description: "Узнайте о том, как получить отчет с данными за определенные интервалы времени, используя для этого диапазоны дат в Dynamics 365 for Financials."
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 05/29/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: dc7cd392843ce7c39200bb2331c09cc44c7a394a
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="entering-date-ranges-in-dynamics-365-for-financials"></a><span data-ttu-id="ef9d1-103">Ввод диапазонов дат в Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="ef9d1-103">Entering Date Ranges in Dynamics 365 for Financials</span></span>
<span data-ttu-id="ef9d1-104">Чтобы на экране отображались только данные за определенный диапазон дат или промежуток времени, можно задать фильтры с указанием даты начала и даты завершения.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="ef9d1-105">При установке диапазонов дат следует руководствоваться определенными правилами.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="ef9d1-106">Рассмотрим пример **Клиент - первая десятка**:</span><span class="sxs-lookup"><span data-stu-id="ef9d1-106">Let's take the **Customer Top 10** as an example:</span></span>

![Установка диапазона дат на странице запросов для списка "Клиент - первая десятка"](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="ef9d1-108">Здесь можно ограничить отчет по диапазону дат, например прошлыми двумя неделями или всего 6 неделями, либо любым другим диапазоном.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="ef9d1-109">Для задания диапазонов дат необходимо указать даты и использовать **..**</span><span class="sxs-lookup"><span data-stu-id="ef9d1-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="ef9d1-110">или **|**, чтобы обозначить диапазон.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-110">or **|** to set the range.</span></span> <span data-ttu-id="ef9d1-111">В нашем примере для отображения десятки клиентов за первые две недели мая необходимо задать фильтра по дате *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="ef9d1-112">Вот еще несколько примеров:</span><span class="sxs-lookup"><span data-stu-id="ef9d1-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="ef9d1-113">Значение</span><span class="sxs-lookup"><span data-stu-id="ef9d1-113">Meaning</span></span> | <span data-ttu-id="ef9d1-114">Пример</span><span class="sxs-lookup"><span data-stu-id="ef9d1-114">Example</span></span> | <span data-ttu-id="ef9d1-115">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="ef9d1-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="ef9d1-116">Равный</span><span class="sxs-lookup"><span data-stu-id="ef9d1-116">Equal to</span></span>| <span data-ttu-id="ef9d1-117">15 12 16</span><span class="sxs-lookup"><span data-stu-id="ef9d1-117">12 15 16</span></span> |<span data-ttu-id="ef9d1-118">Только учтенные на 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="ef9d1-119">Интервал</span><span class="sxs-lookup"><span data-stu-id="ef9d1-119">Interval</span></span>| <span data-ttu-id="ef9d1-120">15 12 16..15 17 17</span><span class="sxs-lookup"><span data-stu-id="ef9d1-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="ef9d1-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="ef9d1-121">..12 15 16</span></span>|<span data-ttu-id="ef9d1-122">Учтенные в даты между 15 декабря 2016 и 15 января 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="ef9d1-123">Учтенные не позднее 15 декабря 2106 года</span><span class="sxs-lookup"><span data-stu-id="ef9d1-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="ef9d1-124">Либо/или</span><span class="sxs-lookup"><span data-stu-id="ef9d1-124">Either/or</span></span>|<span data-ttu-id="ef9d1-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="ef9d1-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="ef9d1-126">Учтенные 15 декабря или 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="ef9d1-127">При наличии операций, учтенных на обе даты, отображаются все эти операции.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="ef9d1-128">Также можно объединять разные типы форматов.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="ef9d1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ef9d1-129">Example</span></span> | <span data-ttu-id="ef9d1-130">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="ef9d1-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="ef9d1-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="ef9d1-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="ef9d1-132">Операции, учтенные 15 декабря 2016 или в даты между 01 декабря 2016 и 31 мая 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="ef9d1-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="ef9d1-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="ef9d1-134">Операции, учтенные не позднее 14 декабря, или операции, учтенные не раньше 30 декабря, т. е. все операции, кроме учтенных между 15 и 29 декабря (включительно).</span><span class="sxs-lookup"><span data-stu-id="ef9d1-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="ef9d1-135">Обратите внимание, что здесь использован американский формат дат ММДДГГ.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="ef9d1-136">Когда [!INCLUDE[d365fin](includes/d365fin_md.md)] появится на других рынках, вы сможете использовать те форматы, к которым вы привыкли.</span><span class="sxs-lookup"><span data-stu-id="ef9d1-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="ef9d1-137">См. также</span><span class="sxs-lookup"><span data-stu-id="ef9d1-137">See Also</span></span>
<span data-ttu-id="ef9d1-138">[Работа с [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ef9d1-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="ef9d1-139">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="ef9d1-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="ef9d1-140">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="ef9d1-140">General Business Functionality</span></span>](ui-across-business-areas.md)

