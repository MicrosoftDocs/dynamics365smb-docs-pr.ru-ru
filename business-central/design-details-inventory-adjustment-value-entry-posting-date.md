---
title: Даты учета для операций стоимости
description: Узнайте, как пакетное задание "Коррекция себестоимости запасов" идентифицирует и назначает дату учета операциям стоимости, которые пакетное задание собирается создать.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: fe03f25c4f9024cb82b83af915e69073d2fdcf1e
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4751509"
---
# <a name="design-details-posting-date-on-adjustment-value-entry"></a><span data-ttu-id="b09a5-103">Подробности разработки: дата учета для операции коррекции стоимости</span><span class="sxs-lookup"><span data-stu-id="b09a5-103">Design Details: Posting Date on Adjustment Value Entry</span></span>
<span data-ttu-id="b09a5-104">Эта статья содержит рекомендации для пользователей функции оценки стоимости запасов в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="b09a5-104">This article provides guidance for users of the Inventory Costing functionality in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="b09a5-105">Конкретная статья предоставляет рекомендации по тому, как пакетное задание **Коррекция себестоимости запасов** идентифицирует и назначает дату учета операциям стоимости, которые пакетное задание собирается создать.</span><span class="sxs-lookup"><span data-stu-id="b09a5-105">The specific article is providing guidance in how the **Adjust Cost - Item Entries** batch job identifies and assigns a posting date to the value entries that the batch job is about to create.</span></span>  

<span data-ttu-id="b09a5-106">Сначала рассматривается концепция процесса, как пакетное задание идентифицирует и назначает дату учета для создаваемой операции стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-106">First the concept of the process is reviewed, how the batch job identifies and assigns the Posting Date to the Value Entry to be created.</span></span> <span data-ttu-id="b09a5-107">Далее приводятся несколько сценариев, с которыми время от времени сталкивается группа поддержки, а в конце приводится сводка концепций, используемых из версии 3.0.</span><span class="sxs-lookup"><span data-stu-id="b09a5-107">Thereafter there are some scenarios shared that we in the support team come across from time to time and finally there is a summary of the concepts used from version 3.0.</span></span>  

## <a name="the-concept"></a><span data-ttu-id="b09a5-108">Концепция</span><span class="sxs-lookup"><span data-stu-id="b09a5-108">The Concept</span></span>  
<span data-ttu-id="b09a5-109">С версии 5.0 пакетное задание **Коррекция себестоимости запасов** назначает дату учета создаваемой операции стоимости с использованием следующих шагов:</span><span class="sxs-lookup"><span data-stu-id="b09a5-109">From version 5.0, the **Adjust Cost – Item Entries** batch job assigns a posting date to the value entry it is about to create in the following steps:</span></span>  

1.  <span data-ttu-id="b09a5-110">Первоначально дата учета создаваемой операции совпадает с датой операции, которую она корректирует.</span><span class="sxs-lookup"><span data-stu-id="b09a5-110">Initially the Posting Date of the entry to be created is the same date as the entry it adjusts.</span></span>  

2.  <span data-ttu-id="b09a5-111">Дата учета проверяется относительно периодов учета запасов и/или настройки ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-111">The Posting Date is validated against Inventory Periods and/or General Ledger Setup.</span></span>  

3.  <span data-ttu-id="b09a5-112">Назначение даты учета: если исходная дата учета не находится в пределах допустимого диапазона дат учета, пакетное задание назначает допустимую дату учета из настройки ГК или периода учета запасов.</span><span class="sxs-lookup"><span data-stu-id="b09a5-112">Assignment of Posting Date; If the initial Posting Date is not within allowed posting date range the batch job will assign an allowed Posting Date from either General Ledger Setup or Inventory Period.</span></span> <span data-ttu-id="b09a5-113">Если определены как периоды учета, так и допустимые даты учета в настройке ГК, для операции коррекции стоимости назначается более поздняя из двух этих дат.</span><span class="sxs-lookup"><span data-stu-id="b09a5-113">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will be assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="b09a5-114">Дайте дополнительно рассмотрим этот процесс на практике.</span><span class="sxs-lookup"><span data-stu-id="b09a5-114">Let’s review this process more in practice.</span></span> <span data-ttu-id="b09a5-115">Предположим, что имеется операция книги товаров для продажи.</span><span class="sxs-lookup"><span data-stu-id="b09a5-115">Assume we have an Item Ledger Entry of Sale.</span></span> <span data-ttu-id="b09a5-116">Товар был отгружен 5 сентября 2013 г., и счет был выставлен на день позже.</span><span class="sxs-lookup"><span data-stu-id="b09a5-116">The item was shipped on September 5th, 2013 and it was invoiced the day after.</span></span>  

<span data-ttu-id="b09a5-117">![Состояние операций книги товаров в сценарии](media/helene/TechArticleAdjustcost1.png "Состояние операций книги товаров в сценарии")</span><span class="sxs-lookup"><span data-stu-id="b09a5-117">![State of item ledger entries in the scenario](media/helene/TechArticleAdjustcost1.png "State of item ledger entries in the scenario")</span></span>  

<span data-ttu-id="b09a5-118">Ниже первая операция стоимости (379) представляет отгрузку и содержит ту же самую дату учета, что и родительская операция книги товаров.</span><span class="sxs-lookup"><span data-stu-id="b09a5-118">Below, the first Value Entry (379) represents the shipment and carry the same Posting Date as the parent Item ledger Entry.</span></span>  

<span data-ttu-id="b09a5-119">Вторая операция стоимости (381) представляет счет.</span><span class="sxs-lookup"><span data-stu-id="b09a5-119">The second Value Entry (381) represents the invoice.</span></span>  

 <span data-ttu-id="b09a5-120">Третья операция стоимости (391) представляет собой коррекцию операции стоимости для выставления счета (381)</span><span class="sxs-lookup"><span data-stu-id="b09a5-120">The third Value Entry (391) is an Adjustment of the invoicing Value Entry (381)</span></span>  

 <span data-ttu-id="b09a5-121">![Состояние операций стоимости в сценарии](media/helene/TechArticleAdjustcost2.png "Состояние операций стоимости в сценарии")</span><span class="sxs-lookup"><span data-stu-id="b09a5-121">![State of value entries in the scenario](media/helene/TechArticleAdjustcost2.png "State of value entries in the scenario")</span></span>  

 <span data-ttu-id="b09a5-122">Шаг 1. Создаваемой операции коррекции стоимости назначается та же дата учета, что и у корректируемой операции, как иллюстрируется выше операцией стоимости 391.</span><span class="sxs-lookup"><span data-stu-id="b09a5-122">Step 1: Adjustment Value Entry to be created is assigned same Posting Date as the entry it adjusts, illustrated above by Value entry 391.</span></span>  

 <span data-ttu-id="b09a5-123">Шаг 2. Проверка первоначально назначенной даты учета.</span><span class="sxs-lookup"><span data-stu-id="b09a5-123">Step 2: Validation of initial assigned Posting Date.</span></span>  

<span data-ttu-id="b09a5-124">Пакетное задание **Коррекция себестоимости запасов** определяет, находится ли исходная дата учета операции коррекции стоимости в допустимом диапазоне дат учета на основе периодов учета запасов и/или настройки ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-124">The **Adjust Cost – Item Entries** batch job determines if the initial Posting Date of the Adjustment Value Entry is within allowed posting date range based upon Inventory Periods and/or General Ledger Setup.</span></span>  

 <span data-ttu-id="b09a5-125">Давайте рассмотрим указанную выше продажу, добавив настройку допустимых диапазонов дат учета.</span><span class="sxs-lookup"><span data-stu-id="b09a5-125">Let’s review the above mentioned Sale by adding setup of allowed posting date ranges.</span></span>  

 <span data-ttu-id="b09a5-126">Периоды учета запасов:</span><span class="sxs-lookup"><span data-stu-id="b09a5-126">Inventory Periods:</span></span>  

<span data-ttu-id="b09a5-127">![Периоды учета запасов в сценарии](media/helene/TechArticleAdjustcost3.png "Периоды учета запасов в сценарии")</span><span class="sxs-lookup"><span data-stu-id="b09a5-127">![Inventory periods in the scenario](media/helene/TechArticleAdjustcost3.png "Inventory periods in the scenario")</span></span>

 <span data-ttu-id="b09a5-128">Первая допустимая дата учета — это первый день первого открытого периода.</span><span class="sxs-lookup"><span data-stu-id="b09a5-128">First allowed posting date is the first day in the first open period.</span></span> <span data-ttu-id="b09a5-129">1 сентября 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-129">September 1st, 2013.</span></span>  

 <span data-ttu-id="b09a5-130">Настройка ГК:</span><span class="sxs-lookup"><span data-stu-id="b09a5-130">General Ledger Setup:</span></span>  

<span data-ttu-id="b09a5-131">![Настройка главной книги в сценарии](media/helene/TechArticleAdjustcost4.png "Настройка главной книги в сценарии")</span><span class="sxs-lookup"><span data-stu-id="b09a5-131">![G/L Setup in the scenario](media/helene/TechArticleAdjustcost4.png "G/L Setup in the scenario")</span></span>

 <span data-ttu-id="b09a5-132">Первая допустимая дата учета — это дата, указанная в поле "Разрешить учет с": 10-е сентября 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-132">First allowed posting date is the date stated in field Allow Posting From: September 10th, 2013.</span></span>  

 <span data-ttu-id="b09a5-133">Если определены как периоды учета, так и допустимые даты учета в настройке ГК, более поздняя дата из этих двух будет определять допустимый диапазон дат учета.</span><span class="sxs-lookup"><span data-stu-id="b09a5-133">If both Inventory Periods and allowed posting dates in General Ledger Setup are defined, the later date of the two will define the allowed posting date range.</span></span>  

 <span data-ttu-id="b09a5-134">Шаг 3. Назначение допустимой даты учета;</span><span class="sxs-lookup"><span data-stu-id="b09a5-134">Step 3: Assignment of an allowed posting date;</span></span>  

 <span data-ttu-id="b09a5-135">Исходная назначенная дата учета была 6-е сентября, как показано в шаге 1.</span><span class="sxs-lookup"><span data-stu-id="b09a5-135">The initial assigned Posting Date was September 6th as illustrated in step 1.</span></span> <span data-ttu-id="b09a5-136">Однако во 2-м шаге пакетное задание "Коррекция себестоимости запасов" определяет, что самая ранняя допустимая дата учета — это 10-е сентября, и поэтому назначает 10-е сентября операции коррекции стоимости ниже.</span><span class="sxs-lookup"><span data-stu-id="b09a5-136">However, in the 2nd step the Adjust Cost – Item entries batch job identifies that earliest allowed Posting Date is September 10th and thereby assigns September 10th to the Adjustment Value Entry, below.</span></span>  

 <span data-ttu-id="b09a5-137">![Состояние операций стоимости в сценарии 2](media/helene/TechArticleAdjustcost5.png "Состояние операций стоимости в сценарии 2")</span><span class="sxs-lookup"><span data-stu-id="b09a5-137">![State of value entries in the scenario 2](media/helene/TechArticleAdjustcost5.png "State of value entries in the scenario 2")</span></span>

 <span data-ttu-id="b09a5-138">Теперь мы рассмотрели концепцию назначения дат учета операциям стоимости, созданным пакетным заданием коррекции себестоимости запасов.</span><span class="sxs-lookup"><span data-stu-id="b09a5-138">We have now reviewed the concept for assigning Posting Dates to Value Entries created by the Adjust Cost - Item entries batch job.</span></span>  

 <span data-ttu-id="b09a5-139">Теперь давайте рассмотрим некоторые сценарии, с которыми мы в группе поддержки сталкиваемся время от времени в отношении назначенных дат учета в пакетном задании коррекции себестоимости запасов и соответствующих настроек.</span><span class="sxs-lookup"><span data-stu-id="b09a5-139">Let’s continue to review some scenarios that we in the support team comes across from time to time in relation to assigned Posting Dates in the Adjust Cost – Item entries batch job and related setups.</span></span>  

## <a name="scenarios"></a><span data-ttu-id="b09a5-140">Сценарии</span><span class="sxs-lookup"><span data-stu-id="b09a5-140">Scenarios</span></span>  

### <a name="scenario-i-posting-date-is-not-within-your-range-of-allowed-posting-dates"></a><span data-ttu-id="b09a5-141">Сценарий I. "Дата учета вне пределов разрешенного диапазона дат учета..."</span><span class="sxs-lookup"><span data-stu-id="b09a5-141">Scenario I: “Posting Date is not within your range of allowed posting dates…”</span></span>  
 <span data-ttu-id="b09a5-142">Это сценарий, в котором пользователь получает указанное выше сообщение об ошибке при запуске пакетного задания коррекции себестоимости запасов.</span><span class="sxs-lookup"><span data-stu-id="b09a5-142">This is a scenario where a user is experiencing mentioned error message when the Adjust Cost – Item entries batch job is run.</span></span>  

 <span data-ttu-id="b09a5-143">В предыдущем разделе, описывающем концепцию назначения дат учета, намерение пакетного задания коррекции себестоимости запасов заключается в создании операции стоимости с датой учета 10-го сентября.</span><span class="sxs-lookup"><span data-stu-id="b09a5-143">In the previous section, describing the concept of assigning posting dates, the intention of the Adjust Cost – Item entries batch job is to create a Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="b09a5-144">![Сообщение об ошибке о дате учета](media/helene/TechArticleAdjustcost6.png "Сообщение об ошибке о дате учета")</span><span class="sxs-lookup"><span data-stu-id="b09a5-144">![Error message about posting date](media/helene/TechArticleAdjustcost6.png "Error message about posting date")</span></span>

 <span data-ttu-id="b09a5-145">Мы отслеживаем настройку пользователя:</span><span class="sxs-lookup"><span data-stu-id="b09a5-145">We follow up on the User Setup:</span></span>  

<span data-ttu-id="b09a5-146">![Настройка разрешенных пользователем дат учета](media/helene/TechArticleAdjustcost7.png "Настройка разрешенных пользователем дат учета")</span><span class="sxs-lookup"><span data-stu-id="b09a5-146">![User's allowed posting dates setup](media/helene/TechArticleAdjustcost7.png "User's allowed posting dates setup")</span></span>

 <span data-ttu-id="b09a5-147">Пользователь в этом случае разрешил диапазон дат учета с 11-го сентября по 30-е сентября, и, таким образом, не разрешил учет операции коррекции стоимости с датой учета 10-е сентября.</span><span class="sxs-lookup"><span data-stu-id="b09a5-147">The user in this case has an allowed posting date range from September 11th to September 30th and is thereby not allowed to post the Adjustment Value Entry with Posting Date September 10th.</span></span>  

<span data-ttu-id="b09a5-148">![Обзор соответствующей настройки дат учета](media/helene/TechArticleAdjustcost8.png "Обзор соответствующей настройки дат учета")</span><span class="sxs-lookup"><span data-stu-id="b09a5-148">![Overview of involved posting date setup](media/helene/TechArticleAdjustcost8.png "Overview of involved posting date setup")</span></span>

 <span data-ttu-id="b09a5-149">В статье базы знаний [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) обсуждаются дополнительные сценарии, связанные с указанным сообщением об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b09a5-149">Knowledge Base article [952996](https://mbs2.microsoft.com/Knowledgebase/kbdisplay.aspx?WTNTZSMNWUKNTMMYXUPYZQPOUXNXSPSYOQQYYMLUQLOYYMWP) discusses additional scenarios related to mentioned error message.</span></span>  

### <a name="scenario-ii-posting-date-on-adjustment-value-entry-versus-posting-date-on-entry-causing-the-adjustment-such-as-revaluation-or-item-charge"></a><span data-ttu-id="b09a5-150">Сценарий II. Дата учета в операции коррекции стоимости и дата учета в операции, вызывающей коррекцию, такую как переоценка или товарная издержка.</span><span class="sxs-lookup"><span data-stu-id="b09a5-150">Scenario II: Posting Date on Adjustment Value Entry versus Posting Date on entry causing the adjustment such as Revaluation or Item charge.</span></span>  

### <a name="revaluation-scenario"></a><span data-ttu-id="b09a5-151">Сценарий переоценки:</span><span class="sxs-lookup"><span data-stu-id="b09a5-151">Revaluation scenario:</span></span>  
 <span data-ttu-id="b09a5-152">Предварительные требования:</span><span class="sxs-lookup"><span data-stu-id="b09a5-152">Prerequisites:</span></span>  

 <span data-ttu-id="b09a5-153">Настройка модуля "Запасы":</span><span class="sxs-lookup"><span data-stu-id="b09a5-153">Inventory setup:</span></span>  

-   <span data-ttu-id="b09a5-154">Автомат. учет себест. = Да</span><span class="sxs-lookup"><span data-stu-id="b09a5-154">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="b09a5-155">Автоматическая коррекция себестоимости = Всегда</span><span class="sxs-lookup"><span data-stu-id="b09a5-155">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="b09a5-156">Тип расчета средней себестоимости = товар</span><span class="sxs-lookup"><span data-stu-id="b09a5-156">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="b09a5-157">Период расчета средней себестоимости = День</span><span class="sxs-lookup"><span data-stu-id="b09a5-157">Average Cost Period=Day</span></span>  

 <span data-ttu-id="b09a5-158">Настройка ГК:</span><span class="sxs-lookup"><span data-stu-id="b09a5-158">General Ledger Setup:</span></span>  

-   <span data-ttu-id="b09a5-159">Разрешить учет с = 1-е января 2014 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-159">Allow Posting From = January 1st, 2014</span></span>  

-   <span data-ttu-id="b09a5-160">Разрешить учет по = пусто</span><span class="sxs-lookup"><span data-stu-id="b09a5-160">Allow Posting To = empty</span></span>  

 <span data-ttu-id="b09a5-161">Настройка пользователя:</span><span class="sxs-lookup"><span data-stu-id="b09a5-161">User Setup:</span></span>  

-   <span data-ttu-id="b09a5-162">Разрешить учет с = 1-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-162">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="b09a5-163">Разрешить учет по = пусто</span><span class="sxs-lookup"><span data-stu-id="b09a5-163">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="b09a5-164">Для проверки сценария</span><span class="sxs-lookup"><span data-stu-id="b09a5-164">To test the scenario</span></span>  

1.  <span data-ttu-id="b09a5-165">Создайте товар ТЕСТ:</span><span class="sxs-lookup"><span data-stu-id="b09a5-165">Create item TEST:</span></span>  

     <span data-ttu-id="b09a5-166">Базовая единица измерения = ШТ.</span><span class="sxs-lookup"><span data-stu-id="b09a5-166">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="b09a5-167">Метод учета себестоимости = Среднее</span><span class="sxs-lookup"><span data-stu-id="b09a5-167">Costing Method = Average</span></span>  

     <span data-ttu-id="b09a5-168">Выберите необязательные учетные группы.</span><span class="sxs-lookup"><span data-stu-id="b09a5-168">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="b09a5-169">Откройте журнал товаров, создайте и учтите строку следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b09a5-169">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="b09a5-170">Дата учета = 15-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-170">Posting Date = December 15th, 2013</span></span>  

     <span data-ttu-id="b09a5-171">Товар = ТЕСТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-171">Item = TEST</span></span>  

     <span data-ttu-id="b09a5-172">Тип операции = Покупка</span><span class="sxs-lookup"><span data-stu-id="b09a5-172">Entry Type = Purchase</span></span>  

     <span data-ttu-id="b09a5-173">Количество = 100</span><span class="sxs-lookup"><span data-stu-id="b09a5-173">Quantity = 100</span></span>  

     <span data-ttu-id="b09a5-174">Цена единицы = 10</span><span class="sxs-lookup"><span data-stu-id="b09a5-174">Unit Amount = 10</span></span>  

3.  <span data-ttu-id="b09a5-175">Откройте журнал товаров, создайте и учтите строку следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b09a5-175">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="b09a5-176">Дата = 20-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-176">Date = December 20th, 2013</span></span>  

     <span data-ttu-id="b09a5-177">Товар = ТЕСТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-177">Item = TEST</span></span>  

     <span data-ttu-id="b09a5-178">Тип операции = Расход</span><span class="sxs-lookup"><span data-stu-id="b09a5-178">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="b09a5-179">Количество = 2</span><span class="sxs-lookup"><span data-stu-id="b09a5-179">Quantity = 2</span></span>  

4.  <span data-ttu-id="b09a5-180">Откройте журнал товаров, создайте и учтите строку следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b09a5-180">Open Item Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="b09a5-181">Дата = 15-е января 2014 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-181">Date = January 15th, 2014</span></span>  

     <span data-ttu-id="b09a5-182">Товар = ТЕСТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-182">Item = TEST</span></span>  

     <span data-ttu-id="b09a5-183">Тип операции = Расход</span><span class="sxs-lookup"><span data-stu-id="b09a5-183">Entry Type = Negative Adjustment</span></span>  

     <span data-ttu-id="b09a5-184">Количество = 3</span><span class="sxs-lookup"><span data-stu-id="b09a5-184">Quantity = 3</span></span>  

5.  <span data-ttu-id="b09a5-185">Откройте журнал переоценки, создайте и учтите строку следующим образом:</span><span class="sxs-lookup"><span data-stu-id="b09a5-185">Open Revaluation Journal, create and post a line as follows:</span></span>  

     <span data-ttu-id="b09a5-186">Товар = ТЕСТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-186">Item = TEST</span></span>  

     <span data-ttu-id="b09a5-187">Примен. к операции = выберите операцию покупки, учтенную на шаге 2.</span><span class="sxs-lookup"><span data-stu-id="b09a5-187">Applies-to Entry = select Purchase entry posted at step 2.</span></span> <span data-ttu-id="b09a5-188">Дата учета переоценки будет такой же, как и в операции, которую она корректирует.</span><span class="sxs-lookup"><span data-stu-id="b09a5-188">The Posting Date of the revaluation will be the same as the entry it adjusts.</span></span>  

     <span data-ttu-id="b09a5-189">Себестоимость единицы (переоценка) = 40</span><span class="sxs-lookup"><span data-stu-id="b09a5-189">Unit Cost Revalued = 40</span></span>  

 <span data-ttu-id="b09a5-190">Были учтены следующие операции журнала товаров и стоимости:</span><span class="sxs-lookup"><span data-stu-id="b09a5-190">The following Item Ledger and Value Entries have been posted:</span></span>  

<span data-ttu-id="b09a5-191">![Обзор получающихся операций книги товаров и стоимости 1](media/helene/TechArticleAdjustcost9.png "Обзор получающихся операций книги товаров и стоимости 1")</span><span class="sxs-lookup"><span data-stu-id="b09a5-191">![Overview of resulting item ledger and value entries 1](media/helene/TechArticleAdjustcost9.png "Overview of resulting item ledger and value entries 1")</span></span>

 <span data-ttu-id="b09a5-192">![Обзор получающихся операций книги товаров и стоимости 2](media/helene/TechArticleAdjustcost10.png "Обзор получающихся операций книги товаров и стоимости 2")</span><span class="sxs-lookup"><span data-stu-id="b09a5-192">![Overview of resulting item ledger and value entries 2](media/helene/TechArticleAdjustcost10.png "Overview of resulting item ledger and value entries 2")</span></span>

 <span data-ttu-id="b09a5-193">Пакетное задание коррекции себестоимости запасов распознало изменение себестоимости и скорректировало поле "Расходы".</span><span class="sxs-lookup"><span data-stu-id="b09a5-193">The Adjust Cost – Item entries batch job has recognized a change in cost and adjusted the Negative Adjustments.</span></span>  

 <span data-ttu-id="b09a5-194">**Проверка дат учета в созданных операциях коррекции стоимости:** самая ранняя допустимая дата учета, с которой должно быть связано пакетное задание коррекции себестоимости запасов, — это 1-е января 2014 года, как указано в настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-194">**Review of Posting Dates on created Adjustment Value Entries:** The earliest allowed Posting Date the Adjust Cost - Item Entries batch job has to relate to is January 1st, 2014 as stated in the General Ledger Setup.</span></span>  

 <span data-ttu-id="b09a5-195">**Расход в шаге 3:** назначена дата учета 1-е января, указанная в настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-195">**Negative Adjustment in step 3:** assigned Posting Date is January 1st, provided by General Ledger Setup.</span></span> <span data-ttu-id="b09a5-196">Дата учета операции стоимости в рамках коррекции — 20-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-196">The Posting Date of the Value Entry in scope for adjustment is December 20, 2013.</span></span> <span data-ttu-id="b09a5-197">В соответствии с настройкой ГК эта дата не находится в разрешенном диапазоне дат учета.</span><span class="sxs-lookup"><span data-stu-id="b09a5-197">According to General Ledger Setup the date is not within allowed posting date range.</span></span> <span data-ttu-id="b09a5-198">Поэтому дата учета, указанная в поле "Разрешить учет от" в настройке ГК, назначена операции коррекции стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-198">Therefore the Posting Date stated in the Allow Posting From field in the General Ledger Setup is assigned to the Adjustment Value Entry.</span></span>  

 <span data-ttu-id="b09a5-199">**Расход на шаге 4:** назначена дата учета 15-е января.</span><span class="sxs-lookup"><span data-stu-id="b09a5-199">**Negative Adjustment in step 4:** assigned Posting Date is January 15th.</span></span> <span data-ttu-id="b09a5-200">Операция стоимости в рамках коррекции имеет дату учета 15-е января, которая находится в диапазоне допустимых дат учета согласно настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-200">The Value Entry in scope of adjustment has Posting Date January 15th, which is within the allowed posting date range according to General Ledger Setup.</span></span>  

 <span data-ttu-id="b09a5-201">Коррекция, выполненная для расхода на шаге 3, вызывает обсуждение.</span><span class="sxs-lookup"><span data-stu-id="b09a5-201">The adjustment made for the Negative Adjustment in step 3 causes discussion.</span></span> <span data-ttu-id="b09a5-202">Предпочтительная дата учета для операции коррекции стоимости была бы 20-е декабря или по крайней мере в декабре, так как переоценка, вызывающая изменение себестоимости продажи, была учтена в декабре.</span><span class="sxs-lookup"><span data-stu-id="b09a5-202">The favorable Posting Date for the Adjustment Value Entry would have been December 20th or at least within December as the revaluation causing the change in COGS was posted in December.</span></span>  

 <span data-ttu-id="b09a5-203">Чтобы получить коррекцию в декабре для расхода на шаге 3, в настройке ГК в поле "Разрешить учет с" должна быть указана дата в декабре.</span><span class="sxs-lookup"><span data-stu-id="b09a5-203">To achieve adjustment in December of the Negative Adjustment in step 3, the General Ledger Setup, Allow Posting From field, need to state a date in December.</span></span>  

 <span data-ttu-id="b09a5-204">**Заключение:**</span><span class="sxs-lookup"><span data-stu-id="b09a5-204">**Conclusion:**</span></span>  

 <span data-ttu-id="b09a5-205">С опытом из этого сценария при рассмотрении наиболее подходящей настройки допустимого диапазона дат разноски для компании могут быть полезны следующие соображения: если изменение стоимости запасов разрешено учитывать в некоторый период (в данном случае это декабрь), настройка компании, используемая для допустимых диапазонов дат учета, должна быть согласована с этим решением.</span><span class="sxs-lookup"><span data-stu-id="b09a5-205">With the experiences from this scenario, considering most suitable setup of allowed posting date range for a company, the following might be useful: As long as changes in inventory value is allowed to be posted in a period, December in this case, the setup the company uses for allowed posting date ranges should be aligned with this decision.</span></span> <span data-ttu-id="b09a5-206">Если в поле "Разрешить учет от" в настройке главной книги задано 1-е декабря, это позволит сделанную в декабре переоценку передать в соответствующие исходящие операции в этом же периоде.</span><span class="sxs-lookup"><span data-stu-id="b09a5-206">The Allow Posting From in the General Ledger Setup, stating December 1st  would allow the revaluation made in December to be forwarded to affected outbound entries in the same period.</span></span>  

 <span data-ttu-id="b09a5-207">Группы пользователей, которым не разрешено выполнять учет в декабря, а разрешено в январе, которые, вероятно, должны были ограничиваться настройкой ГК в этом сценарии, на самом деле следовало бы обрабатывать с помощью настройки пользователя.</span><span class="sxs-lookup"><span data-stu-id="b09a5-207">User groups not allowed to post in December but in January, which was probably intended to be limited by the General Ledger Setup in this scenario, should instead be addressed via the User setup.</span></span>  

### <a name="item-charge-scenario"></a><span data-ttu-id="b09a5-208">Сценарий товарных издержек:</span><span class="sxs-lookup"><span data-stu-id="b09a5-208">Item charge scenario:</span></span>  
 <span data-ttu-id="b09a5-209">Предварительные требования:</span><span class="sxs-lookup"><span data-stu-id="b09a5-209">Prerequisites:</span></span>  

 <span data-ttu-id="b09a5-210">Настройка модуля "Запасы":</span><span class="sxs-lookup"><span data-stu-id="b09a5-210">Inventory setup:</span></span>  

-   <span data-ttu-id="b09a5-211">Автомат. учет себест. = Да</span><span class="sxs-lookup"><span data-stu-id="b09a5-211">Automatic Cost Posting = Yes</span></span>  

-   <span data-ttu-id="b09a5-212">Автоматическая коррекция себестоимости = Всегда</span><span class="sxs-lookup"><span data-stu-id="b09a5-212">Automatic Cost Adjustment=Always</span></span>  

-   <span data-ttu-id="b09a5-213">Тип расчета средней себестоимости = товар</span><span class="sxs-lookup"><span data-stu-id="b09a5-213">Average Cost Calc. Type=item</span></span>  

-   <span data-ttu-id="b09a5-214">Период расчета средней себестоимости = День</span><span class="sxs-lookup"><span data-stu-id="b09a5-214">Average Cost Period=Day</span></span>  

 <span data-ttu-id="b09a5-215">Настройка ГК:</span><span class="sxs-lookup"><span data-stu-id="b09a5-215">General Ledger Setup:</span></span>  

-   <span data-ttu-id="b09a5-216">Разрешить учет с = 1-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-216">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="b09a5-217">Разрешить учет по = пусто</span><span class="sxs-lookup"><span data-stu-id="b09a5-217">Allow Posting To = empty</span></span>  

 <span data-ttu-id="b09a5-218">Настройка пользователя:</span><span class="sxs-lookup"><span data-stu-id="b09a5-218">User Setup:</span></span>  

-   <span data-ttu-id="b09a5-219">Разрешить учет с = 1-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-219">Allow Posting From = December 1st, 2013.</span></span>  

-   <span data-ttu-id="b09a5-220">Разрешить учет по = пусто</span><span class="sxs-lookup"><span data-stu-id="b09a5-220">Allow Posting to = empty</span></span>  

##### <a name="to-test-the-scenario"></a><span data-ttu-id="b09a5-221">Для проверки сценария</span><span class="sxs-lookup"><span data-stu-id="b09a5-221">To test the scenario</span></span>  

1.  <span data-ttu-id="b09a5-222">Создайте товарные издержки:</span><span class="sxs-lookup"><span data-stu-id="b09a5-222">Create item charge:</span></span>  

     <span data-ttu-id="b09a5-223">Базовая единица измерения = ШТ.</span><span class="sxs-lookup"><span data-stu-id="b09a5-223">Base unit of measure = PCS</span></span>  

     <span data-ttu-id="b09a5-224">Метод учета себестоимости = Среднее</span><span class="sxs-lookup"><span data-stu-id="b09a5-224">Costing Method = Average</span></span>  

     <span data-ttu-id="b09a5-225">Выберите необязательные учетные группы.</span><span class="sxs-lookup"><span data-stu-id="b09a5-225">Select optional posting groups.</span></span>  

2.  <span data-ttu-id="b09a5-226">Создание нового заказа на покупку</span><span class="sxs-lookup"><span data-stu-id="b09a5-226">Create new purchase order</span></span>  

     <span data-ttu-id="b09a5-227">Код поставщика: 10000</span><span class="sxs-lookup"><span data-stu-id="b09a5-227">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b09a5-228">Дата учета = 15-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-228">Posting Date = December 15th, 2013</span></span>  

     <span data-ttu-id="b09a5-229">Номер счета-фактуры поставщика: 1234</span><span class="sxs-lookup"><span data-stu-id="b09a5-229">Vendor Invoice No.: 1234</span></span>  

     <span data-ttu-id="b09a5-230">В строке заказа на покупку:</span><span class="sxs-lookup"><span data-stu-id="b09a5-230">On the purchase order line:</span></span>  

     <span data-ttu-id="b09a5-231">Товар = ИЗДЕРЖКИ</span><span class="sxs-lookup"><span data-stu-id="b09a5-231">Item = CHARGE</span></span>  

     <span data-ttu-id="b09a5-232">Количество = 1</span><span class="sxs-lookup"><span data-stu-id="b09a5-232">Quantity = 1</span></span>  

     <span data-ttu-id="b09a5-233">Прямая себестоимость единицы = 100</span><span class="sxs-lookup"><span data-stu-id="b09a5-233">Direct Unit Cost = 100</span></span>  

     <span data-ttu-id="b09a5-234">Выполните учет приемки и счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="b09a5-234">Post Receive and Invoice.</span></span>  

3.  <span data-ttu-id="b09a5-235">Создайте новый заказ на продажу:</span><span class="sxs-lookup"><span data-stu-id="b09a5-235">Create new sales order:</span></span>  

     <span data-ttu-id="b09a5-236">Код клиента: 10000;</span><span class="sxs-lookup"><span data-stu-id="b09a5-236">Sell-to Customer No.: 10000</span></span>  

     <span data-ttu-id="b09a5-237">Дата учета = 16-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-237">Posting Date = December 16th, 2013</span></span>  

     <span data-ttu-id="b09a5-238">В строке заказа продажи:</span><span class="sxs-lookup"><span data-stu-id="b09a5-238">On the sales order line:</span></span>  

     <span data-ttu-id="b09a5-239">Товар = ИЗДЕРЖКИ</span><span class="sxs-lookup"><span data-stu-id="b09a5-239">Item = CHARGE</span></span>  

     <span data-ttu-id="b09a5-240">Количество = 1</span><span class="sxs-lookup"><span data-stu-id="b09a5-240">Quantity = 1</span></span>  

     <span data-ttu-id="b09a5-241">Цена единицы = 135</span><span class="sxs-lookup"><span data-stu-id="b09a5-241">Unit Price = 135</span></span>  

     <span data-ttu-id="b09a5-242">Выполните учет отгрузки и счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="b09a5-242">Post Ship and Invoice.</span></span>  

4.  <span data-ttu-id="b09a5-243">Настройка ГК:</span><span class="sxs-lookup"><span data-stu-id="b09a5-243">General Ledger Setup:</span></span>  

     <span data-ttu-id="b09a5-244">Разрешить учет с = 1-е января 2014 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-244">Allow Posting From = January 1st, 2014</span></span>  

     <span data-ttu-id="b09a5-245">Разрешить учет по = пусто</span><span class="sxs-lookup"><span data-stu-id="b09a5-245">Allow Posting To = blank</span></span>  

5.  <span data-ttu-id="b09a5-246">Создайте новый заказ на покупку:</span><span class="sxs-lookup"><span data-stu-id="b09a5-246">Create new purchase order:</span></span>  

     <span data-ttu-id="b09a5-247">Код поставщика: 10000</span><span class="sxs-lookup"><span data-stu-id="b09a5-247">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b09a5-248">Дата учета = 2-е января 2014 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-248">Posting Date = January 2nd, 2014</span></span>  

     <span data-ttu-id="b09a5-249">Номер счета-фактуры поставщика: 2345</span><span class="sxs-lookup"><span data-stu-id="b09a5-249">Vendor Invoice No.: 2345</span></span>  

     <span data-ttu-id="b09a5-250">В строке заказа на покупку:</span><span class="sxs-lookup"><span data-stu-id="b09a5-250">On the purchase order line:</span></span>  

     <span data-ttu-id="b09a5-251">Товарные издержки = РАБ-ФРАХТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-251">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="b09a5-252">Количество = 1</span><span class="sxs-lookup"><span data-stu-id="b09a5-252">Quantity = 1</span></span>  

     <span data-ttu-id="b09a5-253">Прямая себестоимость единицы = 3</span><span class="sxs-lookup"><span data-stu-id="b09a5-253">Direct Unit Cost = 3</span></span>  

     <span data-ttu-id="b09a5-254">Назначьте товарные издержки приходной накладной покупки из шага 2.</span><span class="sxs-lookup"><span data-stu-id="b09a5-254">Assign Item Charge to Purchase Receipt from step 2.</span></span>  

     <span data-ttu-id="b09a5-255">Выполните учет приходной накладной и счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="b09a5-255">Post Receipt and Invoice.</span></span>  

     <span data-ttu-id="b09a5-256">![Обзор получающихся операций книги товаров и стоимости 3](media/helene/TechArticleAdjustcost11.png "Обзор получающихся операций книги товаров и стоимости 3")</span><span class="sxs-lookup"><span data-stu-id="b09a5-256">![Overview of resulting item ledger and value entries 3](media/helene/TechArticleAdjustcost11.png "Overview of resulting item ledger and value entries 3")</span></span>

6.  <span data-ttu-id="b09a5-257">В рабочую дату 3-го января поступает счет покупки, содержащий дополнительные товарные издержки по покупке, произведенной на шаге 2.</span><span class="sxs-lookup"><span data-stu-id="b09a5-257">On work date January 3rd a purchase invoice arrives, containing an additional item charge to the purchase made in step 2.</span></span> <span data-ttu-id="b09a5-258">Этот счет имеет дату документа 30-е декабря, поэтому он учитывается с датой учета 30-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-258">This invoice has document date December 30th and is therefore posted with Posting Date December 30th, 2013.</span></span>  

     <span data-ttu-id="b09a5-259">Создайте новый заказ на покупку:</span><span class="sxs-lookup"><span data-stu-id="b09a5-259">Create new purchase order:</span></span>  

     <span data-ttu-id="b09a5-260">Код поставщика: 10000</span><span class="sxs-lookup"><span data-stu-id="b09a5-260">Buy-from Vendor No.: 10000</span></span>  

     <span data-ttu-id="b09a5-261">Дата учета = 30-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-261">Posting Date = December 30th, 2013</span></span>  

     <span data-ttu-id="b09a5-262">Номер счета-фактуры поставщика: 3456</span><span class="sxs-lookup"><span data-stu-id="b09a5-262">Vendor Invoice No.: 3456</span></span>  

     <span data-ttu-id="b09a5-263">В строке заказа на покупку:</span><span class="sxs-lookup"><span data-stu-id="b09a5-263">On the purchase order line:</span></span>  

     <span data-ttu-id="b09a5-264">Товарные издержки = РАБ-ФРАХТ</span><span class="sxs-lookup"><span data-stu-id="b09a5-264">Item Charge = JB-FREIGHT</span></span>  

     <span data-ttu-id="b09a5-265">Количество = 1</span><span class="sxs-lookup"><span data-stu-id="b09a5-265">Quantity = 1</span></span>  

     <span data-ttu-id="b09a5-266">Прямая себестоимость единицы = 2</span><span class="sxs-lookup"><span data-stu-id="b09a5-266">Direct Unit Cost = 2</span></span>  

     <span data-ttu-id="b09a5-267">Назначьте товарные издержки приходной накладной покупки из шага 2</span><span class="sxs-lookup"><span data-stu-id="b09a5-267">Assign Item Charge to Purchase Receipt from step 2</span></span>  

     <span data-ttu-id="b09a5-268">Выполните учет приходной накладной и счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="b09a5-268">Post Receipt and Invoice.</span></span>  

   <span data-ttu-id="b09a5-269">![Обзор получающихся операций книги товаров и стоимости 4](media/helene/TechArticleAdjustcost12.png "Обзор получающихся операций книги товаров и стоимости 4")</span><span class="sxs-lookup"><span data-stu-id="b09a5-269">![Overview of resulting item ledger and value entries 4](media/helene/TechArticleAdjustcost12.png "Overview of resulting item ledger and value entries 4")</span></span>

 <span data-ttu-id="b09a5-270">Отчет оценки стоимости запасов распечатывается на дату 31-е декабря 2013 г.</span><span class="sxs-lookup"><span data-stu-id="b09a5-270">Inventory Valuation report is printed as of Date December 31st , 2013</span></span>  

<span data-ttu-id="b09a5-271">![Содержимое отчета "Оценка стоимости запасов"](media/helene/TechArticleAdjustcost13.png "Содержимое отчета "Оценка стоимости запасов"")</span><span class="sxs-lookup"><span data-stu-id="b09a5-271">![Content of the Inventory Valuation report](media/helene/TechArticleAdjustcost13.png "Content of the Inventory Valuation report")</span></span>

 <span data-ttu-id="b09a5-272">**Сводка сценария:**</span><span class="sxs-lookup"><span data-stu-id="b09a5-272">**Summary of scenario:**</span></span>  

 <span data-ttu-id="b09a5-273">Описанный сценарий заканчивается тем, что в отчете оценки стоимости запасов отображается Количество = 0, тогда как Стоимость = 2.</span><span class="sxs-lookup"><span data-stu-id="b09a5-273">The described scenario ends up with an Inventory Valuation report demonstrating Quantity = 0 while the Value = 2.</span></span> <span data-ttu-id="b09a5-274">Товарные издержки, учтенные на шаге 11, являются частью значения прихода склада в декабре, в то время как значение расхода склада за этот же период не затронуто.</span><span class="sxs-lookup"><span data-stu-id="b09a5-274">The Item charge posted in step 11 is part of the Inventory Increase value of December while the Inventory Decrease of the same period is not affected.</span></span>  

 <span data-ttu-id="b09a5-275">Наличие настройки ГК, в которой указано разрешение учета с 1-го января, было удачным решением для первой товарной издержки.</span><span class="sxs-lookup"><span data-stu-id="b09a5-275">Having the General Ledger Setup stating Allow Posting From January 1st was a good thing for the first Item charge.</span></span> <span data-ttu-id="b09a5-276">Себестоимость прихода и расхода склада была зарегистрирована за один и тот же период.</span><span class="sxs-lookup"><span data-stu-id="b09a5-276">The costs of the Inventory Increase and Decrease was recorded in the same period.</span></span> <span data-ttu-id="b09a5-277">Однако для второй товарной издержки настройка главной книги привела к тому, что себестоимость продажи была распознана в последующем периоде.</span><span class="sxs-lookup"><span data-stu-id="b09a5-277">For the second Item charge however, the General Ledger Setup causes the change in COGS to be recognized in the period after.</span></span>  

 <span data-ttu-id="b09a5-278">**Заключение:**</span><span class="sxs-lookup"><span data-stu-id="b09a5-278">**Conclusion:**</span></span>  

 <span data-ttu-id="b09a5-279">Достаточно сложно добиться того, чтобы в отчете по оценке стоимости запасов указывалось количество = 0, когда значение <> 0.</span><span class="sxs-lookup"><span data-stu-id="b09a5-279">It’s a challenge to have the Inventory Valuation report to demonstrate Quantity = 0 while the Value <> 0.</span></span> <span data-ttu-id="b09a5-280">В этом случае также более сложно выразить оптимальные настройки, так как счета покупки поступили в один день, но относятся к разным периодам или даже финансовым годам.</span><span class="sxs-lookup"><span data-stu-id="b09a5-280">In this case it’s also more difficult to express the optimal settings, having purchase invoices arriving the same day but addressing different periods or even fiscal years.</span></span> <span data-ttu-id="b09a5-281">Для перехода на новый финансовый год обычно требуется определенное планирование, в рамках которого требуется учитывать анализ процесса коррекции себестоимости запасов и распознавания себестоимости продажи.</span><span class="sxs-lookup"><span data-stu-id="b09a5-281">Crossing to a new fiscal year usually requires some planning and as part of that the insight of Adjust Cost – Item entries process, recognizing COGS, is to be considered.</span></span>  

 <span data-ttu-id="b09a5-282">В этом сценарии в качестве одного из вариантов можно было бы задать в настройке ГК для поля "Разрешить учет с" дату в декабре еще на пару дополнительных дней, а учет первой товарной издержки задержать, чтобы сначала обеспечить распознавание всех затрат за предыдущий период или фискальный год, к которому они принадлежат, затем запустить пакетное задание коррекции себестоимости запасов, после чего переместить разрешенную дату учета на новый период\/финансовый год.</span><span class="sxs-lookup"><span data-stu-id="b09a5-282">In this scenario one option could have been to have the General Ledger Setup, field Allow Posting From, stating a date in December for a couple of more days and the posting of the first item charge postponed to allow all costs for the previous period/fiscal year to be recognized for the period they belong to first, having the Adjust Cost – Item entries batch job run and thereafter move the allowed posting date to the new period\/fiscal year.</span></span> <span data-ttu-id="b09a5-283">Первая товарная издержка с датой учета 2-е января затем могла бы быть учтена.</span><span class="sxs-lookup"><span data-stu-id="b09a5-283">The first item charge with posting date January 2nd could then be posted.</span></span>  

## <a name="history-of-adjust-cost--item-entries-batch-job"></a><span data-ttu-id="b09a5-284">История пакетного задания коррекции себестоимости запасов</span><span class="sxs-lookup"><span data-stu-id="b09a5-284">History of Adjust Cost – Item entries batch job</span></span>  
 <span data-ttu-id="b09a5-285">Ниже приведена сводка концепции назначения дат учета операций коррекции стоимости пакетным заданием коррекции себестоимости запасов, начиная с версии 3.0.</span><span class="sxs-lookup"><span data-stu-id="b09a5-285">Below is a summary of the concept assigning Posting Dates to Adjustment Value Entries by the Adjust Cost – Item entries batch job since version 3.0.</span></span>  

### <a name="from-version-30370a"></a><span data-ttu-id="b09a5-286">С версии 3.0..3.70.A</span><span class="sxs-lookup"><span data-stu-id="b09a5-286">From version 3.0..3.70.A</span></span>  
 <span data-ttu-id="b09a5-287">В форме запроса пакетного задания корректировки себестоимости запасов имеется дата учета, которая должна вводиться пользователем.</span><span class="sxs-lookup"><span data-stu-id="b09a5-287">In the request form of the Adjust Cost - Item Entries batch job there is a Posting Date to be entered by the user.</span></span> <span data-ttu-id="b09a5-288">Пакетное задание выполняет все необходимые изменения и создает операции стоимости с датой учета, введенной в форму запроса.</span><span class="sxs-lookup"><span data-stu-id="b09a5-288">The batch job runs through all necessary changes and creates value entries with the posting date entered in the request form.</span></span> <span data-ttu-id="b09a5-289">Предлагаемая дата учета — текущая дата.</span><span class="sxs-lookup"><span data-stu-id="b09a5-289">Suggested posting date to use is today’s date.</span></span>  

### <a name="version-370b40"></a><span data-ttu-id="b09a5-290">Версия 3.70.B..4.0</span><span class="sxs-lookup"><span data-stu-id="b09a5-290">Version 3.70.B..4.0</span></span>  
 <span data-ttu-id="b09a5-291">В форме запроса пакетного задания корректировки себестоимости запасов имеется дата учета операции закрытого периода, которая должна вводиться пользователем.</span><span class="sxs-lookup"><span data-stu-id="b09a5-291">In the request form of the Adjust Cost - Item Entries batch job there is a Closed Period Entry Posting Date to be entered by the user.</span></span> <span data-ttu-id="b09a5-292">Пакетное задание выполняет все необходимые изменения и создает операции стоимости с датой учета родительской операции книги товаров (дата отгрузки продажи, для которой выполняется корректировка).</span><span class="sxs-lookup"><span data-stu-id="b09a5-292">The batch job runs through all necessary changes and creates value entries with the posting date of the parent item ledger entry (shipment date of the sale that the adjustment address).</span></span> <span data-ttu-id="b09a5-293">Если дата учета родительской операции книги товаров не находится в допустимом диапазоне дат учета, дата учета, указанная как дата учета операции закрытого периода, будет назначена операции коррекции стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-293">If the posting date of the parent item ledger entry is not within allowed posting date range the posting date stated as Closed Period Entry Posting Date will be assigned the Adjustment Value Entry.</span></span> <span data-ttu-id="b09a5-294">Дата считается относящейся к закрытому периоду, если она раньше даты в поле "Разрешить учет с" в настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-294">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span></span>  

### <a name="from-version-50"></a><span data-ttu-id="b09a5-295">С версии 5.0:</span><span class="sxs-lookup"><span data-stu-id="b09a5-295">From version 5.0:</span></span>  
 <span data-ttu-id="b09a5-296">Больше не требуется указывать дату учета в запросе пакетного задания корректировки себестоимости запасов.</span><span class="sxs-lookup"><span data-stu-id="b09a5-296">There is no longer a posting date to be stated in the request form of the Adjust Cost - Item entries batch job.</span></span> <span data-ttu-id="b09a5-297">Пакетное задание выполняет все необходимые изменения и создает операции стоимости с датой учета операции стоимости, которую оно корректирует.</span><span class="sxs-lookup"><span data-stu-id="b09a5-297">The batch job runs through all necessary changes and creates value entries with the posting date of the value entry it adjusts.</span></span> <span data-ttu-id="b09a5-298">Если дата учета не находится в пределах допустимого диапазона дат учета, будет использована дата учета из поля "Разрешить учет с" в настройке ГК ИЛИ, если используются периоды учета запасов, будет использована более поздняя дата из этих двух.</span><span class="sxs-lookup"><span data-stu-id="b09a5-298">If the posting date is not within allowed posting date range the posting date in the Allow Posting From field in the General Ledger Setup, OR if the Inventory periods are used, the later date of the two will be used.</span></span> <span data-ttu-id="b09a5-299">См. описанную концепцию выше.</span><span class="sxs-lookup"><span data-stu-id="b09a5-299">See described concept above.</span></span>  

## <a name="history-of-post-inventory-cost-to-gl-batch-job"></a><span data-ttu-id="b09a5-300">История пакетного задания «Учет себест. запасов в ГК»</span><span class="sxs-lookup"><span data-stu-id="b09a5-300">History of Post Inventory cost to G/L batch job</span></span>  
 <span data-ttu-id="b09a5-301">Пакетное задание «Учет себест. запасов в ГК» тесно связано с пакетным заданием «Коррекция себест. запасов», поэтому здесь также приводится история этого пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="b09a5-301">The Post Inventory Cost to G/L batch job is closely related to the Adjust Cost – Item entries batch job why the history of this batch job is summarized and shared here as well.</span></span>  

### <a name="from-version-30370a"></a><span data-ttu-id="b09a5-302">С версии 3.0..3.70.A</span><span class="sxs-lookup"><span data-stu-id="b09a5-302">From version 3.0..3.70.A</span></span>  
 <span data-ttu-id="b09a5-303">В форме запроса пакетного «Учет себест. запасов в ГК» имеется дата учета, которая должна вводиться пользователем.</span><span class="sxs-lookup"><span data-stu-id="b09a5-303">In the request form of the Post Inventory Cost to G/L there is a Posting Date to be entered by the user.</span></span> <span data-ttu-id="b09a5-304">Пакетное задание просматривает все операции стоимости в рамках фильтра (при наличии) и создает операции главной книги с датой учета, введенной в форму запроса.</span><span class="sxs-lookup"><span data-stu-id="b09a5-304">The batch job runs through all value entries within the filter, if any, and creates General Ledger Entries with Posting Date entered in the request form.</span></span>  

### <a name="version-370b40"></a><span data-ttu-id="b09a5-305">Версия 3.70.B..4.0</span><span class="sxs-lookup"><span data-stu-id="b09a5-305">Version 3.70.B..4.0</span></span>  
 <span data-ttu-id="b09a5-306">В форме запроса пакетного «Учет себест. запасов в ГК» предусмотрено поле даты учета операций закрытого периода.</span><span class="sxs-lookup"><span data-stu-id="b09a5-306">In the request form of the Post Inventory Cost to G/L the Closed Period Entry Posting Date field is available.</span></span> <span data-ttu-id="b09a5-307">Приложение использует дату, введенную пользователем в это поле, в качестве даты учета для операций главной книги, которые она создает для операций стоимости, даты учета которых относятся к закрытым периодам учета.</span><span class="sxs-lookup"><span data-stu-id="b09a5-307">The application uses the date you enter in this field as the posting date for the general ledger entries it creates for value entries whose posting dates are in closed accounting periods.</span></span> <span data-ttu-id="b09a5-308">В противном случае операции ГК будут иметь ту же дату учета, что и исходные операции стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-308">Otherwise, the general ledger entries will have the same posting date as the original value entries.</span></span> <span data-ttu-id="b09a5-309">Дата считается относящейся к закрытому периоду, если она раньше даты в поле "Разрешить учет с" в настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-309">A date is considered to be in a closed period when it is earlier than the date in the Allow Posting From field in the General Ledger Setup.</span></span> <span data-ttu-id="b09a5-310">При учете в Г\/К по группам учета операции главной книги будут иметь дату учета, которая указана в поле «Дата учета» в форме запроса.</span><span class="sxs-lookup"><span data-stu-id="b09a5-310">If posting to G\/L Per Posting Group, the general ledger entries will have the posting date that is specified in the Posting Date field in the request form.</span></span>  

 <span data-ttu-id="b09a5-311">В версиях 3 и 4 пакетное задание сканирует все операции стоимости для определения, имеются ли какие-либо операции стоимости, в котором сумма себестоимости (факт) отличается от стоимости, учтенной в ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-311">In version 3 and 4 the batch job scans all value entries to detect if there are any value entries where Cost Amount (Actual) differs from Cost Posted to G/L.</span></span> <span data-ttu-id="b09a5-312">Если обнаружено различие, отличающаяся сумма будет учтена в операции ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-312">If there is a difference detected the differing amount will be posted in a G/L entry.</span></span> <span data-ttu-id="b09a5-313">Если используется учет ожидаемой себестоимости, то соответствующие поля обрабатываются таким же образом.</span><span class="sxs-lookup"><span data-stu-id="b09a5-313">If expected cost posting is used corresponding fields are processed in the same way.</span></span>  

<span data-ttu-id="b09a5-314">![Фактическая и ожидаемая себестоимость](media/helene/TechArticleAdjustcost14.png "Фактическая и ожидаемая себестоимость")</span><span class="sxs-lookup"><span data-stu-id="b09a5-314">![Actual cost versus expected cost](media/helene/TechArticleAdjustcost14.png "Actual cost versus expected cost")</span></span>

### <a name="from-version-50"></a><span data-ttu-id="b09a5-315">С версии 5.0:</span><span class="sxs-lookup"><span data-stu-id="b09a5-315">From version 5.0:</span></span>  
 <span data-ttu-id="b09a5-316">Больше не требуется указывать дату учета в запросе пакетного задания «Учет себест. запасов в ГК».</span><span class="sxs-lookup"><span data-stu-id="b09a5-316">There is no longer a posting date to be stated in the request form of the Post Inventory Cost to G/L batch job.</span></span> <span data-ttu-id="b09a5-317">Операция ГК создается с той же датой учета, что и связанная операция стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-317">The G/L entry is created with the same Posting Date as the related value entry.</span></span> <span data-ttu-id="b09a5-318">Чтобы выполнить пакетное задание, допустимый диапазон дат учета должен разрешать дату учета созданной операции ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-318">In order to complete the batch job the allowed posting date range must allow the Posting Date of the created G/L entry.</span></span> <span data-ttu-id="b09a5-319">В противном случае разрешенный диапазон дат учета должен быть временно повторно открыт путем изменения или удаления дат в полях «Разрешить учет с» и «Разрешить учет по» в настройке ГК.</span><span class="sxs-lookup"><span data-stu-id="b09a5-319">If not, the allowed posting date range must be temporarily re-opened by changing or removing the dates in the Allow Posting From and To fields in the General Ledger Setup.</span></span> <span data-ttu-id="b09a5-320">Во избежание проблем выверки необходимо, чтобы дата учета операции ГК соответствовала дате учета операции стоимости.</span><span class="sxs-lookup"><span data-stu-id="b09a5-320">To avoid reconciliation issues it is required that Posting Date of the G/L Entry corresponds to the Posting Date of the Value Entry.</span></span>  

 <span data-ttu-id="b09a5-321">Пакетное задание просматривает таблицу 5811 — Учет операции стоимости в ГК для выявления операций стоимости, входящих в область действия для учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="b09a5-321">The batch job scans Table 5811 - Post Value Entry to G/L, to identify the Value Entries in scope for posting to General Ledger.</span></span> <span data-ttu-id="b09a5-322">После успешного выполнения таблица очищается.</span><span class="sxs-lookup"><span data-stu-id="b09a5-322">After successful run the table is emptied.</span></span>

## <a name="see-also"></a><span data-ttu-id="b09a5-323">См. также</span><span class="sxs-lookup"><span data-stu-id="b09a5-323">See Also</span></span>  
[<span data-ttu-id="b09a5-324">Сведения о проектировании: себестоимость запасов</span><span class="sxs-lookup"><span data-stu-id="b09a5-324">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)  
[<span data-ttu-id="b09a5-325">Сведения о проектировании: применение товара</span><span class="sxs-lookup"><span data-stu-id="b09a5-325">Design Details: Item Application</span></span>](design-details-item-application.md)  
