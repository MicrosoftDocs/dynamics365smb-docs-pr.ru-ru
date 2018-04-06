---
title: "Настройка диапазонов дат в Finance and Operations, Business edition | Microsoft Docs"
description: "Узнайте о том, как получить отчет с данными за определенные интервалы времени, используя для этого диапазоны дат в Finance and Operations, Business edition."
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
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0494a04e67803049df71cfefe779c831c9f31674
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="entering-date-ranges"></a><span data-ttu-id="1d895-103">Ввод диапазонов дат</span><span class="sxs-lookup"><span data-stu-id="1d895-103">Entering Date Ranges</span></span> 
<span data-ttu-id="1d895-104">Чтобы на экране отображались только данные за определенный диапазон дат или промежуток времени, можно задать фильтры с указанием даты начала и даты завершения.</span><span class="sxs-lookup"><span data-stu-id="1d895-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="1d895-105">При установке диапазонов дат следует руководствоваться определенными правилами.</span><span class="sxs-lookup"><span data-stu-id="1d895-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="1d895-106">Рассмотрим пример **Клиент - первая десятка**:</span><span class="sxs-lookup"><span data-stu-id="1d895-106">Let's take the **Customer Top 10** as an example:</span></span>

![Установка диапазона дат на странице запросов для списка "Клиент - первая десятка"](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="1d895-108">Здесь можно ограничить отчет по диапазону дат, например прошлыми двумя неделями или всего 6 неделями, либо любым другим диапазоном.</span><span class="sxs-lookup"><span data-stu-id="1d895-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="1d895-109">Для задания диапазонов дат необходимо указать даты и использовать **..**</span><span class="sxs-lookup"><span data-stu-id="1d895-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="1d895-110">или **|**, чтобы обозначить диапазон.</span><span class="sxs-lookup"><span data-stu-id="1d895-110">or **|** to set the range.</span></span> <span data-ttu-id="1d895-111">В нашем примере для отображения десятки клиентов за первые две недели мая необходимо задать фильтра по дате *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="1d895-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="1d895-112">Вот еще несколько примеров:</span><span class="sxs-lookup"><span data-stu-id="1d895-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="1d895-113">Значение</span><span class="sxs-lookup"><span data-stu-id="1d895-113">Meaning</span></span> | <span data-ttu-id="1d895-114">Пример</span><span class="sxs-lookup"><span data-stu-id="1d895-114">Example</span></span> | <span data-ttu-id="1d895-115">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="1d895-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="1d895-116">Равный</span><span class="sxs-lookup"><span data-stu-id="1d895-116">Equal to</span></span>| <span data-ttu-id="1d895-117">15 12 16</span><span class="sxs-lookup"><span data-stu-id="1d895-117">12 15 16</span></span> |<span data-ttu-id="1d895-118">Только учтенные на 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="1d895-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="1d895-119">Интервал</span><span class="sxs-lookup"><span data-stu-id="1d895-119">Interval</span></span>| <span data-ttu-id="1d895-120">15 12 16..15 17 17</span><span class="sxs-lookup"><span data-stu-id="1d895-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="1d895-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="1d895-121">..12 15 16</span></span>|<span data-ttu-id="1d895-122">Учтенные в даты между 15 декабря 2016 и 15 января 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="1d895-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="1d895-123">Учтенные не позднее 15 декабря 2106 года</span><span class="sxs-lookup"><span data-stu-id="1d895-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="1d895-124">Либо/или</span><span class="sxs-lookup"><span data-stu-id="1d895-124">Either/or</span></span>|<span data-ttu-id="1d895-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="1d895-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="1d895-126">Учтенные 15 декабря или 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="1d895-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="1d895-127">При наличии операций, учтенных на обе даты, отображаются все эти операции.</span><span class="sxs-lookup"><span data-stu-id="1d895-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="1d895-128">Также можно объединять разные типы форматов.</span><span class="sxs-lookup"><span data-stu-id="1d895-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="1d895-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1d895-129">Example</span></span> | <span data-ttu-id="1d895-130">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="1d895-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="1d895-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="1d895-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="1d895-132">Операции, учтенные 15 декабря 2016 или в даты между 01 декабря 2016 и 31 мая 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="1d895-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="1d895-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="1d895-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="1d895-134">Операции, учтенные не позднее 14 декабря, или операции, учтенные не раньше 30 декабря, т. е. все операции, кроме учтенных между 15 и 29 декабря (включительно).</span><span class="sxs-lookup"><span data-stu-id="1d895-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="1d895-135">Обратите внимание, что здесь использован американский формат дат ММДДГГ.</span><span class="sxs-lookup"><span data-stu-id="1d895-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="1d895-136">Когда [!INCLUDE[d365fin](includes/d365fin_md.md)] появится на других рынках, вы сможете использовать те форматы, к которым вы привыкли.</span><span class="sxs-lookup"><span data-stu-id="1d895-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="see-also"></a><span data-ttu-id="1d895-137">См. также</span><span class="sxs-lookup"><span data-stu-id="1d895-137">See Also</span></span>
<span data-ttu-id="1d895-138">[Работа с [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1d895-138">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="1d895-139">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="1d895-139">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="1d895-140">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="1d895-140">General Business Functionality</span></span>](ui-across-business-areas.md)

