---
title: "Обслуживание основных средств | Документы Майкрософт"
description: "Запись обслуживания ведется для ремонтных работ и сервисных обслуживаний основных средств."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: repair, service
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 71210a9acbd196581aa4397264b462728007e5e8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-maintain-fixed-assets"></a><span data-ttu-id="2f249-103">Практическое руководство. Обслуживание основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-103">How to: Maintain Fixed Assets</span></span>
<span data-ttu-id="2f249-104">Стоимость обслуживания — это периодические затраты, направленные на сохранение стоимости основных средств.</span><span class="sxs-lookup"><span data-stu-id="2f249-104">Maintenance expenses are routine periodic costs undertaken to preserve the value of fixed assets.</span></span> <span data-ttu-id="2f249-105">В отличие от капитальных усовершенствований они не увеличивают стоимость.</span><span class="sxs-lookup"><span data-stu-id="2f249-105">Unlike capital improvements, they do not increase values.</span></span>

<span data-ttu-id="2f249-106">Можно записать и обновлять файл по обслуживанию основных средств, чтобы полные сведения об обслуживании каждого основного средства были всегда доступны.</span><span class="sxs-lookup"><span data-stu-id="2f249-106">You can record and maintain an up-to-date file on maintenance and service of your fixed assets to have complete maintenance records on a fixed asset easily accessible.</span></span> <span data-ttu-id="2f249-107">Когда основное средство отправляется для сервиса, вы записываете всю соответствующую информацию, такую как дата обслуживания, номер поставщика и телефонный номер сервисного агента.</span><span class="sxs-lookup"><span data-stu-id="2f249-107">Each time a fixed asset is sent to service, you record all relevant information such as date of service, vendor number and service agent's phone number.</span></span> <span data-ttu-id="2f249-108">Регистрация обслуживания записывается для каждого основного средства из соответствующей карточки основного средства.</span><span class="sxs-lookup"><span data-stu-id="2f249-108">Maintenance registration is recorded for each fixed asset from the relevant fixed asset card.</span></span>

<span data-ttu-id="2f249-109">Переоценка используется для коррекции значений при изменении общего уровня цен.</span><span class="sxs-lookup"><span data-stu-id="2f249-109">Indexation is used to adjust values for general price-level changes.</span></span> <span data-ttu-id="2f249-110">Для пересчета стоимости обслуживания может использоваться пакетное задание **Индекс ОС**.</span><span class="sxs-lookup"><span data-stu-id="2f249-110">The **Index Fixed Assets** batch job can be used to recalculate the maintenance costs.</span></span>

## <a name="to-record-maintenance-work-on-a-fixed-asset"></a><span data-ttu-id="2f249-111">Запись работ по обслуживанию основного средства</span><span class="sxs-lookup"><span data-stu-id="2f249-111">To record maintenance work on a fixed asset</span></span>
<span data-ttu-id="2f249-112">Каждый раз при проведении обслуживания (например, при сервисном посещении) его можно записать для соответствующего основного средства в окне **Обслуживание - регистрация**.</span><span class="sxs-lookup"><span data-stu-id="2f249-112">Every time maintenance has been performed, such as a service visit, you can record it for the relevant fixed asset in the **Maintenance Registrations** window.</span></span>  

1. <span data-ttu-id="2f249-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Основные средства**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2f249-114">Выберите основное средство, для которого требуется зарегистрировать обслуживание, затем выберите действие **Обслуживание - регистрация**.</span><span class="sxs-lookup"><span data-stu-id="2f249-114">Select the fixed asset that you want to record maintenance for, and then choose the **Maintenance Registration** action.</span></span>
3. <span data-ttu-id="2f249-115">В окне **Обслуживание - регистрация** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="2f249-115">In the **Maintenance Registration** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-post-maintenance-costs-from-a-fixed-asset-gl-journal"></a><span data-ttu-id="2f249-116">Учет стоимости обслуживания из журнала ГК учета основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-116">To post maintenance costs from a fixed asset G/L journal</span></span>
1. <span data-ttu-id="2f249-117">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Список книг амортизации**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Depreciation Book List**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2f249-118">Выберите книгу амортизации, которая назначена основному средству, затем выберите действие **Правка**.</span><span class="sxs-lookup"><span data-stu-id="2f249-118">Select the depreciation book that is assigned to the fixed asset, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="2f249-119">В окне **Карточка книги амортизации** убедитесь, что флажок **Обслуживание** не установлен.</span><span class="sxs-lookup"><span data-stu-id="2f249-119">In the **Depreciation Book Card** window, make sure the **Maintenance** check box is not selected.</span></span> <span data-ttu-id="2f249-120">Это гарантирует, что стоимость обслуживания не учитывается в главной книге.</span><span class="sxs-lookup"><span data-stu-id="2f249-120">This ensures that maintenance costs are not posted to the general ledger.</span></span>
4. <span data-ttu-id="2f249-121">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы ГК ОС**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
5. <span data-ttu-id="2f249-122">Создайте начальную строку журнала и заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="2f249-122">Create an initial journal line and fill in the fields as necessary.</span></span>
6. <span data-ttu-id="2f249-123">В поле **Тип учета ОС** выберите **Обслуживание**.</span><span class="sxs-lookup"><span data-stu-id="2f249-123">In the **FA Posting Type** field, select **Maintenance**.</span></span>
7. <span data-ttu-id="2f249-124">Выберите действие **Вставить баланс. счет ОС**.</span><span class="sxs-lookup"><span data-stu-id="2f249-124">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="2f249-125">Вторая строка журнала создается для балансирующего счета, который настроен для учета обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2f249-125">A second journal line is created for the balancing account that is set up for maintenance posting.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="2f249-126">Шаг 7 работает только в том случае, если выполнены следующие настройки: в окне **Карточка учетной группы ОС** для учетной группы основного средства поле **Счет обслуживания** содержит дебетовый счет главной книги, а поле **Баланс. счет обслуживания** содержит счет главной книги, на котором требуется учитывать балансовые операции для повышения стоимости.</span><span class="sxs-lookup"><span data-stu-id="2f249-126">Step 7 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Maintenance Account** field contains the general ledger debit account and the **Maintenance Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="2f249-127">Дополнительные сведения см. в пункте "Настройка учетных групп основных средств" в разделе [Практическое руководство. Настройка общих данных основных средств](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="2f249-127">For more information, see the "To set up fixed asset posting groups" section in [How to: Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>
8. <span data-ttu-id="2f249-128">Выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="2f249-128">Choose the **Post** action.</span></span>

## <a name="to-follow-up-on-fixed-assets-service-visits"></a><span data-ttu-id="2f249-129">Отслеживание сервисных посещений для обслуживания основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-129">To follow up on fixed assets service visits</span></span>
<span data-ttu-id="2f249-130">Чтобы просмотреть, для каких активов запланировано сервисное посещение, можно напечатать отчет **Обслуживание - след. сервис**.</span><span class="sxs-lookup"><span data-stu-id="2f249-130">You can print the **Maintenance - Next Service** report to see which assets you have scheduled a service visit for.</span></span> <span data-ttu-id="2f249-131">Также можно использовать этот отчет при обновлении поля **След. дата сервисного обслуживания** на карточках основных средств.</span><span class="sxs-lookup"><span data-stu-id="2f249-131">You can also use this report when you are updating the **Next Service Date** field on fixed asset cards.</span></span>  

1. <span data-ttu-id="2f249-132">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Обслуживание - след. сервис**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Next Service**, and then choose the related link.</span></span>  
2. <span data-ttu-id="2f249-133">Заполните поля **Дата начала** и **Дата окончания**.</span><span class="sxs-lookup"><span data-stu-id="2f249-133">Fill in the **Starting Date** and **Ending Date** fields.</span></span>  
3. <span data-ttu-id="2f249-134">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="2f249-134">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-monitor-maintenance-costs"></a><span data-ttu-id="2f249-135">Просмотр значений стоимости обслуживания</span><span class="sxs-lookup"><span data-stu-id="2f249-135">To monitor maintenance costs</span></span>
<span data-ttu-id="2f249-136">Можно просматривать значения стоимости обслуживания при просмотре статистики основных средств.</span><span class="sxs-lookup"><span data-stu-id="2f249-136">You can view the maintenance costs when you look at the statistics of a fixed asset.</span></span>  

1. <span data-ttu-id="2f249-137">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Основные средства**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-137">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="2f249-138">Выберите основное средство, для которого требуется просмотреть затраты на обслуживание, затем выберите действие **Книги амортизации**.</span><span class="sxs-lookup"><span data-stu-id="2f249-138">Select the fixed asset you want to view maintenance costs for, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="2f249-139">В окне **Книги амортизации ОС** выберите книгу амортизации соответствующего основного средства, затем выберите действие **Статистика**.</span><span class="sxs-lookup"><span data-stu-id="2f249-139">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Statistics** action.</span></span>
4. <span data-ttu-id="2f249-140">В окне **ОС - статистика** выберите поле **Обслуживание**.</span><span class="sxs-lookup"><span data-stu-id="2f249-140">In the **Fixed Asset Statistics** window, choose the **Maintenance** field.</span></span>

<span data-ttu-id="2f249-141">Открывается окно **Операции книги обслуживания** с записями, из которых складывается сумма в поле **Обслуживание**.</span><span class="sxs-lookup"><span data-stu-id="2f249-141">The **Maintenance Ledger Entries** window opens showing the entries that make up the amount in the **Maintenance** field.</span></span>

## <a name="to-view-or-print-maintenance-costs-for-multiple-fixed-assets"></a><span data-ttu-id="2f249-142">Просмотр или печатать значений стоимости обслуживания для нескольких основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-142">To view or print maintenance costs for multiple fixed assets</span></span>
<span data-ttu-id="2f249-143">В отчете **Обслуживание - анализ** можно выбрать просмотр обслуживания по одному, двум или трем кодам обслуживания относительно определенной даты или периода.</span><span class="sxs-lookup"><span data-stu-id="2f249-143">In the **Maintenance - Analysis** report, you can select to see maintenance based on one, two, or three maintenance codes for a specified date or period.</span></span> <span data-ttu-id="2f249-144">Можно посмотреть итоги по всем выбранным основным средствам или итоги по каждому основному средству.</span><span class="sxs-lookup"><span data-stu-id="2f249-144">You can see the total of all selected assets or a total for each asset.</span></span>

1. <span data-ttu-id="2f249-145">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Обслуживание - анализ**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Analysis**, and then choose the related link.</span></span>
2. <span data-ttu-id="2f249-146">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="2f249-146">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="2f249-147">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="2f249-147">Choose the **Print** or **Preview** button.</span></span>

## <a name="to-view-maintenance-ledger-entries"></a><span data-ttu-id="2f249-148">Просмотр операций книги обслуживания</span><span class="sxs-lookup"><span data-stu-id="2f249-148">To view maintenance ledger entries</span></span>
<span data-ttu-id="2f249-149">Можно также изучать значения стоимости обслуживания, просматривая операции книги обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2f249-149">You can also study maintenance costs by viewing the maintenance ledger entries.</span></span>  

1. <span data-ttu-id="2f249-150">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Основные средства**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-150">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="2f249-151">Выберите основное средство, для которого требуется просмотреть операции книги учета, затем выберите действие **Книги амортизации**.</span><span class="sxs-lookup"><span data-stu-id="2f249-151">Select the fixed asset that you want to view ledger entries for, and then choose the **Depreciation Books** action.</span></span>
3. <span data-ttu-id="2f249-152">В окне **Книги амортизации ОС** выберите книгу амортизации соответствующего основного средства, затем выберите действие **Книга операций по обслуживанию**.</span><span class="sxs-lookup"><span data-stu-id="2f249-152">In the **FA Depreciation Books** window, select the relevant fixed asset depreciation book, and then choose the **Maintenance Ledger Entries** action.</span></span>

## <a name="to-view-or-print-maintenance-ledger-entries-for-multiple-fixed-assets"></a><span data-ttu-id="2f249-153">Просмотр или печатать операций книги обслуживания для нескольких основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-153">To view or print maintenance ledger entries for multiple fixed assets</span></span>
<span data-ttu-id="2f249-154">В отчете **Обслуживание - подробности** можно просмотреть или распечатать операции книги обслуживания для одного или нескольких основных средств.</span><span class="sxs-lookup"><span data-stu-id="2f249-154">In the **Maintenance - Details** report, you can view or print maintenance ledger entries for one or many fixed assets.</span></span>  

1. <span data-ttu-id="2f249-155">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Обслуживание - подробности**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2f249-155">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Maintenance Details**, and then choose the related link.</span></span>
2. <span data-ttu-id="2f249-156">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="2f249-156">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="2f249-157">Нажмите кнопку **Печать** или **Просмотр**.</span><span class="sxs-lookup"><span data-stu-id="2f249-157">Choose the **Print** or **Preview** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="2f249-158">См. также</span><span class="sxs-lookup"><span data-stu-id="2f249-158">See Also</span></span>
[<span data-ttu-id="2f249-159">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="2f249-159">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="2f249-160">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="2f249-160">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="2f249-161">Финансы</span><span class="sxs-lookup"><span data-stu-id="2f249-161">Finance</span></span>](finance.md)  
<span data-ttu-id="2f249-162">[Добро пожаловать в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="2f249-162">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="2f249-163">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2f249-163">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
