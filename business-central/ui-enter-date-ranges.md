---
title: Ввод значений дат и времени в Business Central | Документация Майкрософт
description: Изучение процедуры ввода дат и времени, включая различные подсказки производительности, такие как стенография, выражения и диапазоны. Отфильтруйте списки отчеты до конкретных периодов времени или дат.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter, calendar, shorthand, range
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 404c39cba663cebc4d9ab30126de97bd20cf7e8e
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773534"
---
# <a name="working-with-calendar-dates-and-times"></a><span data-ttu-id="c84cc-104">Работа с календарными датами и значениями времени</span><span class="sxs-lookup"><span data-stu-id="c84cc-104">Working with Calendar Dates and Times</span></span>

[!INCLUDE[prod_short](includes/prod_long.md)] <span data-ttu-id="c84cc-105">предлагает несколько способов ввода дат и времени, включая мощные функции, которые ускоряют ввод данных или помогают написать сложные выражения календаря.</span><span class="sxs-lookup"><span data-stu-id="c84cc-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span></span> <span data-ttu-id="c84cc-106">Имеются различные места в приложении, в которых можно ввести в полях даты и значения времени.</span><span class="sxs-lookup"><span data-stu-id="c84cc-106">There are various places throughout the application where you can enter dates and times in fields.</span></span> <span data-ttu-id="c84cc-107">Например, в заказе на продажу можно установить дату отгрузки.</span><span class="sxs-lookup"><span data-stu-id="c84cc-107">For example, on a sales order, you can set the shipment date.</span></span> <span data-ttu-id="c84cc-108">При фильтрации данных или подготовке отчета по данным можно ввести даты и время для выделения только данных, в которых вы заинтересованы.</span><span class="sxs-lookup"><span data-stu-id="c84cc-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span></span>

## <a name="check-your-region-and-language-settings"></a><span data-ttu-id="c84cc-109">Проверьте свои настройки региона и языка</span><span class="sxs-lookup"><span data-stu-id="c84cc-109">Check your region and language settings</span></span>
<span data-ttu-id="c84cc-110">На странице **Мои настройки** указаны **Регион** и **Язык**, которые вы используете в приложении.</span><span class="sxs-lookup"><span data-stu-id="c84cc-110">The **My Settings** page specifies the **Region** and **Language** that you are using in the application.</span></span> <span data-ttu-id="c84cc-111">Данные настройки влияют на способ ввода дат и времени.</span><span class="sxs-lookup"><span data-stu-id="c84cc-111">These settings influence how you enter dates and times.</span></span>

-   <span data-ttu-id="c84cc-112">Настройка **Регион** определяет способ отображения или форматирования дат, времени, чисел и валюты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span></span>

-   <span data-ttu-id="c84cc-113">Для шаблонов дат, включающих слова, используемый язык слов должен совпадать с настройкой **Язык**.</span><span class="sxs-lookup"><span data-stu-id="c84cc-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span></span>

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_long.md)] <span data-ttu-id="c84cc-114">использует Григорианскую систему календаря.</span><span class="sxs-lookup"><span data-stu-id="c84cc-114">uses the Gregorian calendar system.</span></span>

<!--
The following sections describe how you can enter dates, times, datetimes, durations, date ranges, and how you use date formulas.
-->

## <a name="entering-dates"></a><span data-ttu-id="c84cc-115">Ввод дат</span><span class="sxs-lookup"><span data-stu-id="c84cc-115">Entering Dates</span></span>

<span data-ttu-id="c84cc-116">В поле даты можно ввести дату, используя стандартный формат для региона настройки.</span><span class="sxs-lookup"><span data-stu-id="c84cc-116">In a date field, you can enter a date using the standard format for your region setting.</span></span> <span data-ttu-id="c84cc-117">Можно использовать различные разделители в различных регионах между днями, месяцами и годами.</span><span class="sxs-lookup"><span data-stu-id="c84cc-117">Different regions can use different separators between the days, months and years.</span></span> <span data-ttu-id="c84cc-118">Например, некоторые регионы используют черточки (mm-dd-yyyy), другие используют наклонные черты (mm/dd/yyyy).</span><span class="sxs-lookup"><span data-stu-id="c84cc-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span></span> <span data-ttu-id="c84cc-119">Однако можно использовать любые разделители, даже пробелы, и дата будет автоматически изменена для использования разделителей в соответствии с регионом пользователя.</span><span class="sxs-lookup"><span data-stu-id="c84cc-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span></span>

<span data-ttu-id="c84cc-120">Обратите внимание, что формат, в котором отображаются даты в печатных отчетах или отправленных по электронной почте документах, не зависит от вашего личного выбора настроек региона.</span><span class="sxs-lookup"><span data-stu-id="c84cc-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span></span>

<span data-ttu-id="c84cc-121">Для работы продуктивнее с датами и временами можно использовать любой из методов или форматов, которые описаны в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="c84cc-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span></span>

### <a name="picking-dates-from-the-calendar"></a><span data-ttu-id="c84cc-122">Выбор дат из календаря</span><span class="sxs-lookup"><span data-stu-id="c84cc-122">Picking dates from the calendar</span></span>

<span data-ttu-id="c84cc-123">Любое поле, в котором отображается значок календаря, можно настроить с помощью средства выбора даты календаря.</span><span class="sxs-lookup"><span data-stu-id="c84cc-123">Any field displaying a calendar icon can be set using the calendar date picker.</span></span> <span data-ttu-id="c84cc-124">Для отображения средства выбора даты календаря активируйте значок календаря или нажмите сочетание клавиш CTRL + HOME в поле.</span><span class="sxs-lookup"><span data-stu-id="c84cc-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span></span>

<span data-ttu-id="c84cc-125">![Поля даты](media/ui-date-field.png "Пример поля даты")</span><span class="sxs-lookup"><span data-stu-id="c84cc-125">![Date fields](media/ui-date-field.png "Example of a date field")</span></span>

<span data-ttu-id="c84cc-126">См. также [Сочетания клавиш в элементе управления для выбора даты календаря](keyboard-shortcuts.md#calendarshortcuts).</span><span class="sxs-lookup"><span data-stu-id="c84cc-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts).</span></span>

### <a name="day-week-year-pattern"></a><span data-ttu-id="c84cc-127">Структура день\-неделя\-год</span><span class="sxs-lookup"><span data-stu-id="c84cc-127">Day\-week\-year pattern</span></span>

<span data-ttu-id="c84cc-128">Можно ввести дату как день недели, за которым следует номер недели и, необязательно, год.</span><span class="sxs-lookup"><span data-stu-id="c84cc-128">You can enter a date as a weekday followed by a week number and, optionally, a year.</span></span> <span data-ttu-id="c84cc-129">Например, Пон25 или пон25 означает понедельник недели 25.</span><span class="sxs-lookup"><span data-stu-id="c84cc-129">For example, Mon25 or mon25 means Monday in week 25.</span></span> <span data-ttu-id="c84cc-130">Год если не вводить, то используется год рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-130">If you do not enter a year, the year of the work date is used.</span></span>

<span data-ttu-id="c84cc-131">Вместо ввода всего слова для дня недели можно ввести слово часть, начиная с начала.</span><span class="sxs-lookup"><span data-stu-id="c84cc-131">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span></span> <span data-ttu-id="c84cc-132">В случае конфликта (например, с может быть субботой или средой), дни оцениваются в соответствии с настройками региона.</span><span class="sxs-lookup"><span data-stu-id="c84cc-132">In case of conflicts (such as with s which could be Saturday or Sunday), the days are evaluated according to the region setting.</span></span> <span data-ttu-id="c84cc-133">Сначала ввод оценивается по "рабочей дате" и "сегодня", поэтому помните об этом при сокращении.</span><span class="sxs-lookup"><span data-stu-id="c84cc-133">The input is first evaluated against workdate and today as well, so keep this in mind when abbreviating.</span></span> <span data-ttu-id="c84cc-134">Например, с уже означает сегодня, поэтому оно не может означать среду или субботу.</span><span class="sxs-lookup"><span data-stu-id="c84cc-134">For example, t already means today, so it cannot mean Tuesday or Thursday.</span></span>

<span data-ttu-id="c84cc-135">Схема номера недели всегда ISO 8601, в котором неделя 1 — это неделя, включающая 4-е января или неделя с первым четвергом года.</span><span class="sxs-lookup"><span data-stu-id="c84cc-135">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span></span>

### <a name="digit-patterns"></a><span data-ttu-id="c84cc-136">Цифровые схемы</span><span class="sxs-lookup"><span data-stu-id="c84cc-136">Digit patterns</span></span>

<span data-ttu-id="c84cc-137">В поле даты можно ввести две, четыре, шесть или восемь цифр:</span><span class="sxs-lookup"><span data-stu-id="c84cc-137">In a date field you can enter two, four, six, or eight digits:</span></span>

-   <span data-ttu-id="c84cc-138">Если введены только две цифры, они будут интерпретированы как день, а месяц и год будут добавлены к рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-138">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>

-   <span data-ttu-id="c84cc-139">Если введены четыре цифры, они будут интерпретированы как день и месяц, к которым будет добавлен год рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-139">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span> <span data-ttu-id="c84cc-140">Порядок дня и месяца определяется настройками региона.</span><span class="sxs-lookup"><span data-stu-id="c84cc-140">The order of the day and month is determined by your region settings.</span></span> <span data-ttu-id="c84cc-141">Даже если ваши настройки региона имеют года до дня и месяца, четыре цифры интерпретируются как день и месяц.</span><span class="sxs-lookup"><span data-stu-id="c84cc-141">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span></span>

-   <span data-ttu-id="c84cc-142">При вводе даты в интервале от 01.01.1930 до 31.12.2029 можно ввести две цифры года; в противном случае необходимо ввести все четыре цифры.</span><span class="sxs-lookup"><span data-stu-id="c84cc-142">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>

### <a name="today"></a><span data-ttu-id="c84cc-143">Сегодня</span><span class="sxs-lookup"><span data-stu-id="c84cc-143">Today</span></span>

<span data-ttu-id="c84cc-144">Введите слово "сегодня" на языке, заданном настройкой **Язык**, которая задает текущую дату.</span><span class="sxs-lookup"><span data-stu-id="c84cc-144">Enter the word for today, in the language set by **Language** setting, that will set the date to the current date.</span></span> <span data-ttu-id="c84cc-145">Вместо ввода всего слова можно ввести его часть, начиная с начала, например с или сег, чтобы оно не было также началом другого слова.</span><span class="sxs-lookup"><span data-stu-id="c84cc-145">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as t or tod, as long as it is not also the start of another word.</span></span>

### <a name="period"></a><span data-ttu-id="c84cc-146">периодам</span><span class="sxs-lookup"><span data-stu-id="c84cc-146">Period</span></span>

<span data-ttu-id="c84cc-147">Для фильтрации по определенному учетному периоду введите в поле даты букву п или слово период, затем введите число, которое указывает учетный период, например п2 или период4.</span><span class="sxs-lookup"><span data-stu-id="c84cc-147">To filter on a specific accounting period, in a date field enter the letter p, or the word period, followed by a number that identifies the accounting period, like p2 or period4.</span></span> <span data-ttu-id="c84cc-148">Учетный период задается по отношению к финансовому году текущей рабочей даты, которая задана в вашем ролевом центре.</span><span class="sxs-lookup"><span data-stu-id="c84cc-148">The accounting period is relative to the fiscal year of the current work date that set in your Role Center.</span></span> <span data-ttu-id="c84cc-149">Например, если рабочая дата **21.03.22**, то п1 или просто п выполняет фильтрацию по первому учетному периоду для финансового года 2022 (например, 01.01.22..31.01.22).</span><span class="sxs-lookup"><span data-stu-id="c84cc-149">For example, if the work date is **03/21/22**, then p1, or just p, filters on the first accounting period of the fiscal year 2022 (such as 01/01/22..01/31/22).</span></span> <span data-ttu-id="c84cc-150">п15 фильтрует по 15-му учетному периоду с начала финансового года 2022 (например, 01.03.23..31.03.23).</span><span class="sxs-lookup"><span data-stu-id="c84cc-150">p15 filters on the fifteenth accounting period from the start of fiscal year 2022 (such as 03/01/23..03/31/23).</span></span>

<span data-ttu-id="c84cc-151">Учетные периоды определяются на странице **Учетные периоды**.</span><span class="sxs-lookup"><span data-stu-id="c84cc-151">The accounting periods are defined on the **Accounting Periods** page.</span></span> <span data-ttu-id="c84cc-152">Для просмотра или изменения учетных периодов откройте страницу [здесь](https://businesscentral.dynamics.com/?page=100).</span><span class="sxs-lookup"><span data-stu-id="c84cc-152">To view or change the accounting periods, open the page [here](https://businesscentral.dynamics.com/?page=100).</span></span>

### <a name="current-work-date"></a><span data-ttu-id="c84cc-153">Текущая рабочая дата</span><span class="sxs-lookup"><span data-stu-id="c84cc-153">Current work date</span></span>

<span data-ttu-id="c84cc-154">Функция рабочей даты позволяет записывать транзакции с помощью даты, которая отличается от текущей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-154">The work date feature allows you to record transactions using a date that is different from the current date.</span></span>

<span data-ttu-id="c84cc-155">Слово, соответствующее "рабочей дате" на языке, заданном настройкой **Язык**, устанавливает дату равной текущей заданной рабочей дате, которая указана на странице **Мои настройки**.</span><span class="sxs-lookup"><span data-stu-id="c84cc-155">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the **My Settings** page.</span></span> <span data-ttu-id="c84cc-156">Вместо ввода всего слова можно ввести часть слова, начиная с начала, например 'р' или 'ра'.</span><span class="sxs-lookup"><span data-stu-id="c84cc-156">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span></span>

<span data-ttu-id="c84cc-157">Если рабочая дата не определена, в качестве рабочей даты будет использоваться текущая дата.</span><span class="sxs-lookup"><span data-stu-id="c84cc-157">If you have not defined a work date, the current date will be used as the work date.</span></span> <span data-ttu-id="c84cc-158">Необходимость в использовании рабочей даты возникает при наличии большого количества транзакций, дата которых отличается от текущей.</span><span class="sxs-lookup"><span data-stu-id="c84cc-158">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>

<span data-ttu-id="c84cc-159">См. также [Изменение базовых настроек, таких как рабочая дата](ui-change-basic-settings.md#work-date).</span><span class="sxs-lookup"><span data-stu-id="c84cc-159">See also [Change Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date).</span></span>

### <a name="closing-date"></a><span data-ttu-id="c84cc-160">Дата закрытия</span><span class="sxs-lookup"><span data-stu-id="c84cc-160">Closing Date</span></span>

<span data-ttu-id="c84cc-161">При закрытии финансового года можно использовать даты в специальном формате, указывающем на закрытие.</span><span class="sxs-lookup"><span data-stu-id="c84cc-161">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span></span> <span data-ttu-id="c84cc-162">Дата закрытия технически лежит между двумя календарными датами, например между 31 декабря и 1 января.</span><span class="sxs-lookup"><span data-stu-id="c84cc-162">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span></span>

<span data-ttu-id="c84cc-163">Чтобы указать, что дата является датой закрытия, следует непосредственно перед датой ввести букву З, например З123101.</span><span class="sxs-lookup"><span data-stu-id="c84cc-163">To specify that a date is a closing date, put C just before the date, such as C123101.</span></span> <span data-ttu-id="c84cc-164">Это можно использовать в сочетании со всеми схемами даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-164">This can be used in combination with all the date patterns.</span></span>

### <a name="examples"></a><span data-ttu-id="c84cc-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="c84cc-165">Examples</span></span>

<span data-ttu-id="c84cc-166">В следующей таблице содержится несколько примеров дат с использованием всех форматов.</span><span class="sxs-lookup"><span data-stu-id="c84cc-166">The following table contains examples of dates using all the formats.</span></span> <span data-ttu-id="c84cc-167">Предполагаются настройки региона, которые форматируют даты в соответствии со следующими параметрами: **год.месяц.дата.**, неделя начинается в понедельник и английский язык.</span><span class="sxs-lookup"><span data-stu-id="c84cc-167">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span></span>

|<span data-ttu-id="c84cc-168">**Формат ввода**</span><span class="sxs-lookup"><span data-stu-id="c84cc-168">**Entry**</span></span>      |<span data-ttu-id="c84cc-169">**Интерпретация**</span><span class="sxs-lookup"><span data-stu-id="c84cc-169">**Interpretation**</span></span>      |
|---------------|------------------------|
|<span data-ttu-id="c84cc-170">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-170">2022.12.31.</span></span>|<span data-ttu-id="c84cc-171">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-171">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-172">221231</span><span class="sxs-lookup"><span data-stu-id="c84cc-172">221231</span></span>|<span data-ttu-id="c84cc-173">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-173">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-174">22.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-174">22.12.31.</span></span>|<span data-ttu-id="c84cc-175">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-175">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-176">22.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-176">22.12.31.</span></span>|<span data-ttu-id="c84cc-177">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-177">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-178">20221231</span><span class="sxs-lookup"><span data-stu-id="c84cc-178">20221231</span></span>|<span data-ttu-id="c84cc-179">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-179">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-180">22/12,31</span><span class="sxs-lookup"><span data-stu-id="c84cc-180">22/12,31</span></span>|<span data-ttu-id="c84cc-181">2022.12.31.</span><span class="sxs-lookup"><span data-stu-id="c84cc-181">2022.12.31.</span></span>|
|<span data-ttu-id="c84cc-182">11</span><span class="sxs-lookup"><span data-stu-id="c84cc-182">11</span></span>|<span data-ttu-id="c84cc-183">год рабочей даты.месяц рабочей даты.11.</span><span class="sxs-lookup"><span data-stu-id="c84cc-183">work date year.work date month.11.</span></span>|
|<span data-ttu-id="c84cc-184">1112</span><span class="sxs-lookup"><span data-stu-id="c84cc-184">1112</span></span>|<span data-ttu-id="c84cc-185">год рабочей даты.11.12.</span><span class="sxs-lookup"><span data-stu-id="c84cc-185">work date year.11.12.</span></span>|
|<span data-ttu-id="c84cc-186">t или сегодня</span><span class="sxs-lookup"><span data-stu-id="c84cc-186">t or today</span></span>|<span data-ttu-id="c84cc-187">текущая дата</span><span class="sxs-lookup"><span data-stu-id="c84cc-187">today's date</span></span>|
|<span data-ttu-id="c84cc-188">п4</span><span class="sxs-lookup"><span data-stu-id="c84cc-188">p4</span></span>|<span data-ttu-id="c84cc-189">диапазон дат, который включает четвертый учетный период, такой как 01.04.20..30.04.20</span><span class="sxs-lookup"><span data-stu-id="c84cc-189">date range that includes the fourth accounting period, such as 04/01/20..04/30/20</span></span>|
|<span data-ttu-id="c84cc-190">w или рабочая дата</span><span class="sxs-lookup"><span data-stu-id="c84cc-190">w or workdate</span></span>|<span data-ttu-id="c84cc-191">рабочая дата</span><span class="sxs-lookup"><span data-stu-id="c84cc-191">the working date</span></span>|
|<span data-ttu-id="c84cc-192">m или понедельник</span><span class="sxs-lookup"><span data-stu-id="c84cc-192">m or Monday</span></span>|<span data-ttu-id="c84cc-193">Понедельник недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-193">Monday of the work date week</span></span>|
|<span data-ttu-id="c84cc-194">tu или вторник</span><span class="sxs-lookup"><span data-stu-id="c84cc-194">tu or Tuesday</span></span>|<span data-ttu-id="c84cc-195">Вторник недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-195">Tuesday of the work date week</span></span>|
|<span data-ttu-id="c84cc-196">су или суббота</span><span class="sxs-lookup"><span data-stu-id="c84cc-196">sa or Saturday</span></span>|<span data-ttu-id="c84cc-197">Суббота недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-197">Saturday of the work date week</span></span>|
|<span data-ttu-id="c84cc-198">во или воскресенье</span><span class="sxs-lookup"><span data-stu-id="c84cc-198">s or Sunday</span></span>|<span data-ttu-id="c84cc-199">Воскресенье недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-199">Sunday of the work date week</span></span>|
|<span data-ttu-id="c84cc-200">в23</span><span class="sxs-lookup"><span data-stu-id="c84cc-200">t23</span></span>|<span data-ttu-id="c84cc-201">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-201">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="c84cc-202">в 23</span><span class="sxs-lookup"><span data-stu-id="c84cc-202">t 23</span></span>|<span data-ttu-id="c84cc-203">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-203">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="c84cc-204">в-1</span><span class="sxs-lookup"><span data-stu-id="c84cc-204">t-1</span></span>|<span data-ttu-id="c84cc-205">Вторник недели 1 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="c84cc-205">Tuesday of week 1 of the work date year</span></span>|

##  <a name="setting-ranges"></a><a name="BKMK_SettingDateRanges"></a> <span data-ttu-id="c84cc-206">Диапазоны дат</span><span class="sxs-lookup"><span data-stu-id="c84cc-206">Setting Ranges</span></span>

<span data-ttu-id="c84cc-207">В списках, итогах и отчетах можно установить фильтры по датам, времени и дате и времени, содержащие начальное значение и, необязательно, конечное значение для отображения только данных, содержащихся в данном диапазоне.</span><span class="sxs-lookup"><span data-stu-id="c84cc-207">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span></span> <span data-ttu-id="c84cc-208">При установке диапазонов дат следует руководствоваться стандартными правилами.</span><span class="sxs-lookup"><span data-stu-id="c84cc-208">The standard rules apply to the way you set date ranges.</span></span>

|<span data-ttu-id="c84cc-209">**Значение**</span><span class="sxs-lookup"><span data-stu-id="c84cc-209">**Meaning**</span></span>|<span data-ttu-id="c84cc-210">**Пример выражения (дата)**</span><span class="sxs-lookup"><span data-stu-id="c84cc-210">**Sample expression (Date)**</span></span>|<span data-ttu-id="c84cc-211">**Данные, включенные в фильтр**</span><span class="sxs-lookup"><span data-stu-id="c84cc-211">**Data included in the filter**</span></span>|
|-----------|---------------------|--------------------|
|<span data-ttu-id="c84cc-212">Интервал</span><span class="sxs-lookup"><span data-stu-id="c84cc-212">Interval</span></span>|<span data-ttu-id="c84cc-213">15 12 00..15 01 01</span><span class="sxs-lookup"><span data-stu-id="c84cc-213">12 15 00..01 15 01</span></span><br /><br /><span data-ttu-id="c84cc-214">..15 12 00</span><span class="sxs-lookup"><span data-stu-id="c84cc-214">..12 15 00</span></span><br /><br /><span data-ttu-id="c84cc-215">п1..п4</span><span class="sxs-lookup"><span data-stu-id="c84cc-215">p1..p4</span></span>|<span data-ttu-id="c84cc-216">Записи датами, попадающими в период с 15.12.00 по 15.01.01 включительно.</span><span class="sxs-lookup"><span data-stu-id="c84cc-216">Records with dates between and including 12 15 00 and 01 15 01.</span></span><br /><br /><span data-ttu-id="c84cc-217">Записи с датами 15.12.00 или ранее.</span><span class="sxs-lookup"><span data-stu-id="c84cc-217">Records with dates of 12 15 00 or earlier.</span></span><br /><br /><span data-ttu-id="c84cc-218">Диапазон дат, который включает второй, третий и четвертый учетные периоды, такой как 01.01.20..30.04.20.</span><span class="sxs-lookup"><span data-stu-id="c84cc-218">Date range that includes the second, third, and fourth accounting periods, such as 01/01/20..04/30/20.</span></span>|
|<span data-ttu-id="c84cc-219">Либо/или</span><span class="sxs-lookup"><span data-stu-id="c84cc-219">Either/or</span></span>|<span data-ttu-id="c84cc-220">12 15 00\|12 16 00</span><span class="sxs-lookup"><span data-stu-id="c84cc-220">12 15 00\|12 16 00</span></span>|<span data-ttu-id="c84cc-221">Записи с датами 15.12.00 или 16.12.00.</span><span class="sxs-lookup"><span data-stu-id="c84cc-221">Records with dates of either 12 15 00 or 12 16 00.</span></span> <span data-ttu-id="c84cc-222">Если существуют записи с датами для обоих дней, все они будут выведены на экран.</span><span class="sxs-lookup"><span data-stu-id="c84cc-222">If there are records with dates on both days, they will all be displayed.</span></span>|
|<span data-ttu-id="c84cc-223">Комбинация</span><span class="sxs-lookup"><span data-stu-id="c84cc-223">Combination</span></span>|<span data-ttu-id="c84cc-224">12 15 00\|12 01 00..12 10 00</span><span class="sxs-lookup"><span data-stu-id="c84cc-224">12 15 00\|12 01 00..12 10 00</span></span>  <br /><br /><span data-ttu-id="c84cc-225">..12 14 00\|12 30 00..</span><span class="sxs-lookup"><span data-stu-id="c84cc-225">..12 14 00\|12 30 00..</span></span>|<span data-ttu-id="c84cc-226">Записи с датами 15.12.00 или за период с 01.12.00 по 10.12.00 включительно.</span><span class="sxs-lookup"><span data-stu-id="c84cc-226">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span></span>  <br /><br /><span data-ttu-id="c84cc-227">Записи с датами не позднее 14.12.00 или не ранее 30.12.00. То есть все записи за исключением тех, даты отклика которых попадают в период с 15.12.00 по 29.12.00 включительно.</span><span class="sxs-lookup"><span data-stu-id="c84cc-227">Records with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span></span>|

<span data-ttu-id="c84cc-228">Можно использовать любые допустимые форматы в фильтрах диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="c84cc-228">You can use any of the valid formats in date range filters.</span></span> <span data-ttu-id="c84cc-229">Например, пон14 3..с 4п при применении к полю даты и времени дает фильтр с 3 утра в понедельник в неделю 14 года текущей рабочей даты, включительно, до 16:00 сегодня, включительно.</span><span class="sxs-lookup"><span data-stu-id="c84cc-229">For example, mon14 3..t 4p applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span></span>

## <a name="using-date-formulas"></a><span data-ttu-id="c84cc-230">Использование формул дат</span><span class="sxs-lookup"><span data-stu-id="c84cc-230">Using Date Formulas</span></span>
<span data-ttu-id="c84cc-231">Формула даты — это краткая сокращенная буквенно-числовая комбинация, задающая способ вычисления дат.</span><span class="sxs-lookup"><span data-stu-id="c84cc-231">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="c84cc-232">Можно вводить формулы дат в различных вычисляемых полях расчета даты или фильтрах.</span><span class="sxs-lookup"><span data-stu-id="c84cc-232">You can enter date formulas in various date calculation fields or filters.</span></span>

> [!NOTE]
>  <span data-ttu-id="c84cc-233">Во всех полях формул данных один день включается автоматически для покрытия сегодняшнего дня как дня начала периода.</span><span class="sxs-lookup"><span data-stu-id="c84cc-233">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="c84cc-234">Соответственно, например, если ввести 1Н, то период фактически будет равен восьми дням, поскольку в него включается сегодняшний.</span><span class="sxs-lookup"><span data-stu-id="c84cc-234">Accordingly, for example, if you enter 1W, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="c84cc-235">Чтобы указать период, равный 7 дням \(одной реальной неделе\), включая дату начала периода, следует ввести 6Д или 1Н-1Д.</span><span class="sxs-lookup"><span data-stu-id="c84cc-235">To specify a period of seven days \(one true week\) including the period starting date, then you must enter 6D or 1W-1D.</span></span>

<span data-ttu-id="c84cc-236">Примеры использования формул дат:</span><span class="sxs-lookup"><span data-stu-id="c84cc-236">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="c84cc-237">Формула даты в поле частоты повторения в типовом журнале определяет периодичность учета операции в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="c84cc-237">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="c84cc-238">Формула даты в поле **Период отсрочки** того или иного уровня напоминания определяет период от срока оплаты \(или от даты предыдущего напоминания\) до создания напоминания.</span><span class="sxs-lookup"><span data-stu-id="c84cc-238">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span></span>

-   <span data-ttu-id="c84cc-239">Формула даты в поле **Расчет срока оплаты** определяет способ расчета даты оплаты в напоминании.</span><span class="sxs-lookup"><span data-stu-id="c84cc-239">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="c84cc-240">Формула даты может содержать до 20 знаков, как цифр, так и букв.</span><span class="sxs-lookup"><span data-stu-id="c84cc-240">The date formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="c84cc-241">В этих формулах можно использовать следующие сокращения календарных единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="c84cc-241">You can use the following letters, which are abbreviations for calendar units.</span></span>

|  <span data-ttu-id="c84cc-242">Буква</span><span class="sxs-lookup"><span data-stu-id="c84cc-242">Letter</span></span>  |  <span data-ttu-id="c84cc-243">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-243">Meaning</span></span>  |
|----------|----------------------|
|<span data-ttu-id="c84cc-244">Т</span><span class="sxs-lookup"><span data-stu-id="c84cc-244">C</span></span>|<span data-ttu-id="c84cc-245">текущий;</span><span class="sxs-lookup"><span data-stu-id="c84cc-245">Current</span></span>|
|<span data-ttu-id="c84cc-246">Д</span><span class="sxs-lookup"><span data-stu-id="c84cc-246">D</span></span>|<span data-ttu-id="c84cc-247">День\(дни\)</span><span class="sxs-lookup"><span data-stu-id="c84cc-247">Day\(s\)</span></span>|
|<span data-ttu-id="c84cc-248">Н</span><span class="sxs-lookup"><span data-stu-id="c84cc-248">W</span></span>|<span data-ttu-id="c84cc-249">Неделя\(недели\)</span><span class="sxs-lookup"><span data-stu-id="c84cc-249">Week\(s\)</span></span>|
|<span data-ttu-id="c84cc-250">М</span><span class="sxs-lookup"><span data-stu-id="c84cc-250">M</span></span>|<span data-ttu-id="c84cc-251">Месяц\(месяцы\)</span><span class="sxs-lookup"><span data-stu-id="c84cc-251">Month\(s\)</span></span>|
|<span data-ttu-id="c84cc-252">К</span><span class="sxs-lookup"><span data-stu-id="c84cc-252">Q</span></span>|<span data-ttu-id="c84cc-253">Квартал\(кварталы\)</span><span class="sxs-lookup"><span data-stu-id="c84cc-253">Quarter\(s\)</span></span>|
|<span data-ttu-id="c84cc-254">Г</span><span class="sxs-lookup"><span data-stu-id="c84cc-254">Y</span></span>|<span data-ttu-id="c84cc-255">Год\(года\)</span><span class="sxs-lookup"><span data-stu-id="c84cc-255">Year\(s\)</span></span>|

<span data-ttu-id="c84cc-256">Составить формулу даты можно тремя способами.</span><span class="sxs-lookup"><span data-stu-id="c84cc-256">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="c84cc-257">В следующем примере описывается способ использования Т в качестве текущей даты и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="c84cc-257">The following example shows how to use C, for current, and a time unit.</span></span>

|  <span data-ttu-id="c84cc-258">Выражение</span><span class="sxs-lookup"><span data-stu-id="c84cc-258">Expression</span></span>  |  <span data-ttu-id="c84cc-259">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-259">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="c84cc-260">ТН</span><span class="sxs-lookup"><span data-stu-id="c84cc-260">CW</span></span>|<span data-ttu-id="c84cc-261">текущая неделя;</span><span class="sxs-lookup"><span data-stu-id="c84cc-261">Current week</span></span>|
|<span data-ttu-id="c84cc-262">ТМ</span><span class="sxs-lookup"><span data-stu-id="c84cc-262">CM</span></span>|<span data-ttu-id="c84cc-263">текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="c84cc-263">Current month</span></span>|

<span data-ttu-id="c84cc-264">В следующем примере описывается способ использования числа и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="c84cc-264">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="c84cc-265">Число не может быть больше 9999.</span><span class="sxs-lookup"><span data-stu-id="c84cc-265">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="c84cc-266">Выражение</span><span class="sxs-lookup"><span data-stu-id="c84cc-266">Expression</span></span>  |  <span data-ttu-id="c84cc-267">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-267">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="c84cc-268">10Д</span><span class="sxs-lookup"><span data-stu-id="c84cc-268">10D</span></span>|<span data-ttu-id="c84cc-269">через 10 дней после текущей даты;</span><span class="sxs-lookup"><span data-stu-id="c84cc-269">10 days from today</span></span>|
|<span data-ttu-id="c84cc-270">2В</span><span class="sxs-lookup"><span data-stu-id="c84cc-270">2W</span></span>|<span data-ttu-id="c84cc-271">через 2 недели после текущей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-271">2 weeks from today</span></span>|

<span data-ttu-id="c84cc-272">В следующем примере описывается способ использования единицы измерения времени и числа.</span><span class="sxs-lookup"><span data-stu-id="c84cc-272">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="c84cc-273">Выражение</span><span class="sxs-lookup"><span data-stu-id="c84cc-273">Expression</span></span>  |  <span data-ttu-id="c84cc-274">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-274">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="c84cc-275">Д10</span><span class="sxs-lookup"><span data-stu-id="c84cc-275">D10</span></span>|<span data-ttu-id="c84cc-276">следующий 10-й день месяца;</span><span class="sxs-lookup"><span data-stu-id="c84cc-276">The next 10th day of a month</span></span>|
|<span data-ttu-id="c84cc-277">ДН4</span><span class="sxs-lookup"><span data-stu-id="c84cc-277">WD4</span></span>|<span data-ttu-id="c84cc-278">следующий 4-й день недели \(четверг\).</span><span class="sxs-lookup"><span data-stu-id="c84cc-278">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="c84cc-279">В следующем примере описывается способ комбинирования таких трех форм при необходимости.</span><span class="sxs-lookup"><span data-stu-id="c84cc-279">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="c84cc-280">Выражение</span><span class="sxs-lookup"><span data-stu-id="c84cc-280">Expression</span></span>  |  <span data-ttu-id="c84cc-281">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-281">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="c84cc-282">ТМ+10Д</span><span class="sxs-lookup"><span data-stu-id="c84cc-282">CM+10D</span></span>|<span data-ttu-id="c84cc-283">текущий месяц \+ 10 дней</span><span class="sxs-lookup"><span data-stu-id="c84cc-283">Current month \+ 10 days</span></span>|

<span data-ttu-id="c84cc-284">В следующем примере показано, как использовать знак минуса для указания прошедшей даты.</span><span class="sxs-lookup"><span data-stu-id="c84cc-284">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="c84cc-285">Выражение</span><span class="sxs-lookup"><span data-stu-id="c84cc-285">Expression</span></span>  |  <span data-ttu-id="c84cc-286">Значение</span><span class="sxs-lookup"><span data-stu-id="c84cc-286">Meaning</span></span>  |
|--------------|-----------|
|<span data-ttu-id="c84cc-287">-1Г</span><span class="sxs-lookup"><span data-stu-id="c84cc-287">-1Y</span></span>|<span data-ttu-id="c84cc-288">1 год назад.</span><span class="sxs-lookup"><span data-stu-id="c84cc-288">1 year ago from today</span></span>|

> [!IMPORTANT]
> <span data-ttu-id="c84cc-289">Если на складе используется базовый календарь, то вводимая в это поле формула даты, например **Время отгрузки**, интерпретирована в соответствии с рабочими днями календаря.</span><span class="sxs-lookup"><span data-stu-id="c84cc-289">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="c84cc-290">Например, 1Н означает семь рабочих дней.</span><span class="sxs-lookup"><span data-stu-id="c84cc-290">For example, 1W  means seven working days.</span></span>
<!--
# Entering Date Ranges
You can set filters containing a start date and an end date to display only the data contained in that date range or time interval. Special rules apply to the way you set date ranges. Let's take the **Customer Top 10** as an example:

![Setting a date range in the request page for the Customer Top 10 list](./media/ui-enter-date-ranges/customer-top10-list.png)

Here you can limit the report to a date range such as the past 2 weeks, or a total of 6 weeks, or whatever range you want. To set date ranges, you enter dates and then use either **..** or **|** to set the range. In our example, to show the top 10 customers for the first two weeks of May, you would set the date filter to *05 01 17..05 14 17*.
Here are a couple of other examples:

| Meaning | Example | Entries included |
|---|---|---|
|Equal to| 12 15 16 |Only those posted on December 15 2016.|
|Interval| 12 15 16..01 15 17<br /><br />..12 15 16|Those posted on dates between and including December 15 2016 and January 15 2017.<br /><br />Those posted on December 15 2016 or earlier.|
|Either/or|12 15 16&#124;12 16 16|Those posted on either December 15 or December 16 2016. If there are entries posted on both days, they will all be displayed.|

You can also combine the various format types.

| Example | Entries included |
|---|---|
|12 15 16&#124;12 01 16..05 31 17 | Entries posted either on December 15 2016 or on dates between and including December 01 2016 and May 31 2017. |
|..12 14 16&#124;12 30 16.. | Entries posted on December 14 or earlier, or entries posted on December 30 or later - that is, all entries except those posted on dates between and including December 15 and 29. |

Note that we have used the US date format MMDDYY here. As [!INCLUDE[prod_short](includes/prod_short.md)] becomes available in other markets, you'll be able to use the formats that you are used to.

## Using Date Formulas
A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates. You can enter date formulas in various date calculation fields and in recurring frequency fields in recurring journals.

> [!NOTE]
>  In all data formula fields, one day is automatically included to cover today as the day when the period starts. Accordingly, for example, if you enter **1W**, then the period is actually eight days because today is included. To specify a period of seven days (one true week) including the period starting date, then you must enter **6D** or **1W\-1D**.

Here are some examples of how date formulas can be used:

-   The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.

-   The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date (or from the due date of the previous reminder) before a reminder will be created.

-   The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.

The date calculation formula can contain a maximum of 20 characters, both numbers and letters. You can use the following letters, which are abbreviations for time specifications.

|  Letter  |  Time specification  |
|----------|----------------------|
|C|Current|
|D|Day\(s\)|
|W|Week\(s\)|
|M|Month\(s\)|
|Q|Quarter\(s\)|
|Y|Year\(s\)|

You can construct a date formula in three ways.

The following example shows how to use **C**, for current, and a time unit.

|  Expression  |  Meaning  |
|--------------|-----------|
|CW|Current week|
|CM|Current month|

The following example shows how to use a number and a time unit. A number cannot be larger than 9999.

|  Expression  |  Meaning  |
|--------------|-----------|
|10D|10 days from today|
|2W|2 weeks from today|

The following example shows how to use a time unit and a number.

|  Expression  |  Meaning  |
|--------------|-----------|
|D10|The next 10th day of a month|
|WD4|The next 4th day of a week \(Thursday\)|

The following example shows how you can combine these three forms as needed.

|  Expression  |  Meaning  |
|--------------|-----------|
|CM\+10D|Current month \+ 10 days|

The following example shows how you can use a minus sign to indicate a date in the past.

|  Expression  |  Meaning  |
|--------------|-----------|
|-1Y|1 year ago from today|

> [!IMPORTANT]
>  If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days. For example, **1W**  means seven working days.

-->

## <a name="entering-times"></a><span data-ttu-id="c84cc-291">Ввод времени</span><span class="sxs-lookup"><span data-stu-id="c84cc-291">Entering Times</span></span>
<span data-ttu-id="c84cc-292">При вводе времени можно вставить любые разделители, отличные от пробелов, которые необходимы между единицами измерения, но при использовании двух цифр для каждой единицы измерения вплоть до миллисекунд это не является необходимым.</span><span class="sxs-lookup"><span data-stu-id="c84cc-292">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span></span>

<span data-ttu-id="c84cc-293">Следует только записать наибольшую необходимую единицу измерения; остатки будет установлен на нуль.</span><span class="sxs-lookup"><span data-stu-id="c84cc-293">You only have to write the largest units that you require; the rest will be set to zero.</span></span> <span data-ttu-id="c84cc-294">Также можно не указывать никакого индикатора AM/PM.</span><span class="sxs-lookup"><span data-stu-id="c84cc-294">You can also leave out any AM/PM indicator.</span></span>

<span data-ttu-id="c84cc-295">В следующей таблице представлены способы ввода времени и их интерпретация.</span><span class="sxs-lookup"><span data-stu-id="c84cc-295">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span> <span data-ttu-id="c84cc-296">Предполагаются настройки региона, которые форматируют время в соответствии со следующими параметрами: **Часы:Минуты:Секунды.Миллисекунды.**</span><span class="sxs-lookup"><span data-stu-id="c84cc-296">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span></span> <span data-ttu-id="c84cc-297">и используются показатели до и после полудня "AM" и "PM", соответственно.</span><span class="sxs-lookup"><span data-stu-id="c84cc-297">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span></span>

|<span data-ttu-id="c84cc-298">**Формат ввода**</span><span class="sxs-lookup"><span data-stu-id="c84cc-298">**Entry**</span></span>      |<span data-ttu-id="c84cc-299">**Интерпретация**</span><span class="sxs-lookup"><span data-stu-id="c84cc-299">**Interpretation**</span></span>      |
|---------------|------------------------|
|<span data-ttu-id="c84cc-300">05:23:17</span><span class="sxs-lookup"><span data-stu-id="c84cc-300">05:23:17</span></span>|<span data-ttu-id="c84cc-301">05:23:17</span><span class="sxs-lookup"><span data-stu-id="c84cc-301">05:23:17</span></span>|
|<span data-ttu-id="c84cc-302">5</span><span class="sxs-lookup"><span data-stu-id="c84cc-302">5</span></span>|<span data-ttu-id="c84cc-303">05:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-303">05:00:00</span></span>|
|<span data-ttu-id="c84cc-304">5AM</span><span class="sxs-lookup"><span data-stu-id="c84cc-304">5AM</span></span>|<span data-ttu-id="c84cc-305">05:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-305">05:00:00</span></span>|
|<span data-ttu-id="c84cc-306">5P</span><span class="sxs-lookup"><span data-stu-id="c84cc-306">5P</span></span>|<span data-ttu-id="c84cc-307">17:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-307">17:00:00</span></span>|
|<span data-ttu-id="c84cc-308">12</span><span class="sxs-lookup"><span data-stu-id="c84cc-308">12</span></span>|<span data-ttu-id="c84cc-309">12:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-309">12:00:00</span></span>|
|<span data-ttu-id="c84cc-310">12А</span><span class="sxs-lookup"><span data-stu-id="c84cc-310">12A</span></span>|<span data-ttu-id="c84cc-311">00:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-311">00:00:00</span></span>|
|<span data-ttu-id="c84cc-312">12P</span><span class="sxs-lookup"><span data-stu-id="c84cc-312">12P</span></span>|<span data-ttu-id="c84cc-313">12:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-313">12:00:00</span></span>|
|<span data-ttu-id="c84cc-314">17</span><span class="sxs-lookup"><span data-stu-id="c84cc-314">17</span></span>|<span data-ttu-id="c84cc-315">17:00:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-315">17:00:00</span></span>|
|<span data-ttu-id="c84cc-316">5:30</span><span class="sxs-lookup"><span data-stu-id="c84cc-316">5:30</span></span>|<span data-ttu-id="c84cc-317">05:30:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-317">05:30:00</span></span>|
|<span data-ttu-id="c84cc-318">0530</span><span class="sxs-lookup"><span data-stu-id="c84cc-318">0530</span></span>|<span data-ttu-id="c84cc-319">05:30:00</span><span class="sxs-lookup"><span data-stu-id="c84cc-319">05:30:00</span></span>|
|<span data-ttu-id="c84cc-320">5:30:5</span><span class="sxs-lookup"><span data-stu-id="c84cc-320">5:30:5</span></span>|<span data-ttu-id="c84cc-321">05:30:05</span><span class="sxs-lookup"><span data-stu-id="c84cc-321">05:30:05</span></span>|
|<span data-ttu-id="c84cc-322">053005</span><span class="sxs-lookup"><span data-stu-id="c84cc-322">053005</span></span>|<span data-ttu-id="c84cc-323">05:30:05</span><span class="sxs-lookup"><span data-stu-id="c84cc-323">05:30:05</span></span>|
|<span data-ttu-id="c84cc-324">5:30:5,50</span><span class="sxs-lookup"><span data-stu-id="c84cc-324">5:30:5,50</span></span>|<span data-ttu-id="c84cc-325">05:30:05,5</span><span class="sxs-lookup"><span data-stu-id="c84cc-325">05:30:05.5</span></span>|
|<span data-ttu-id="c84cc-326">053005050</span><span class="sxs-lookup"><span data-stu-id="c84cc-326">053005050</span></span>|<span data-ttu-id="c84cc-327">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="c84cc-327">05:30:05.05</span></span>|

<span data-ttu-id="c84cc-328">Необходимо помнить, что миллисекунды интерпретируются как десятичная нотация.</span><span class="sxs-lookup"><span data-stu-id="c84cc-328">You should be aware that milliseconds are interpreted as decimal notation.</span></span> <span data-ttu-id="c84cc-329">Поэтому, например, 3, 30 и 300 все означают 300 миллисекунд, а 03 означает 30 и 003 означает 3 миллисекунды.</span><span class="sxs-lookup"><span data-stu-id="c84cc-329">So, for example, 3, 30, and 300 all mean 300 milliseconds, while 03 means 30 and 003 means 3 milliseconds.</span></span>

<span data-ttu-id="c84cc-330">Нельзя использовать 24:00 для полночи или использовать любое значение, большее 24:00.</span><span class="sxs-lookup"><span data-stu-id="c84cc-330">You cannot use 24:00 to mean midnight, or use any value greater than 24:00.</span></span>

<span data-ttu-id="c84cc-331">Слово "время" на языке, используемом [!INCLUDE[prod_short](includes/prod_long.md)], будет оценено как текущее время на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="c84cc-331">The word for 'time' in the language used by [!INCLUDE[prod_short](includes/prod_long.md)] will be evaluated to the current time on your computer or mobile device.</span></span> <span data-ttu-id="c84cc-332">Можно ввести любую часть слова, начиная с начала, например в или ВРЕМ.</span><span class="sxs-lookup"><span data-stu-id="c84cc-332">You can enter any part of the word, starting from the beginning, such as t or TIM.</span></span>

## <a name="entering-combined-dates-and-times"></a><span data-ttu-id="c84cc-333">Ввод комбинированных дат и времени</span><span class="sxs-lookup"><span data-stu-id="c84cc-333">Entering Combined Dates and Times</span></span>

[!INCLUDE [datetimes](includes/datetimes.md)]

## <a name="entering-duration"></a><span data-ttu-id="c84cc-334">Ввод продолжительности</span><span class="sxs-lookup"><span data-stu-id="c84cc-334">Entering Duration</span></span>
<span data-ttu-id="c84cc-335">Некоторые поля в приложении представляют длительность или прошедшее время, а не определенную дату или время.</span><span class="sxs-lookup"><span data-stu-id="c84cc-335">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span></span> <span data-ttu-id="c84cc-336">Длительность вводится в виде числа, за которым следует единица измерения.</span><span class="sxs-lookup"><span data-stu-id="c84cc-336">You enter a duration as a number followed by its unit of measure.</span></span>

<span data-ttu-id="c84cc-337">Примеры:</span><span class="sxs-lookup"><span data-stu-id="c84cc-337">Here are some examples.</span></span>

|<span data-ttu-id="c84cc-338">**Длительность**</span><span class="sxs-lookup"><span data-stu-id="c84cc-338">**Duration**</span></span>|<span data-ttu-id="c84cc-339">**Единица измерения**</span><span class="sxs-lookup"><span data-stu-id="c84cc-339">**Unit of measure**</span></span>|
|------------|-------------------|
|<span data-ttu-id="c84cc-340">2ч</span><span class="sxs-lookup"><span data-stu-id="c84cc-340">2h</span></span>|<span data-ttu-id="c84cc-341">2 часа</span><span class="sxs-lookup"><span data-stu-id="c84cc-341">2 hrs</span></span>|
|<span data-ttu-id="c84cc-342">6ч 30мин</span><span class="sxs-lookup"><span data-stu-id="c84cc-342">6h 30 m</span></span>|<span data-ttu-id="c84cc-343">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="c84cc-343">6 hrs 30 mins</span></span>|
|<span data-ttu-id="c84cc-344">6,5ч</span><span class="sxs-lookup"><span data-stu-id="c84cc-344">6.5h</span></span>|<span data-ttu-id="c84cc-345">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="c84cc-345">6 hrs 30 mins</span></span>|
|<span data-ttu-id="c84cc-346">90мин</span><span class="sxs-lookup"><span data-stu-id="c84cc-346">90m</span></span>|<span data-ttu-id="c84cc-347">1 час 30 минут</span><span class="sxs-lookup"><span data-stu-id="c84cc-347">1 hr 30 mins</span></span>|
|<span data-ttu-id="c84cc-348">2дн 6ч 30мин</span><span class="sxs-lookup"><span data-stu-id="c84cc-348">2d 6h 30m</span></span>|<span data-ttu-id="c84cc-349">2 дня 6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="c84cc-349">2 days 6 hrs 30 mins</span></span>|
|<span data-ttu-id="c84cc-350">2дн 6ч 30мин 56сек 600мс</span><span class="sxs-lookup"><span data-stu-id="c84cc-350">2d 6h 30m 56s 600ms</span></span>|<span data-ttu-id="c84cc-351">2 дня 6 часов 30 минут 56 секунд 600 миллисекунд</span><span class="sxs-lookup"><span data-stu-id="c84cc-351">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|

<span data-ttu-id="c84cc-352">Можно также ввести число, которое будет автоматически преобразовано во временной интервал.</span><span class="sxs-lookup"><span data-stu-id="c84cc-352">You can also enter a number, which will be automatically converted to a duration.</span></span> <span data-ttu-id="c84cc-353">При этом по умолчанию используется единица измерения, указанная в поле «Длительность».</span><span class="sxs-lookup"><span data-stu-id="c84cc-353">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>

<span data-ttu-id="c84cc-354">Чтобы узнать, какая единица измерения указана в поле "Длительность", введите любое число и посмотрите, в какую единицу измерения оно преобразуется.</span><span class="sxs-lookup"><span data-stu-id="c84cc-354">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>

<span data-ttu-id="c84cc-355">Например, если по умолчанию используются часы, число 5 будет преобразовано в 5 часов.</span><span class="sxs-lookup"><span data-stu-id="c84cc-355">For example, if the unit of measure is hours, the number 5 is converted to 5 hrs.</span></span>

## <a name="see-also"></a><span data-ttu-id="c84cc-356">См. также</span><span class="sxs-lookup"><span data-stu-id="c84cc-356">See Also</span></span>
<span data-ttu-id="c84cc-357">[Работа с [!INCLUDE[prod_short](includes/prod_long.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c84cc-357">[Working with [!INCLUDE[prod_short](includes/prod_long.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="c84cc-358">Расчет даты для покупок</span><span class="sxs-lookup"><span data-stu-id="c84cc-358">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="c84cc-359">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="c84cc-359">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]