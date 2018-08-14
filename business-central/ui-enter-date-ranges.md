---
title: "Установка диапазонов дат в Business Central | Документы Майкрософт"
description: "Узнайте о том, как получить отчет с данными за определенные интервалы времени, используя для этого диапазоны дат в Business Central."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter
ms.date: 07/05/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7664360941313da6ea0b797ef00df2e9810ad62
ms.openlocfilehash: ff63ae71a78f956dddb7b5247ee66f9416cf7cf1
ms.contentlocale: ru-ru
ms.lasthandoff: 07/09/2018

---
# <a name="entering-date-ranges"></a><span data-ttu-id="1a3ac-103">Ввод диапазонов дат</span><span class="sxs-lookup"><span data-stu-id="1a3ac-103">Entering Date Ranges</span></span>
<span data-ttu-id="1a3ac-104">Чтобы на экране отображались только данные за определенный диапазон дат или промежуток времени, можно задать фильтры с указанием даты начала и даты завершения.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-104">You can set filters containing a start date and an end date to display only the data contained in that date range or time interval.</span></span> <span data-ttu-id="1a3ac-105">При установке диапазонов дат следует руководствоваться определенными правилами.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-105">Special rules apply to the way you set date ranges.</span></span> <span data-ttu-id="1a3ac-106">Рассмотрим пример **Клиент - первая десятка**:</span><span class="sxs-lookup"><span data-stu-id="1a3ac-106">Let's take the **Customer Top 10** as an example:</span></span>

![Установка диапазона дат на странице запросов для списка "Клиент - первая десятка"](./media/ui-enter-date-ranges/customer-top10-list.png)

<span data-ttu-id="1a3ac-108">Здесь можно ограничить отчет по диапазону дат, например прошлыми двумя неделями или всего 6 неделями, либо любым другим диапазоном.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-108">Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want.</span></span> <span data-ttu-id="1a3ac-109">Для задания диапазонов дат необходимо указать даты и использовать **..**</span><span class="sxs-lookup"><span data-stu-id="1a3ac-109">To set date ranges, you enter dates and then use either **..**</span></span> <span data-ttu-id="1a3ac-110">или **|**, чтобы обозначить диапазон.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-110">or **|** to set the range.</span></span> <span data-ttu-id="1a3ac-111">В нашем примере для отображения десятки клиентов за первые две недели мая необходимо задать фильтра по дате *05 01 17..05 14 17*.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-111">In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.</span></span>
<span data-ttu-id="1a3ac-112">Вот еще несколько примеров:</span><span class="sxs-lookup"><span data-stu-id="1a3ac-112">Here are a couple of other examples:</span></span>

| <span data-ttu-id="1a3ac-113">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-113">Meaning</span></span> | <span data-ttu-id="1a3ac-114">Пример</span><span class="sxs-lookup"><span data-stu-id="1a3ac-114">Example</span></span> | <span data-ttu-id="1a3ac-115">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="1a3ac-115">Entries included</span></span> |
|---|---|---|
|<span data-ttu-id="1a3ac-116">Равный</span><span class="sxs-lookup"><span data-stu-id="1a3ac-116">Equal to</span></span>| <span data-ttu-id="1a3ac-117">15 12 16</span><span class="sxs-lookup"><span data-stu-id="1a3ac-117">12 15 16</span></span> |<span data-ttu-id="1a3ac-118">Только учтенные на 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-118">Only those posted on December 15 2016.</span></span>|
|<span data-ttu-id="1a3ac-119">Интервал</span><span class="sxs-lookup"><span data-stu-id="1a3ac-119">Interval</span></span>| <span data-ttu-id="1a3ac-120">15 12 16..15 17 17</span><span class="sxs-lookup"><span data-stu-id="1a3ac-120">12 15 16..01 15 17</span></span><br /><br /><span data-ttu-id="1a3ac-121">..12 15 16</span><span class="sxs-lookup"><span data-stu-id="1a3ac-121">..12 15 16</span></span>|<span data-ttu-id="1a3ac-122">Учтенные в даты между 15 декабря 2016 и 15 января 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-122">Those posted on dates between and including December 15 2016 and January 15 2017.</span></span><br /><br /><span data-ttu-id="1a3ac-123">Учтенные не позднее 15 декабря 2106 года</span><span class="sxs-lookup"><span data-stu-id="1a3ac-123">Those posted on December 15 2016 or earlier.</span></span>|
|<span data-ttu-id="1a3ac-124">Либо/или</span><span class="sxs-lookup"><span data-stu-id="1a3ac-124">Either/or</span></span>|<span data-ttu-id="1a3ac-125">12 15 16&#124;12 16 16</span><span class="sxs-lookup"><span data-stu-id="1a3ac-125">12 15 16&#124;12 16 16</span></span>|<span data-ttu-id="1a3ac-126">Учтенные 15 декабря или 15 декабря 2016 года.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-126">Those posted on either December 15 or December 16 2016.</span></span> <span data-ttu-id="1a3ac-127">При наличии операций, учтенных на обе даты, отображаются все эти операции.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-127">If there are entries posted on both days, they will all be displayed.</span></span>|

<span data-ttu-id="1a3ac-128">Также можно объединять разные типы форматов.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-128">You can also combine the various format types.</span></span>

| <span data-ttu-id="1a3ac-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1a3ac-129">Example</span></span> | <span data-ttu-id="1a3ac-130">Включенные операции</span><span class="sxs-lookup"><span data-stu-id="1a3ac-130">Entries included</span></span> |
|---|---|
|<span data-ttu-id="1a3ac-131">12 15 16&#124;12 01 16..05 31 17</span><span class="sxs-lookup"><span data-stu-id="1a3ac-131">12 15 16&#124;12 01 16..05 31 17</span></span> | <span data-ttu-id="1a3ac-132">Операции, учтенные 15 декабря 2016 или в даты между 01 декабря 2016 и 31 мая 2017 включительно.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-132">Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017.</span></span> |
|<span data-ttu-id="1a3ac-133">..12 14 16&#124;12 30 16..</span><span class="sxs-lookup"><span data-stu-id="1a3ac-133">..12 14 16&#124;12 30 16..</span></span> | <span data-ttu-id="1a3ac-134">Операции, учтенные не позднее 14 декабря, или операции, учтенные не раньше 30 декабря, т. е. все операции, кроме учтенных между 15 и 29 декабря (включительно).</span><span class="sxs-lookup"><span data-stu-id="1a3ac-134">Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29.</span></span> |

<span data-ttu-id="1a3ac-135">Обратите внимание, что здесь использован американский формат дат ММДДГГ.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-135">Note that we have used the US date format MMDDYY here.</span></span> <span data-ttu-id="1a3ac-136">Когда [!INCLUDE[d365fin](includes/d365fin_md.md)] появится на других рынках, вы сможете использовать те форматы, к которым вы привыкли.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-136">As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.</span></span>

## <a name="using-date-formulas"></a><span data-ttu-id="1a3ac-137">Использование формул дат</span><span class="sxs-lookup"><span data-stu-id="1a3ac-137">Using Date Formulas</span></span>
<span data-ttu-id="1a3ac-138">Формула даты — это краткая сокращенная буквенно-числовая комбинация, задающая способ вычисления дат.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-138">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="1a3ac-139">Формулы дат вводятся в различных вычисляемых полях даты и в полях частоты повторения в типовых журналах.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-139">You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.</span></span>

> [!NOTE]
>  <span data-ttu-id="1a3ac-140">Во всех полях формул данных один день включается автоматически для покрытия сегодняшнего дня как дня начала периода.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-140">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="1a3ac-141">Соответственно, например, если ввести **1W**, то период фактически будет равен восьми дням, поскольку в него включается сегодняшний.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-141">Accordingly, for example, if you enter **1W**, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="1a3ac-142">Чтобы указать период, равный семи дням (одной реальной неделе), включая дату начала периода, следует ввести **6D** или **1W\-1D**.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-142">To specify a period of seven days (one true week) including the period starting date, then you must enter **6D** or **1W\-1D**.</span></span>

<span data-ttu-id="1a3ac-143">Примеры использования формул дат:</span><span class="sxs-lookup"><span data-stu-id="1a3ac-143">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="1a3ac-144">Формула даты в поле частоты повторения в типовом журнале определяет периодичность учета операции в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-144">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="1a3ac-145">Формула даты в поле **Период отсрочки** того или иного уровня напоминания определяет период от срока оплаты (или от даты предыдущего напоминания) до создания напоминания.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-145">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date (or from the due date of the previous reminder) before a reminder will be created.</span></span>

-   <span data-ttu-id="1a3ac-146">Формула даты в поле **Расчет срока оплаты** определяет способ расчета даты оплаты в напоминании.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-146">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="1a3ac-147">Формула расчета даты может содержать до 20 знаков, как цифр, так и букв.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-147">The date calculation formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="1a3ac-148">Можно использовать следующие буквы, которые представляют собой аббревиатуры спецификации времени.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-148">You can use the following letters, which are abbreviations for time specifications.</span></span>

|  <span data-ttu-id="1a3ac-149">Буква</span><span class="sxs-lookup"><span data-stu-id="1a3ac-149">Letter</span></span>  |  <span data-ttu-id="1a3ac-150">Спецификация времени</span><span class="sxs-lookup"><span data-stu-id="1a3ac-150">Time specification</span></span>  |
|----------|----------------------|
|<span data-ttu-id="1a3ac-151">З</span><span class="sxs-lookup"><span data-stu-id="1a3ac-151">C</span></span>|<span data-ttu-id="1a3ac-152">Текущая</span><span class="sxs-lookup"><span data-stu-id="1a3ac-152">Current</span></span>|
|<span data-ttu-id="1a3ac-153">Д</span><span class="sxs-lookup"><span data-stu-id="1a3ac-153">D</span></span>|<span data-ttu-id="1a3ac-154">День\(дни\)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-154">Day\(s\)</span></span>|
|<span data-ttu-id="1a3ac-155">З</span><span class="sxs-lookup"><span data-stu-id="1a3ac-155">W</span></span>|<span data-ttu-id="1a3ac-156">Неделя\(недели\)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-156">Week\(s\)</span></span>|
|<span data-ttu-id="1a3ac-157">М</span><span class="sxs-lookup"><span data-stu-id="1a3ac-157">M</span></span>|<span data-ttu-id="1a3ac-158">Месяц\(месяцы\)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-158">Month\(s\)</span></span>|
|<span data-ttu-id="1a3ac-159">К</span><span class="sxs-lookup"><span data-stu-id="1a3ac-159">Q</span></span>|<span data-ttu-id="1a3ac-160">Квартал\(кварталы\)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-160">Quarter\(s\)</span></span>|
|<span data-ttu-id="1a3ac-161">Г</span><span class="sxs-lookup"><span data-stu-id="1a3ac-161">Y</span></span>|<span data-ttu-id="1a3ac-162">Год\(года\)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-162">Year\(s\)</span></span>|

<span data-ttu-id="1a3ac-163">Составить формулу даты можно тремя способами.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-163">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="1a3ac-164">В следующем примере описывается способ использования **C** в качестве текущей даты и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-164">The following example shows how to use **C**, for current, and a time unit.</span></span>

|  <span data-ttu-id="1a3ac-165">Выражение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-165">Expression</span></span>  |  <span data-ttu-id="1a3ac-166">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-166">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="1a3ac-167">CW</span><span class="sxs-lookup"><span data-stu-id="1a3ac-167">CW</span></span>|<span data-ttu-id="1a3ac-168">текущая неделя;</span><span class="sxs-lookup"><span data-stu-id="1a3ac-168">Current week</span></span>|
|<span data-ttu-id="1a3ac-169">ТМ</span><span class="sxs-lookup"><span data-stu-id="1a3ac-169">CM</span></span>|<span data-ttu-id="1a3ac-170">текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-170">Current month</span></span>|

<span data-ttu-id="1a3ac-171">В следующем примере описывается способ использования числа и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-171">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="1a3ac-172">Число не может быть больше 9999.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-172">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="1a3ac-173">Выражение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-173">Expression</span></span>  |  <span data-ttu-id="1a3ac-174">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-174">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="1a3ac-175">10D</span><span class="sxs-lookup"><span data-stu-id="1a3ac-175">10D</span></span>|<span data-ttu-id="1a3ac-176">через 10 дней после текущей даты;</span><span class="sxs-lookup"><span data-stu-id="1a3ac-176">10 days from today</span></span>|
|<span data-ttu-id="1a3ac-177">2W</span><span class="sxs-lookup"><span data-stu-id="1a3ac-177">2W</span></span>|<span data-ttu-id="1a3ac-178">через 2 недели после текущей даты.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-178">2 weeks from today</span></span>|

<span data-ttu-id="1a3ac-179">В следующем примере описывается способ использования единицы измерения времени и числа.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-179">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="1a3ac-180">Выражение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-180">Expression</span></span>  |  <span data-ttu-id="1a3ac-181">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-181">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="1a3ac-182">D10</span><span class="sxs-lookup"><span data-stu-id="1a3ac-182">D10</span></span>|<span data-ttu-id="1a3ac-183">следующий 10-й день месяца;</span><span class="sxs-lookup"><span data-stu-id="1a3ac-183">The next 10th day of a month</span></span>|
|<span data-ttu-id="1a3ac-184">WD4</span><span class="sxs-lookup"><span data-stu-id="1a3ac-184">WD4</span></span>|<span data-ttu-id="1a3ac-185">следующий 4-й день недели \(четверг\).</span><span class="sxs-lookup"><span data-stu-id="1a3ac-185">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="1a3ac-186">В следующем примере описывается способ комбинирования таких трех форм при необходимости.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-186">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="1a3ac-187">Выражение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-187">Expression</span></span>  |  <span data-ttu-id="1a3ac-188">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-188">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="1a3ac-189">CM\+10D</span><span class="sxs-lookup"><span data-stu-id="1a3ac-189">CM\+10D</span></span>|<span data-ttu-id="1a3ac-190">текущий месяц \+ 10 дней</span><span class="sxs-lookup"><span data-stu-id="1a3ac-190">Current month \+ 10 days</span></span>|

<span data-ttu-id="1a3ac-191">В следующем примере показано, как использовать знак минуса для указания прошедшей даты.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-191">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="1a3ac-192">Выражение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-192">Expression</span></span>  |  <span data-ttu-id="1a3ac-193">Значение</span><span class="sxs-lookup"><span data-stu-id="1a3ac-193">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="1a3ac-194">-1Г</span><span class="sxs-lookup"><span data-stu-id="1a3ac-194">-1Y</span></span>|<span data-ttu-id="1a3ac-195">1 год назад.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-195">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="1a3ac-196">Если на складе используется базовый календарь, то вводимая в это поле формула даты, например **Время отгрузки**, интерпретирована в соответствии с рабочими днями календаря.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-196">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="1a3ac-197">Например, **1W** означает семь рабочих дней.</span><span class="sxs-lookup"><span data-stu-id="1a3ac-197">For example, **1W**  means seven working days.</span></span>

## <a name="see-also"></a><span data-ttu-id="1a3ac-198">См. также</span><span class="sxs-lookup"><span data-stu-id="1a3ac-198">See Also</span></span>
<span data-ttu-id="1a3ac-199">[Работа с [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1a3ac-199">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="1a3ac-200">Расчет даты для покупок</span><span class="sxs-lookup"><span data-stu-id="1a3ac-200">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="1a3ac-201">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="1a3ac-201">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  

