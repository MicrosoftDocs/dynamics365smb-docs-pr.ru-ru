---
title: "Ввод значений дат и времени в Business Central | Документы Майкрософт"
description: "Изучение процедуры ввода дат и времени, включая различные подсказки производительности, такие как стенография, выражения и диапазоны. Отфильтруйте списки отчеты до конкретных периодов времени или дат."
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: dates, reporting, filter, calendar, shorthand, range
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 8717d60a8449ca300eaf9c1a5c4b137ea1a1a247
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---

# <a name="working-with-calendar-dates-and-times"></a><span data-ttu-id="21981-104">Работа с календарными датами и значениями времени</span><span class="sxs-lookup"><span data-stu-id="21981-104">Working with Calendar Dates and Times</span></span>
[!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="21981-105">предлагает несколько способов ввода дат и времени, включая мощные функции, которые ускоряют ввод данных или помогают написать сложные выражения календаря.</span><span class="sxs-lookup"><span data-stu-id="21981-105">offers multiple ways to enter dates and times, including powerful features that accelerate data entry, or help you write complex calendar expressions.</span></span> <span data-ttu-id="21981-106">Имеются различные места в приложении, в которых можно ввести в полях даты и значения времени.</span><span class="sxs-lookup"><span data-stu-id="21981-106">There are various places throughout the application where you can enter dates and times in fields.</span></span> <span data-ttu-id="21981-107">Например, в заказе на продажу можно установить дату отгрузки.</span><span class="sxs-lookup"><span data-stu-id="21981-107">For example, on a sales order, you can set the shipment date.</span></span> <span data-ttu-id="21981-108">При фильтрации данных или подготовке отчета по данным можно ввести даты и время для выделения только данных, в которых вы заинтересованы.</span><span class="sxs-lookup"><span data-stu-id="21981-108">When filtering lists or report data, you can enter dates and times to pinpoint only the data that you are interested in.</span></span>

## <a name="check-your-region-and-language-settings"></a><span data-ttu-id="21981-109">Проверьте свои настройки региона и языка</span><span class="sxs-lookup"><span data-stu-id="21981-109">Check your region and language settings</span></span>
<span data-ttu-id="21981-110">Страница [**Мои настройки**](https://businesscentral.dynamics.com?page=9176 "Прямой переход на страницу настроек пользователя в Business Central") задает **Регион** и **Язык**, которые вы используете в приложении.</span><span class="sxs-lookup"><span data-stu-id="21981-110">The [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page specifies the **Region** and **Language** that you are using in the application.</span></span> <span data-ttu-id="21981-111">Данные настройки влияют на способ ввода дат и времени.</span><span class="sxs-lookup"><span data-stu-id="21981-111">These settings influence how you enter dates and times.</span></span> 

-   <span data-ttu-id="21981-112">Настройка **Регион** определяет способ отображения или форматирования дат, времени, чисел и валюты.</span><span class="sxs-lookup"><span data-stu-id="21981-112">The **Region** setting determines how dates, times, numbers, and currencies are shown or formatted.</span></span>

-   <span data-ttu-id="21981-113">Для шаблонов дат, включающих слова, используемый язык слов должен совпадать с настройкой **Язык**.</span><span class="sxs-lookup"><span data-stu-id="21981-113">For date patterns that involve words, the language of the words that you use must correspond to the **Language** setting.</span></span>

> [!NOTE]
> [!INCLUDE[d365fin](includes/d365fin_long_md.md)] <span data-ttu-id="21981-114">использует Григорианскую систему календаря.</span><span class="sxs-lookup"><span data-stu-id="21981-114">uses the Gregorian calendar system.</span></span>

<!-- 
The following sections describe how you can enter dates, times, datetimes, durations, date ranges, and how you use date formulas.
-->
## <a name="entering-dates"></a><span data-ttu-id="21981-115">Ввод дат</span><span class="sxs-lookup"><span data-stu-id="21981-115">Entering Dates</span></span>
<span data-ttu-id="21981-116">В поле даты можно ввести дату, используя стандартный формат для региона настройки.</span><span class="sxs-lookup"><span data-stu-id="21981-116">In a date field, you can enter a date using the standard format for your region setting.</span></span> <span data-ttu-id="21981-117">Можно использовать различные разделители в различных регионах между днями, месяцами и годами.</span><span class="sxs-lookup"><span data-stu-id="21981-117">Different regions can use different separators between the days, months and years.</span></span> <span data-ttu-id="21981-118">Например, некоторые регионы используют черточки (mm-dd-yyyy), другие используют наклонные черты (mm/dd/yyyy).</span><span class="sxs-lookup"><span data-stu-id="21981-118">For example, some regions use dashes (mm-dd-yyyy) and others use forward slashes (mm/dd/yyyy).</span></span> <span data-ttu-id="21981-119">Однако можно использовать любые разделители, даже пробелы, и дата будет автоматически изменена для использования разделителей в соответствии с регионом пользователя.</span><span class="sxs-lookup"><span data-stu-id="21981-119">However, you can use any separators, even a space, and the date will automatically be changed to use separators that match your region.</span></span>

<span data-ttu-id="21981-120">Обратите внимание, что формат, в котором отображаются даты в печатных отчетах или отправленных по электронной почте документах, не зависит от вашего личного выбора настроек региона.</span><span class="sxs-lookup"><span data-stu-id="21981-120">Note that the format in which dates are displayed on printed reports or emailed documents is not influenced by your personal choice of region setting.</span></span>

<span data-ttu-id="21981-121">Для работы продуктивнее с датами и временами можно использовать любой из методов или форматов, которые описаны в следующих разделах.</span><span class="sxs-lookup"><span data-stu-id="21981-121">To work more productively with dates and times, you can use any of the methods or formats that are described in the following sections.</span></span> 

### <a name="picking-dates-from-the-calendar"></a><span data-ttu-id="21981-122">Выбор дат из календаря</span><span class="sxs-lookup"><span data-stu-id="21981-122">Picking dates from the calendar</span></span>
<span data-ttu-id="21981-123">Любое поле, в котором отображается значок календаря, можно настроить с помощью средства выбора даты календаря.</span><span class="sxs-lookup"><span data-stu-id="21981-123">Any field displaying a calendar icon can be set using the calendar date picker.</span></span> <span data-ttu-id="21981-124">Для отображения средства выбора даты календаря активируйте значок календаря или нажмите сочетание клавиш CTRL + HOME в поле.</span><span class="sxs-lookup"><span data-stu-id="21981-124">To display the calendar date picker, activate the calendar icon or press the Ctrl + Home keyboard shortcut in the field.</span></span>

<span data-ttu-id="21981-125">![Поля даты](media/ui-date-field.png "Пример поля даты")</span><span class="sxs-lookup"><span data-stu-id="21981-125">![Date fields](media/ui-date-field.png "Example of a date field")</span></span>

<span data-ttu-id="21981-126">См. также [Сочетания клавиш в элементе управления для выбора даты календаря](keyboard-shortcuts.md#calendarshortcuts)</span><span class="sxs-lookup"><span data-stu-id="21981-126">See also [Keyboard Shortcuts in the calendar date picker](keyboard-shortcuts.md#calendarshortcuts)</span></span>

### <a name="today"></a><span data-ttu-id="21981-127">Сегодня</span><span class="sxs-lookup"><span data-stu-id="21981-127">Today</span></span>
<span data-ttu-id="21981-128">Введите слово `today` на языке, заданном настройкой **Язык**, которая задает текущую дату.</span><span class="sxs-lookup"><span data-stu-id="21981-128">Enter the word for `today`, in the language set by **Language** setting, that will set the date to the current date.</span></span> <span data-ttu-id="21981-129">Вместо ввода всего слова можно ввести его часть, начиная с начала, например `t` или `tod`, чтобы оно не было также началом другого слова.</span><span class="sxs-lookup"><span data-stu-id="21981-129">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as `t` or `tod`, as long as it is not also the start of another word.</span></span>

### <a name="day-week-year-pattern"></a><span data-ttu-id="21981-130">Структура день\-неделя\-год</span><span class="sxs-lookup"><span data-stu-id="21981-130">Day\-week\-year pattern</span></span>
<span data-ttu-id="21981-131">Можно ввести дату как день недели, за которым следует номер недели и, необязательно, год.</span><span class="sxs-lookup"><span data-stu-id="21981-131">You can enter a date as a weekday followed by a week number and, optionally, a year.</span></span> <span data-ttu-id="21981-132">Например, `Mon25` или `mon25` означает понедельник недели 25.</span><span class="sxs-lookup"><span data-stu-id="21981-132">For example, `Mon25` or `mon25` means Monday in week 25.</span></span> <span data-ttu-id="21981-133">Год если не вводить, то используется год рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-133">If you do not enter a year, the year of the work date is used.</span></span>

<span data-ttu-id="21981-134">Вместо ввода всего слова для дня недели можно ввести слово часть, начиная с начала.</span><span class="sxs-lookup"><span data-stu-id="21981-134">Instead of entering the entire word for the day of the week, you can enter part of the word, starting from the beginning.</span></span> <span data-ttu-id="21981-135">В случае конфликта (например, `s` может быть субботой или воскресеньем), дни оцениваются в соответствии с настройками региона.</span><span class="sxs-lookup"><span data-stu-id="21981-135">In case of conflicts (such as with `s` which could be Saturday or Sunday), the days are evaluated according to the region setting.</span></span> <span data-ttu-id="21981-136">Сначала ввод оценивается по `workdate` и `today` также, поэтому помните об этом при сокращении.</span><span class="sxs-lookup"><span data-stu-id="21981-136">The input is first evaluated against `workdate` and `today` as well, so keep this in mind when abbreviating.</span></span> <span data-ttu-id="21981-137">Например, `t` уже означает сегодня, поэтому оно не может означать вторник или четверг.</span><span class="sxs-lookup"><span data-stu-id="21981-137">For example, `t` already means today, so it cannot mean Tuesday or Thursday.</span></span>

<span data-ttu-id="21981-138">Схема номера недели всегда ISO 8601, в котором неделя 1 — это неделя, включающая 4-е января или неделя с первым четвергом года.</span><span class="sxs-lookup"><span data-stu-id="21981-138">The week number scheme is always ISO 8601, where week 1 is the week with 4 January in it, or the week with the first Thursday of the year.</span></span>

### <a name="digit-patterns"></a><span data-ttu-id="21981-139">Цифровые схемы</span><span class="sxs-lookup"><span data-stu-id="21981-139">Digit patterns</span></span>
<span data-ttu-id="21981-140">В поле даты можно ввести две, четыре, шесть или восемь цифр:</span><span class="sxs-lookup"><span data-stu-id="21981-140">In a date field you can enter two, four, six, or eight digits:</span></span>

-   <span data-ttu-id="21981-141">Если введены только две цифры, они будут интерпретированы как день, а месяц и год будут добавлены к рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-141">If you enter only two digits, this is interpreted as the day, and it will add the month and the year of the work date.</span></span>

-   <span data-ttu-id="21981-142">Если введены четыре цифры, они будут интерпретированы как день и месяц, к которым будет добавлен год рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-142">If you enter four digits, this is interpreted as the day and the month, and it will add the year of the work date.</span></span> <span data-ttu-id="21981-143">Порядок дня и месяца определяется настройками региона.</span><span class="sxs-lookup"><span data-stu-id="21981-143">The order of the day and month is determined by your region settings.</span></span> <span data-ttu-id="21981-144">Даже если ваши настройки региона имеют года до дня и месяца, четыре цифры интерпретируются как день и месяц.</span><span class="sxs-lookup"><span data-stu-id="21981-144">Even if your region settings have the year before the day and month, four digits are interpreted as the day and month.</span></span>

-   <span data-ttu-id="21981-145">При вводе даты в интервале от 01.01.1930 до 31.12.2029 можно ввести две цифры года; в противном случае необходимо ввести все четыре цифры.</span><span class="sxs-lookup"><span data-stu-id="21981-145">If the date you want to enter is in the range 01/01/1930 through 12/31/2029, you can enter the year with two digits; otherwise, enter the year with four digits.</span></span>

### <a name="current-work-date"></a><span data-ttu-id="21981-146">Текущая рабочая дата</span><span class="sxs-lookup"><span data-stu-id="21981-146">Current work date</span></span>
<span data-ttu-id="21981-147">Функция рабочей даты позволяет записывать транзакции с помощью даты, которая отличается от текущей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-147">The work date feature allows you to record transations using a date that is different from the current date.</span></span>

<span data-ttu-id="21981-148">Слово для "рабочей даты" в языке, заданном настройкой **Язык**, установит дату текущей заданной рабочей даты, которая задана на странице [**Мои настройки**](https://businesscentral.dynamics.com?page=9176 "Прямой переход на страницу настроек пользователя в Business Central").</span><span class="sxs-lookup"><span data-stu-id="21981-148">The word for 'workdate', in the language set by **Language** setting, will set the date to the currently set work date that is specified on the [**My Settings**](https://businesscentral.dynamics.com?page=9176 "Go directly to your user settings page in Business Central") page.</span></span> <span data-ttu-id="21981-149">Вместо ввода всего слова можно ввести часть слова, начиная с начала, например 'w' или 'work'.</span><span class="sxs-lookup"><span data-stu-id="21981-149">Instead of entering the entire word, you can enter part of the word, starting from the beginning, such as 'w' or 'work'.</span></span>

<span data-ttu-id="21981-150">Если рабочая дата не определена, в качестве рабочей даты будет использоваться текущая дата.</span><span class="sxs-lookup"><span data-stu-id="21981-150">If you have not defined a work date, the current date will be used as the work date.</span></span> <span data-ttu-id="21981-151">Необходимость в использовании рабочей даты возникает при наличии большого количества транзакций, дата которых отличается от текущей.</span><span class="sxs-lookup"><span data-stu-id="21981-151">You may want to use a work date if you have many transactions with a date other than today's date.</span></span>

<span data-ttu-id="21981-152">См. также [Изменение базовых настроек, таких как рабочая дата](ui-change-basic-settings.md#work-date)</span><span class="sxs-lookup"><span data-stu-id="21981-152">See also [Changing Basic Settings, such as the Work Date](ui-change-basic-settings.md#work-date)</span></span>

### <a name="closing-date"></a><span data-ttu-id="21981-153">Дата закрытия</span><span class="sxs-lookup"><span data-stu-id="21981-153">Closing Date</span></span>
<span data-ttu-id="21981-154">При закрытии финансового года можно использовать даты в специальном формате, указывающем на закрытие.</span><span class="sxs-lookup"><span data-stu-id="21981-154">When you close a fiscal year, you can use closing dates to indicate that an entry is a closing entry.</span></span> <span data-ttu-id="21981-155">Дата закрытия технически лежит между двумя календарными датами, например между 31 декабря и 1 января.</span><span class="sxs-lookup"><span data-stu-id="21981-155">A closing date technically is between two dates, for example between Dec 31 and Jan 1.</span></span>

<span data-ttu-id="21981-156">Чтобы указать, что дата является датой закрытия, следует непосредственно перед датой ввести букву `C`, например `C123101`.</span><span class="sxs-lookup"><span data-stu-id="21981-156">To specify that a date is a closing date, put `C` just before the date, such as `C123101`.</span></span> <span data-ttu-id="21981-157">Это можно использовать в сочетании со всеми схемами даты.</span><span class="sxs-lookup"><span data-stu-id="21981-157">This can be used in combination with all the date patterns.</span></span>

### <a name="examples"></a><span data-ttu-id="21981-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="21981-158">Examples</span></span>
<span data-ttu-id="21981-159">В следующей таблице содержится несколько примеров дат с использованием всех форматов.</span><span class="sxs-lookup"><span data-stu-id="21981-159">The following table contains examples of dates using all the formats.</span></span> <span data-ttu-id="21981-160">Предполагаются настройки региона, которые форматируют даты в соответствии со следующими параметрами: **год.месяц.дата.**, неделя начинается в понедельник и английский язык.</span><span class="sxs-lookup"><span data-stu-id="21981-160">It assumes region settings that format dates according to: **year.month.day.**, a week starting on Monday, and the English language.</span></span>

|<span data-ttu-id="21981-161">**Формат ввода**</span><span class="sxs-lookup"><span data-stu-id="21981-161">**Entry**</span></span>      |<span data-ttu-id="21981-162">**Интерпретация**</span><span class="sxs-lookup"><span data-stu-id="21981-162">**Interpretation**</span></span>      |
|---------------|------------------------|
|`2018.12.31.`|<span data-ttu-id="21981-163">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-163">2018.12.31.</span></span>|
|`181231`|<span data-ttu-id="21981-164">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-164">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="21981-165">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-165">2018.12.31.</span></span>|
|`18.12.31.`|<span data-ttu-id="21981-166">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-166">2018.12.31.</span></span>|
|`20181231`|<span data-ttu-id="21981-167">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-167">2018.12.31.</span></span>|
|`18/12,31`|<span data-ttu-id="21981-168">2018.12.31.</span><span class="sxs-lookup"><span data-stu-id="21981-168">2018.12.31.</span></span>|
|`11`|<span data-ttu-id="21981-169">год рабочей даты.месяц рабочей даты.11.</span><span class="sxs-lookup"><span data-stu-id="21981-169">work date year.work date month.11.</span></span>|
|`1112`|<span data-ttu-id="21981-170">год рабочей даты.11.12.</span><span class="sxs-lookup"><span data-stu-id="21981-170">work date year.11.12.</span></span>|
|<span data-ttu-id="21981-171">`t` или `today`</span><span class="sxs-lookup"><span data-stu-id="21981-171">`t` or `today`</span></span>|<span data-ttu-id="21981-172">текущая дата</span><span class="sxs-lookup"><span data-stu-id="21981-172">today's date</span></span>|
|<span data-ttu-id="21981-173">`w` или `workdate`</span><span class="sxs-lookup"><span data-stu-id="21981-173">`w` or `workdate`</span></span>|<span data-ttu-id="21981-174">рабочая дата</span><span class="sxs-lookup"><span data-stu-id="21981-174">the working date</span></span>|
|<span data-ttu-id="21981-175">`m` или `Monday`</span><span class="sxs-lookup"><span data-stu-id="21981-175">`m` or `Monday`</span></span>|<span data-ttu-id="21981-176">Понедельник недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-176">Monday of the work date week</span></span>|
|<span data-ttu-id="21981-177">`tu` или `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="21981-177">`tu` or `Tuesday`</span></span>|<span data-ttu-id="21981-178">Вторник недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-178">Tuesday of the work date week</span></span>|
|<span data-ttu-id="21981-179">`sa` или `Saturday`</span><span class="sxs-lookup"><span data-stu-id="21981-179">`sa` or `Saturday`</span></span>|<span data-ttu-id="21981-180">Суббота недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-180">Saturday of the work date week</span></span>|
|<span data-ttu-id="21981-181">`s` или `Sunday`</span><span class="sxs-lookup"><span data-stu-id="21981-181">`s` or `Sunday`</span></span>|<span data-ttu-id="21981-182">Воскресенье недели рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-182">Sunday of the work date week</span></span>|
|`t23`|<span data-ttu-id="21981-183">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-183">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="21981-184">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-184">Tuesday of week 23 of the work date year</span></span>|
|`t-1`|<span data-ttu-id="21981-185">Вторник недели 1 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-185">Tuesday of week 1 of the work date year</span></span>|

##  <a name="BKMK_SettingDateRanges"></a> <span data-ttu-id="21981-186">Диапазоны дат</span><span class="sxs-lookup"><span data-stu-id="21981-186">Setting Ranges</span></span>
<span data-ttu-id="21981-187">В списках, итогах и отчетах можно установить фильтры по датам, времени и дате и времени, содержащие начальное значение и, необязательно, конечное значение для отображения только данных, содержащихся в данном диапазоне.</span><span class="sxs-lookup"><span data-stu-id="21981-187">On lists, totals and reports, you can set filters on dates, times and datetimes containing a start value and optionally an end value to display only the data contained in that range.</span></span> <span data-ttu-id="21981-188">При установке диапазонов дат следует руководствоваться стандартными правилами.</span><span class="sxs-lookup"><span data-stu-id="21981-188">The standard rules apply to the way you set date ranges.</span></span>

|<span data-ttu-id="21981-189">**Значение**</span><span class="sxs-lookup"><span data-stu-id="21981-189">**Meaning**</span></span>|<span data-ttu-id="21981-190">**Пример выражения (дата)**</span><span class="sxs-lookup"><span data-stu-id="21981-190">**Sample expression (Date)**</span></span>|<span data-ttu-id="21981-191">**Данные, включенные в фильтр**</span><span class="sxs-lookup"><span data-stu-id="21981-191">**Data included in the filter**</span></span>|
|-----------|---------------------|--------------------|
|<span data-ttu-id="21981-192">Интервал</span><span class="sxs-lookup"><span data-stu-id="21981-192">Interval</span></span>|<span data-ttu-id="21981-193">`12 15 00..01 15 01`  \n`..12 15 00`</span><span class="sxs-lookup"><span data-stu-id="21981-193">`12 15 00..01 15 01`  \n`..12 15 00`</span></span>|<span data-ttu-id="21981-194">Записи датами, попадающими в период с 15.12.00 по 15.01.01 включительно.</span><span class="sxs-lookup"><span data-stu-id="21981-194">Records with dates between and including 12 15 00 and 01 15 01.</span></span>  <span data-ttu-id="21981-195">\nЗаписи с датами 15.12.00 или ранее.</span><span class="sxs-lookup"><span data-stu-id="21981-195">\nRecords with dates of 12 15 00 or earlier.</span></span>|
|<span data-ttu-id="21981-196">Либо/или</span><span class="sxs-lookup"><span data-stu-id="21981-196">Either/or</span></span>|<span data-ttu-id="21981-197">\`12 15 00</span><span class="sxs-lookup"><span data-stu-id="21981-197">\`12 15 00</span></span>|<span data-ttu-id="21981-198">12 16 00\`</span><span class="sxs-lookup"><span data-stu-id="21981-198">12 16 00\`</span></span>|<span data-ttu-id="21981-199">Записи с датами 15.12.00 или 16.12.00.</span><span class="sxs-lookup"><span data-stu-id="21981-199">Records with dates of either 12 15 00 or 12 16 00.</span></span> <span data-ttu-id="21981-200">Если существуют записи с датами для обоих дней, все они будут выведены на экран.</span><span class="sxs-lookup"><span data-stu-id="21981-200">If there are records with dates on both days, they will all be displayed.</span></span>|
|<span data-ttu-id="21981-201">Комбинация</span><span class="sxs-lookup"><span data-stu-id="21981-201">Combination</span></span>|<span data-ttu-id="21981-202">\`12 15 00</span><span class="sxs-lookup"><span data-stu-id="21981-202">\`12 15 00</span></span>|<span data-ttu-id="21981-203">12 01 00..12 10 00`  \n`..12 14 00</span><span class="sxs-lookup"><span data-stu-id="21981-203">12 01 00..12 10 00`  \n`..12 14 00</span></span>|<span data-ttu-id="21981-204">12 30 00..\`</span><span class="sxs-lookup"><span data-stu-id="21981-204">12 30 00..\`</span></span>|<span data-ttu-id="21981-205">Записи с датами 15.12.00 или за период с 01.12.00 по 10.12.00 включительно.</span><span class="sxs-lookup"><span data-stu-id="21981-205">Records with dates of 12 15 00 or on dates between and including 12 01 00 and 12 10 00.</span></span>  <span data-ttu-id="21981-206">\nЗаписи с датами не позднее 14.12.00 или не ранее 30.12.00. То есть все записи за исключением тех, даты отклика которых попадают в период с 15.12.00 по 29.12.00 включительно.</span><span class="sxs-lookup"><span data-stu-id="21981-206">\nRecords with dates of 12 14 00 or earlier, or dates of 12 30 00 or later, that is, all records except those with dates between and including 12 15 00 and 12 29 00.</span></span>|

<span data-ttu-id="21981-207">Можно использовать любые допустимые форматы в фильтрах диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="21981-207">You can use any of the valid formats in date range filters.</span></span> <span data-ttu-id="21981-208">Например, `mon14 3..t 4p` при применении к полю даты и времени дает фильтр с 3 утра в понедельник в неделю 14 года текущей рабочей даты, включительно, до 16:00 сегодня, включительно.</span><span class="sxs-lookup"><span data-stu-id="21981-208">For example, `mon14 3..t 4p` applied on a datetime field results in a filter from 3 AM on Monday in week 14 of the current work date year, inclusive, until today at 4PM, inclusive.</span></span>


## <a name="using-date-formulas"></a><span data-ttu-id="21981-209">Использование формул дат</span><span class="sxs-lookup"><span data-stu-id="21981-209">Using Date Formulas</span></span>
<span data-ttu-id="21981-210">Формула даты — это краткая сокращенная буквенно-числовая комбинация, задающая способ вычисления дат.</span><span class="sxs-lookup"><span data-stu-id="21981-210">A date formula is a short, abbreviated combination of letters and numbers that specifies how to calculate dates.</span></span> <span data-ttu-id="21981-211">Можно вводить формулы дат в различных вычисляемых полях расчета даты или фильтрах.</span><span class="sxs-lookup"><span data-stu-id="21981-211">You can enter date formulas in various date calculation fields or filters.</span></span>

> [!NOTE]
>  <span data-ttu-id="21981-212">Во всех полях формул данных один день включается автоматически для покрытия сегодняшнего дня как дня начала периода.</span><span class="sxs-lookup"><span data-stu-id="21981-212">In all data formula fields, one day is automatically included to cover today as the day when the period starts.</span></span> <span data-ttu-id="21981-213">Соответственно, например, если ввести `1W`, то период фактически будет равен восьми дням, поскольку в него включается сегодняшний.</span><span class="sxs-lookup"><span data-stu-id="21981-213">Accordingly, for example, if you enter `1W`, then the period is actually eight days because today is included.</span></span> <span data-ttu-id="21981-214">Чтобы указать период, равный 7 дням \(одной реальной неделе\), включая дату начала периода, следует ввести `6D` или `1W-1D`.</span><span class="sxs-lookup"><span data-stu-id="21981-214">To specify a period of seven days \(one true week\) including the period starting date, then you must enter `6D` or `1W-1D`.</span></span>

<span data-ttu-id="21981-215">Примеры использования формул дат:</span><span class="sxs-lookup"><span data-stu-id="21981-215">Here are some examples of how date formulas can be used:</span></span>

-   <span data-ttu-id="21981-216">Формула даты в поле частоты повторения в типовом журнале определяет периодичность учета операции в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="21981-216">The date formula in the recurring frequency field in recurring journals determines how often the entry on the journal line will be posted.</span></span>

-   <span data-ttu-id="21981-217">Формула даты в поле **Период отсрочки** того или иного уровня напоминания определяет период от срока оплаты \(или от даты предыдущего напоминания\) до создания напоминания.</span><span class="sxs-lookup"><span data-stu-id="21981-217">The date formula in the **Grace Period** field for a specified reminder level determines the period of time that must pass from the due date \(or from the date of the previous reminder\) before a reminder will be created.</span></span>

-   <span data-ttu-id="21981-218">Формула даты в поле **Расчет срока оплаты** определяет способ расчета даты оплаты в напоминании.</span><span class="sxs-lookup"><span data-stu-id="21981-218">The date formula in the **Due Date Calculation** field determines how to calculate the due date on the reminder.</span></span>

<span data-ttu-id="21981-219">Формула даты может содержать до 20 знаков, как цифр, так и букв.</span><span class="sxs-lookup"><span data-stu-id="21981-219">The date formula can contain a maximum of 20 characters, both numbers and letters.</span></span> <span data-ttu-id="21981-220">В этих формулах можно использовать следующие сокращения календарных единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="21981-220">You can use the following letters, which are abbreviations for calendar units.</span></span>

|  <span data-ttu-id="21981-221">Буква</span><span class="sxs-lookup"><span data-stu-id="21981-221">Letter</span></span>  |  <span data-ttu-id="21981-222">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-222">Meaning</span></span>  |
|----------|----------------------|
|`C`|<span data-ttu-id="21981-223">Текущая</span><span class="sxs-lookup"><span data-stu-id="21981-223">Current</span></span>|
|`D`|<span data-ttu-id="21981-224">День\(дни\)</span><span class="sxs-lookup"><span data-stu-id="21981-224">Day\(s\)</span></span>|
|`W`|<span data-ttu-id="21981-225">Неделя\(недели\)</span><span class="sxs-lookup"><span data-stu-id="21981-225">Week\(s\)</span></span>|
|`M`|<span data-ttu-id="21981-226">Месяц\(месяцы\)</span><span class="sxs-lookup"><span data-stu-id="21981-226">Month\(s\)</span></span>|
|`Q`|<span data-ttu-id="21981-227">Квартал\(кварталы\)</span><span class="sxs-lookup"><span data-stu-id="21981-227">Quarter\(s\)</span></span>|
|`Y`|<span data-ttu-id="21981-228">Год\(года\)</span><span class="sxs-lookup"><span data-stu-id="21981-228">Year\(s\)</span></span>|

<span data-ttu-id="21981-229">Составить формулу даты можно тремя способами.</span><span class="sxs-lookup"><span data-stu-id="21981-229">You can construct a date formula in three ways.</span></span>

<span data-ttu-id="21981-230">В следующем примере описывается способ использования `C` в качестве текущей даты и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="21981-230">The following example shows how to use `C`, for current, and a time unit.</span></span>

|  <span data-ttu-id="21981-231">Выражение</span><span class="sxs-lookup"><span data-stu-id="21981-231">Expression</span></span>  |  <span data-ttu-id="21981-232">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-232">Meaning</span></span>  |
|--------------|-----------|
|`CW`|<span data-ttu-id="21981-233">текущая неделя;</span><span class="sxs-lookup"><span data-stu-id="21981-233">Current week</span></span>|
|`CM`|<span data-ttu-id="21981-234">текущий месяц.</span><span class="sxs-lookup"><span data-stu-id="21981-234">Current month</span></span>|

<span data-ttu-id="21981-235">В следующем примере описывается способ использования числа и единицы измерения времени.</span><span class="sxs-lookup"><span data-stu-id="21981-235">The following example shows how to use a number and a time unit.</span></span> <span data-ttu-id="21981-236">Число не может быть больше 9999.</span><span class="sxs-lookup"><span data-stu-id="21981-236">A number cannot be larger than 9999.</span></span>

|  <span data-ttu-id="21981-237">Выражение</span><span class="sxs-lookup"><span data-stu-id="21981-237">Expression</span></span>  |  <span data-ttu-id="21981-238">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-238">Meaning</span></span>  |
|--------------|-----------|
|`10D`|<span data-ttu-id="21981-239">через 10 дней после текущей даты;</span><span class="sxs-lookup"><span data-stu-id="21981-239">10 days from today</span></span>|
|`2W`|<span data-ttu-id="21981-240">через 2 недели после текущей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-240">2 weeks from today</span></span>|

<span data-ttu-id="21981-241">В следующем примере описывается способ использования единицы измерения времени и числа.</span><span class="sxs-lookup"><span data-stu-id="21981-241">The following example shows how to use a time unit and a number.</span></span>

|  <span data-ttu-id="21981-242">Выражение</span><span class="sxs-lookup"><span data-stu-id="21981-242">Expression</span></span>  |  <span data-ttu-id="21981-243">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-243">Meaning</span></span>  |
|--------------|-----------|
|`D10`|<span data-ttu-id="21981-244">следующий 10-й день месяца;</span><span class="sxs-lookup"><span data-stu-id="21981-244">The next 10th day of a month</span></span>|
|`WD4`|<span data-ttu-id="21981-245">следующий 4-й день недели \(четверг\).</span><span class="sxs-lookup"><span data-stu-id="21981-245">The next 4th day of a week \(Thursday\)</span></span>|

<span data-ttu-id="21981-246">В следующем примере описывается способ комбинирования таких трех форм при необходимости.</span><span class="sxs-lookup"><span data-stu-id="21981-246">The following example shows how you can combine these three forms as needed.</span></span>

|  <span data-ttu-id="21981-247">Выражение</span><span class="sxs-lookup"><span data-stu-id="21981-247">Expression</span></span>  |  <span data-ttu-id="21981-248">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-248">Meaning</span></span>  |
|--------------|-----------|
|`CM+10D`|<span data-ttu-id="21981-249">текущий месяц \+ 10 дней</span><span class="sxs-lookup"><span data-stu-id="21981-249">Current month \+ 10 days</span></span>|

<span data-ttu-id="21981-250">В следующем примере показано, как использовать знак минуса для указания прошедшей даты.</span><span class="sxs-lookup"><span data-stu-id="21981-250">The following example shows how you can use a minus sign to indicate a date in the past.</span></span>

|  <span data-ttu-id="21981-251">Выражение</span><span class="sxs-lookup"><span data-stu-id="21981-251">Expression</span></span>  |  <span data-ttu-id="21981-252">Значение</span><span class="sxs-lookup"><span data-stu-id="21981-252">Meaning</span></span>  |
|--------------|-----------|
|`-1Y`|<span data-ttu-id="21981-253">1 год назад.</span><span class="sxs-lookup"><span data-stu-id="21981-253">1 year ago from today</span></span>|

> [!IMPORTANT]
>  <span data-ttu-id="21981-254">Если на складе используется базовый календарь, то вводимая в это поле формула даты, например **Время отгрузки**, интерпретирована в соответствии с рабочими днями календаря.</span><span class="sxs-lookup"><span data-stu-id="21981-254">If the location uses a base calendar, then the date formula that you enter in, for example, the **Shipping Time** field is interpreted according to the calendar working days.</span></span> <span data-ttu-id="21981-255">Например, `1W` означает семь рабочих дней.</span><span class="sxs-lookup"><span data-stu-id="21981-255">For example, `1W`  means seven working days.</span></span>
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

Note that we have used the US date format MMDDYY here. As [!INCLUDE[d365fin](includes/d365fin_md.md)] becomes available in other markets, you'll be able to use the formats that you are used to.

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

## <a name="entering-times"></a><span data-ttu-id="21981-256">Ввод времени</span><span class="sxs-lookup"><span data-stu-id="21981-256">Entering Times</span></span>
<span data-ttu-id="21981-257">При вводе времени можно вставить любые разделители, отличные от пробелов, которые необходимы между единицами измерения, но при использовании двух цифр для каждой единицы измерения вплоть до миллисекунд это не является необходимым.</span><span class="sxs-lookup"><span data-stu-id="21981-257">When you enter times, you can insert any non-space separators that you want between the units, but if you use double digits for each unit up to milliseconds, then it is not required.</span></span>

<span data-ttu-id="21981-258">Следует только записать наибольшую необходимую единицу измерения; остатки будет установлен на нуль.</span><span class="sxs-lookup"><span data-stu-id="21981-258">You only have to write the largest units that you require; the rest will be set to zero.</span></span> <span data-ttu-id="21981-259">Также можно не указывать никакого индикатора AM/PM.</span><span class="sxs-lookup"><span data-stu-id="21981-259">You can also leave out any AM/PM indicator.</span></span>

<span data-ttu-id="21981-260">В следующей таблице представлены способы ввода времени и их интерпретация.</span><span class="sxs-lookup"><span data-stu-id="21981-260">The following table lists the various ways in which times can be entered and how they are interpreted.</span></span> <span data-ttu-id="21981-261">Предполагаются настройки региона, которые форматируют время в соответствии со следующими параметрами: **Часы:Минуты:Секунды.Миллисекунды.**</span><span class="sxs-lookup"><span data-stu-id="21981-261">It assumes region settings that format times according to: **Hours:Minutes:Seconds.Milliseconds.**</span></span> <span data-ttu-id="21981-262">и используются показатели до и после полудня "AM" и "PM", соответственно.</span><span class="sxs-lookup"><span data-stu-id="21981-262">and use the AM and PM indicators of 'AM' and 'PM', respectively.</span></span>

|<span data-ttu-id="21981-263">**Формат ввода**</span><span class="sxs-lookup"><span data-stu-id="21981-263">**Entry**</span></span>      |<span data-ttu-id="21981-264">**Интерпретация**</span><span class="sxs-lookup"><span data-stu-id="21981-264">**Interpretation**</span></span>      |
|---------------|------------------------|
|`05:23:17`|<span data-ttu-id="21981-265">05:23:17</span><span class="sxs-lookup"><span data-stu-id="21981-265">05:23:17</span></span>|
|`5`|<span data-ttu-id="21981-266">05:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-266">05:00:00</span></span>|
|`5AM`|<span data-ttu-id="21981-267">05:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-267">05:00:00</span></span>|
|`5P`|<span data-ttu-id="21981-268">17:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-268">17:00:00</span></span>|
|`12`|<span data-ttu-id="21981-269">12:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-269">12:00:00</span></span>|
|`12A`|<span data-ttu-id="21981-270">00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-270">00:00:00</span></span>|
|`12P`|<span data-ttu-id="21981-271">12:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-271">12:00:00</span></span>|
|`17`|<span data-ttu-id="21981-272">17:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-272">17:00:00</span></span>|
|`5:30`|<span data-ttu-id="21981-273">05:30:00</span><span class="sxs-lookup"><span data-stu-id="21981-273">05:30:00</span></span>|
|`0530`|<span data-ttu-id="21981-274">05:30:00</span><span class="sxs-lookup"><span data-stu-id="21981-274">05:30:00</span></span>|
|`5:30:5`|<span data-ttu-id="21981-275">05:30:05</span><span class="sxs-lookup"><span data-stu-id="21981-275">05:30:05</span></span>|
|`053005`|<span data-ttu-id="21981-276">05:30:05</span><span class="sxs-lookup"><span data-stu-id="21981-276">05:30:05</span></span>|
|`5:30:5,50`|<span data-ttu-id="21981-277">05:30:05,5</span><span class="sxs-lookup"><span data-stu-id="21981-277">05:30:05.5</span></span>|
|`053005050`|<span data-ttu-id="21981-278">05:30:05.05</span><span class="sxs-lookup"><span data-stu-id="21981-278">05:30:05.05</span></span>|

<span data-ttu-id="21981-279">Необходимо помнить, что миллисекунды интерпретируются как десятичная нотация.</span><span class="sxs-lookup"><span data-stu-id="21981-279">You should be aware that milliseconds are interpreted as decimal notation.</span></span> <span data-ttu-id="21981-280">Поэтому, например, `3`, `30` и `300` все означают 300 миллисекунд, а `03` означает `30` и `003` означает 3 миллисекунды.</span><span class="sxs-lookup"><span data-stu-id="21981-280">So, for example, `3`, `30`, and `300` all mean 300 milliseconds, while `03` means `30` and `003` means 3 milliseconds.</span></span>

<span data-ttu-id="21981-281">Нельзя использовать `24:00` для полночи или использовать любое значение, большее 24:00.</span><span class="sxs-lookup"><span data-stu-id="21981-281">You cannot use `24:00` to mean midnight, or use any value greater than 24:00.</span></span>

<span data-ttu-id="21981-282">Слово "время" на языке, используемом [!INCLUDE[d365fin](includes/d365fin_long_md.md)], будет оценено как текущее время на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="21981-282">The word for 'time' in the language used by [!INCLUDE[d365fin](includes/d365fin_long_md.md)] will be evaluated to the current time on your computer or mobile device.</span></span> <span data-ttu-id="21981-283">Можно ввести любую часть слова, начиная с начала, например `t` или `TIM`.</span><span class="sxs-lookup"><span data-stu-id="21981-283">You can enter any part of the word, starting from the beginning, such as `t` or `TIM`.</span></span>

## <a name="entering-combined-dates-and-times"></a><span data-ttu-id="21981-284">Ввода комбинированных дат и времени</span><span class="sxs-lookup"><span data-stu-id="21981-284">Entering combined Dates and Times</span></span>
<span data-ttu-id="21981-285">При вводе даты и времени, то есть даты и времени в одном поле, необходимо оставлять пробел между датой и временем.</span><span class="sxs-lookup"><span data-stu-id="21981-285">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="21981-286">Часть даты может содержать только пробелы в форме официального разделителя дат настроек региона.</span><span class="sxs-lookup"><span data-stu-id="21981-286">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="21981-287">Время может содержать пробелы вокруг индикатора AM/PM.</span><span class="sxs-lookup"><span data-stu-id="21981-287">The time can contain spaces around the AM/PM indicator.</span></span>

<span data-ttu-id="21981-288">Можно также ввести только дату в поле даты и времени, но невозможно ввести только время.</span><span class="sxs-lookup"><span data-stu-id="21981-288">It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.</span></span>

<span data-ttu-id="21981-289">В следующей таблице приведены некоторые примеры комбинаций даты и времени.</span><span class="sxs-lookup"><span data-stu-id="21981-289">The following table lists some examples of date/time combinations.</span></span> <span data-ttu-id="21981-290">Настройки региона в примерах отображают даты в формате день\-месяц\-год, с использованием обозначений AM/PM, на английском языке и воскресеньем, как начало недели.</span><span class="sxs-lookup"><span data-stu-id="21981-290">The region settings in the examples displays dates in the day\-month\-year format, using AM/PM designators, English language, and Sunday as the start of the week.</span></span>

|<span data-ttu-id="21981-291">**Формат ввода**</span><span class="sxs-lookup"><span data-stu-id="21981-291">**Entry**</span></span>      |<span data-ttu-id="21981-292">**Интерпретация**</span><span class="sxs-lookup"><span data-stu-id="21981-292">**Interpretation**</span></span>      |
|---------------|------------------------|
|`08-01-2016 05:48:12 PM`|<span data-ttu-id="21981-293">08\-01\-2016 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="21981-293">08\-01\-2016 05:48:12 PM</span></span>|
|`131202 132455`|<span data-ttu-id="21981-294">13\-12\-2002 13:24:55</span><span class="sxs-lookup"><span data-stu-id="21981-294">13\-12\-2002 13:24:55</span></span>|
|`1-12-02 10`|<span data-ttu-id="21981-295">01\-12\-2002 10:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-295">01\-12\-2002 10:00:00</span></span>|
|`1.12.02 5`|<span data-ttu-id="21981-296">01\-12\-2002 05:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-296">01\-12\-2002 05:00:00</span></span>|
|`1.12.02`|<span data-ttu-id="21981-297">01\-12\-2002 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-297">01\-12\-2002 00:00:00</span></span>|
|`11 12`|<span data-ttu-id="21981-298">11\-месяц рабочей даты\-год рабочей даты 12:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-298">11\-work date month\-work date year 12:00:00</span></span>|
|`1112 12`|<span data-ttu-id="21981-299">11\-12\-год рабочей даты 12:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-299">11\-12\-work date year 12:00:00</span></span>|
|<span data-ttu-id="21981-300">`t` или `today`</span><span class="sxs-lookup"><span data-stu-id="21981-300">`t` or `today`</span></span>|<span data-ttu-id="21981-301">текущая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-301">today's date 00:00:00</span></span>|
|`t 10:30`|<span data-ttu-id="21981-302">текущая дата, 10:30:00</span><span class="sxs-lookup"><span data-stu-id="21981-302">today's date 10:30:00</span></span>|
|`t 3:3:3`|<span data-ttu-id="21981-303">текущая дата, 03:03:03</span><span class="sxs-lookup"><span data-stu-id="21981-303">today's date 03:03:03</span></span>|
|<span data-ttu-id="21981-304">`w` или `workdate`</span><span class="sxs-lookup"><span data-stu-id="21981-304">`w` or `workdate`</span></span>|<span data-ttu-id="21981-305">рабочая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-305">the working date 00:00:00</span></span>|
|<span data-ttu-id="21981-306">`m` или `Monday`</span><span class="sxs-lookup"><span data-stu-id="21981-306">`m` or `Monday`</span></span>|<span data-ttu-id="21981-307">Понедельник недели рабочей даты 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-307">Monday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="21981-308">`tu` или `Tuesday`</span><span class="sxs-lookup"><span data-stu-id="21981-308">`tu` or `Tuesday`</span></span>|<span data-ttu-id="21981-309">Вторник недели рабочей даты 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-309">Tuesday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="21981-310">`sa` или `Saturday`</span><span class="sxs-lookup"><span data-stu-id="21981-310">`sa` or `Saturday`</span></span>|<span data-ttu-id="21981-311">Суббота недели рабочей даты 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-311">Saturday of the work date week 00:00:00</span></span>|
|<span data-ttu-id="21981-312">`s` или `Sunday`</span><span class="sxs-lookup"><span data-stu-id="21981-312">`s` or `Sunday`</span></span>|<span data-ttu-id="21981-313">Воскресенье недели рабочей даты 00:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-313">Sunday of the work date week 00:00:00</span></span>|
|`tu 10:30`|<span data-ttu-id="21981-314">Вторник недели рабочей даты 10:30:00</span><span class="sxs-lookup"><span data-stu-id="21981-314">Tuesday of the work date week 10:30:00</span></span>|
|`tu 3:3:3`|<span data-ttu-id="21981-315">Вторник недели рабочей даты 03:03:03</span><span class="sxs-lookup"><span data-stu-id="21981-315">Tuesday of the work date week 03:03:03</span></span>|
|`t23 t`|<span data-ttu-id="21981-316">Вторник недели 23 года рабочей даты, текущее время дня</span><span class="sxs-lookup"><span data-stu-id="21981-316">Tuesday of week 23 of the work date year, current time of day</span></span>|
|`t23`|<span data-ttu-id="21981-317">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-317">Tuesday of week 23 of the work date year</span></span>|
|`t 23`|<span data-ttu-id="21981-318">Сегодня 23:00:00</span><span class="sxs-lookup"><span data-stu-id="21981-318">Today 23:00:00</span></span>|
|`t-1`|<span data-ttu-id="21981-319">Вторник недели 1 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="21981-319">Tuesday of week 1 of the work date year</span></span>|

## <a name="entering-duration"></a><span data-ttu-id="21981-320">Ввод продолжительности</span><span class="sxs-lookup"><span data-stu-id="21981-320">Entering Duration</span></span>
<span data-ttu-id="21981-321">Некоторые поля в приложении представляют длительность или прошедшее время, а не определенную дату или время.</span><span class="sxs-lookup"><span data-stu-id="21981-321">Some fields in the application represent a duration, or amount of elapsed time, instead of a specific date or time.</span></span> <span data-ttu-id="21981-322">Длительность вводится в виде числа, за которым следует единица измерения.</span><span class="sxs-lookup"><span data-stu-id="21981-322">You enter a duration as a number followed by its unit of measure.</span></span>

<span data-ttu-id="21981-323">Примеры:</span><span class="sxs-lookup"><span data-stu-id="21981-323">Here are some examples.</span></span>

|<span data-ttu-id="21981-324">**Длительность**</span><span class="sxs-lookup"><span data-stu-id="21981-324">**Duration**</span></span>|<span data-ttu-id="21981-325">**Единица измерения**</span><span class="sxs-lookup"><span data-stu-id="21981-325">**Unit of measure**</span></span>|
|------------|-------------------|
|`2h`|<span data-ttu-id="21981-326">2 часа</span><span class="sxs-lookup"><span data-stu-id="21981-326">2 hrs</span></span>|
|`6h 30 m`|<span data-ttu-id="21981-327">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="21981-327">6 hrs 30 mins</span></span>|
|`6.5h`|<span data-ttu-id="21981-328">6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="21981-328">6 hrs 30 mins</span></span>|
|`90m`|<span data-ttu-id="21981-329">1 час 30 минут</span><span class="sxs-lookup"><span data-stu-id="21981-329">1 hr 30 mins</span></span>|
|`2d 6h 30m`|<span data-ttu-id="21981-330">2 дня 6 часов 30 минут</span><span class="sxs-lookup"><span data-stu-id="21981-330">2 days 6 hrs 30 mins</span></span>|
|`2d 6h 30m 56s 600ms`|<span data-ttu-id="21981-331">2 дня 6 часов 30 минут 56 секунд 600 миллисекунд</span><span class="sxs-lookup"><span data-stu-id="21981-331">2 days 6 hrs 30 mins 56 secs 600 msecs</span></span>|

<span data-ttu-id="21981-332">Можно также ввести число, которое будет автоматически преобразовано во временной интервал.</span><span class="sxs-lookup"><span data-stu-id="21981-332">You can also enter a number, which will be automatically converted to a duration.</span></span> <span data-ttu-id="21981-333">При этом по умолчанию используется единица измерения, указанная в поле «Длительность».</span><span class="sxs-lookup"><span data-stu-id="21981-333">The number you enter is converted according to the default unit of measure that has been specified for the duration field.</span></span>

<span data-ttu-id="21981-334">Чтобы узнать, какая единица измерения указана в поле "Длительность", введите любое число и посмотрите, в какую единицу измерения оно преобразуется.</span><span class="sxs-lookup"><span data-stu-id="21981-334">To see what unit of measure is being used in a duration field, enter a number and see which unit of measure it is converted to.</span></span>

<span data-ttu-id="21981-335">Например, если по умолчанию используются часы, число `5` будет преобразовано в 5 часов.</span><span class="sxs-lookup"><span data-stu-id="21981-335">For example, if the unit of measure is hours, the number `5` is converted to 5 hrs.</span></span>


## <a name="see-also"></a><span data-ttu-id="21981-336">См. также</span><span class="sxs-lookup"><span data-stu-id="21981-336">See Also</span></span>
<span data-ttu-id="21981-337">[Работа с [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21981-337">[Working with [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="21981-338">Расчет даты для покупок</span><span class="sxs-lookup"><span data-stu-id="21981-338">Date Calculation for Purchases</span></span>](purchasing-date-calculation-for-purchases.md)  
[<span data-ttu-id="21981-339">Ввод критериев в фильтрах</span><span class="sxs-lookup"><span data-stu-id="21981-339">Entering Criteria in Filters </span></span>](ui-enter-criteria-filters.md)  

