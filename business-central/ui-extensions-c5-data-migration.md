---
title: Использование расширения "Миграция данных C5" | Документация Майкрософт
description: Используйте это расширение для переноса клиентов, поставщиков, товаров и счетов главной книги из Microsoft Dynamics C5 2012 в Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 07/23/2020
ms.author: bholtorf
ms.openlocfilehash: d52b04f000617ac037ccc37bcf02061609e680c6
ms.sourcegitcommit: 7b5c927ea9a59329daf1b60633b8290b552d6531
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "3617840"
---
# <a name="the-c5-data-migration-extension"></a><span data-ttu-id="837b7-103">Расширение миграции данных C5</span><span class="sxs-lookup"><span data-stu-id="837b7-103">The C5 Data Migration Extension</span></span>

<span data-ttu-id="837b7-104">Это расширение упрощает перенос клиентов, поставщиков, товаров и ваших счетов главной книги из Microsoft Dynamics C5 2012 в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="837b7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamics C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="837b7-105">Также можно перенести архивные операции для счетов главной книги.</span><span class="sxs-lookup"><span data-stu-id="837b7-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="837b7-106">Организация в [!INCLUDE[d365fin](includes/d365fin_md.md)] не должна содержать никаких данных.</span><span class="sxs-lookup"><span data-stu-id="837b7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="837b7-107">Кроме того, после запуска миграции не создавайте клиентов, поставщиков, товаров или счетов, пока миграция не закончит работу.</span><span class="sxs-lookup"><span data-stu-id="837b7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="837b7-108">Какие данные можно перенести?</span><span class="sxs-lookup"><span data-stu-id="837b7-108">What Data is Migrated?</span></span>
<span data-ttu-id="837b7-109">Следующие данные можно перенести для каждого объекта:</span><span class="sxs-lookup"><span data-stu-id="837b7-109">The following data is migrated for each entity:</span></span>

### <a name="customers"></a><span data-ttu-id="837b7-110">Клиенты</span><span class="sxs-lookup"><span data-stu-id="837b7-110">Customers</span></span>

* <span data-ttu-id="837b7-111">Контакты</span><span class="sxs-lookup"><span data-stu-id="837b7-111">Contacts</span></span>  
* <span data-ttu-id="837b7-112">Склады</span><span class="sxs-lookup"><span data-stu-id="837b7-112">Location</span></span>
* <span data-ttu-id="837b7-113">Страна</span><span class="sxs-lookup"><span data-stu-id="837b7-113">Country</span></span>
* <span data-ttu-id="837b7-114">Измерения клиента (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="837b7-114">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="837b7-115">Метод поставки</span><span class="sxs-lookup"><span data-stu-id="837b7-115">Shipment method</span></span>
* <span data-ttu-id="837b7-116">Продавец</span><span class="sxs-lookup"><span data-stu-id="837b7-116">Sales Person</span></span>
* <span data-ttu-id="837b7-117">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="837b7-117">Payment terms</span></span>
* <span data-ttu-id="837b7-118">Способ оплаты</span><span class="sxs-lookup"><span data-stu-id="837b7-118">Payment method</span></span>
* <span data-ttu-id="837b7-119">Ценовая группа клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-119">Customer price group</span></span>
* <span data-ttu-id="837b7-120">Скидка по счету клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-120">Customer invoice discount</span></span>

<span data-ttu-id="837b7-121">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="837b7-121">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="837b7-122">Настройка учета клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-122">Customer posting setup</span></span>
* <span data-ttu-id="837b7-123">Раздел финансового журнала</span><span class="sxs-lookup"><span data-stu-id="837b7-123">General journal batch</span></span>
* <span data-ttu-id="837b7-124">Открытые транзакции (операции книги клиентов)</span><span class="sxs-lookup"><span data-stu-id="837b7-124">Open transactions (customer ledger entries)</span></span>

### <a name="vendors"></a><span data-ttu-id="837b7-125">Поставщики</span><span class="sxs-lookup"><span data-stu-id="837b7-125">Vendors</span></span>

* <span data-ttu-id="837b7-126">Контакты</span><span class="sxs-lookup"><span data-stu-id="837b7-126">Contacts</span></span>
* <span data-ttu-id="837b7-127">Склады</span><span class="sxs-lookup"><span data-stu-id="837b7-127">Location</span></span>
* <span data-ttu-id="837b7-128">Страна</span><span class="sxs-lookup"><span data-stu-id="837b7-128">Country</span></span>
* <span data-ttu-id="837b7-129">Измерения поставщика (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="837b7-129">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="837b7-130">Скидка по счету</span><span class="sxs-lookup"><span data-stu-id="837b7-130">Invoice discount</span></span>
* <span data-ttu-id="837b7-131">Метод поставки</span><span class="sxs-lookup"><span data-stu-id="837b7-131">Shipment method</span></span>
* <span data-ttu-id="837b7-132">Закупщик</span><span class="sxs-lookup"><span data-stu-id="837b7-132">Purchaser</span></span>
* <span data-ttu-id="837b7-133">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="837b7-133">Payment terms</span></span>
* <span data-ttu-id="837b7-134">Способ оплаты</span><span class="sxs-lookup"><span data-stu-id="837b7-134">Payment method</span></span>
* <span data-ttu-id="837b7-135">Скидка по счету поставщика</span><span class="sxs-lookup"><span data-stu-id="837b7-135">Vendor invoice discount</span></span>

<span data-ttu-id="837b7-136">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="837b7-136">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="837b7-137">Настройка учета поставщика</span><span class="sxs-lookup"><span data-stu-id="837b7-137">Vendor posting setup</span></span>
* <span data-ttu-id="837b7-138">Раздел финансового журнала</span><span class="sxs-lookup"><span data-stu-id="837b7-138">General journal batch</span></span>
* <span data-ttu-id="837b7-139">Открытые транзакции (операции книги поставщиков)</span><span class="sxs-lookup"><span data-stu-id="837b7-139">Open transactions (vendor ledger entries)</span></span>

### <a name="items"></a><span data-ttu-id="837b7-140">Товаров</span><span class="sxs-lookup"><span data-stu-id="837b7-140">Items</span></span>

* <span data-ttu-id="837b7-141">Склады</span><span class="sxs-lookup"><span data-stu-id="837b7-141">Location</span></span>
* <span data-ttu-id="837b7-142">Страна</span><span class="sxs-lookup"><span data-stu-id="837b7-142">Country</span></span>
* <span data-ttu-id="837b7-143">Измерения товара (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="837b7-143">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="837b7-144">Скидки строки продаж</span><span class="sxs-lookup"><span data-stu-id="837b7-144">Sales line discounts</span></span>
* <span data-ttu-id="837b7-145">Группы скидок клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-145">Customer discount groups</span></span>
* <span data-ttu-id="837b7-146">Группы скидок по товару</span><span class="sxs-lookup"><span data-stu-id="837b7-146">Item discount groups</span></span>
* <span data-ttu-id="837b7-147">Цена продажи</span><span class="sxs-lookup"><span data-stu-id="837b7-147">Sales price</span></span>
* <span data-ttu-id="837b7-148">Код тарифа</span><span class="sxs-lookup"><span data-stu-id="837b7-148">Tariff number</span></span>
* <span data-ttu-id="837b7-149">Единицы измерения</span><span class="sxs-lookup"><span data-stu-id="837b7-149">Units of measure</span></span>
* <span data-ttu-id="837b7-150">Код трассировки товара</span><span class="sxs-lookup"><span data-stu-id="837b7-150">Item tracking code</span></span>
* <span data-ttu-id="837b7-151">Ценовая группа клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-151">Customer price group</span></span>
* <span data-ttu-id="837b7-152">Сборочные спецификации</span><span class="sxs-lookup"><span data-stu-id="837b7-152">Assembly BOMs</span></span>

<span data-ttu-id="837b7-153">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="837b7-153">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="837b7-154">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="837b7-154">Inventory posting setup</span></span>
* <span data-ttu-id="837b7-155">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="837b7-155">General posting setup</span></span>
* <span data-ttu-id="837b7-156">Раздел журнала товаров</span><span class="sxs-lookup"><span data-stu-id="837b7-156">Item journal batch</span></span>
* <span data-ttu-id="837b7-157">Открытые транзакции (операции книги товаров)</span><span class="sxs-lookup"><span data-stu-id="837b7-157">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="837b7-158">При наличии открытых транзакций, использующих иностранные валюты, также переносятся валютные курсы для этих валют.</span><span class="sxs-lookup"><span data-stu-id="837b7-158">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="837b7-159">Другие валютные курсы не переносятся.</span><span class="sxs-lookup"><span data-stu-id="837b7-159">Other exchange rates are not migrated.</span></span>

### <a name="chart-of-accounts"></a><span data-ttu-id="837b7-160">План счетов</span><span class="sxs-lookup"><span data-stu-id="837b7-160">Chart of Accounts</span></span>

* <span data-ttu-id="837b7-161">Стандартные измерения: подразделение, центр затрат, назначение</span><span class="sxs-lookup"><span data-stu-id="837b7-161">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="837b7-162">Исторические транзакции ГК</span><span class="sxs-lookup"><span data-stu-id="837b7-162">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="837b7-163">Исторические транзакции ГК обрабатываются несколько иначе.</span><span class="sxs-lookup"><span data-stu-id="837b7-163">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="837b7-164">При переносе данных вы задаете параметр **Текущий период**.</span><span class="sxs-lookup"><span data-stu-id="837b7-164">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="837b7-165">Этот параметр определяет порядок обработки транзакций ГК.</span><span class="sxs-lookup"><span data-stu-id="837b7-165">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="837b7-166">Транзакции после этой даты переносятся по отдельности.</span><span class="sxs-lookup"><span data-stu-id="837b7-166">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="837b7-167">Транзакции до этой даты агрегируются по счету и переносятся как единая сумма.</span><span class="sxs-lookup"><span data-stu-id="837b7-167">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="837b7-168">Например, предположим, что были транзакции в 2015, 2016, 2017, 2018 и в поле "Текущий период" вы указали 1 января 2017 г.</span><span class="sxs-lookup"><span data-stu-id="837b7-168">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="837b7-169">Для каждого счета, суммы по транзакциям, имевшим место по 31 декабря 2016 г. включительно, агрегируются в одну строку финансового журнала для каждого счета ГК.</span><span class="sxs-lookup"><span data-stu-id="837b7-169">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="837b7-170">Все транзакции после этой даты будут перенесены по отдельности.</span><span class="sxs-lookup"><span data-stu-id="837b7-170">All transactions after this date will be migrated individually.</span></span>

## <a name="file-size-requirements"></a><span data-ttu-id="837b7-171">Требования к размеру файла</span><span class="sxs-lookup"><span data-stu-id="837b7-171">File Size Requirements</span></span>

<span data-ttu-id="837b7-172">Максимальный размер файла, который можно загружать в [!INCLUDE[d365fin](includes/d365fin_md.md)], равен 150 МБ.</span><span class="sxs-lookup"><span data-stu-id="837b7-172">The largest file size you can upload to [!INCLUDE[d365fin](includes/d365fin_md.md)] is 150 MB.</span></span> <span data-ttu-id="837b7-173">Если размер экспортированного из C5 файла больше, попробуйте выполнить перенос данных в нескольких файлах.</span><span class="sxs-lookup"><span data-stu-id="837b7-173">If the file you export from C5 is larger than that, consider migrating data in multiple files.</span></span> <span data-ttu-id="837b7-174">Например, экспортируйте из C5 сущности одного или двух типов, например, клиентов и поставщиков, в файл, затем экспортируйте товары в другой файл, и так далее.</span><span class="sxs-lookup"><span data-stu-id="837b7-174">For example, export one or two types of entities from C5, such as customers and vendors, to a file, and then export items to another file, and so on.</span></span> <span data-ttu-id="837b7-175">Можно импортировать файлы индивидуально в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="837b7-175">You can import files individually in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="837b7-176">Для миграции данных</span><span class="sxs-lookup"><span data-stu-id="837b7-176">To migrate data</span></span>

<span data-ttu-id="837b7-177">Для экспорта данных из C5 и импорта их в [!INCLUDE[d365fin](includes/d365fin_md.md)] нужно выполнить всего несколько шагов:</span><span class="sxs-lookup"><span data-stu-id="837b7-177">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="837b7-178">В C5, используйте функцию **Экспорт базы данных**, чтобы экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="837b7-178">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="837b7-179">Затем отправьте папку экспорта в сжатую (ZIP) папку.</span><span class="sxs-lookup"><span data-stu-id="837b7-179">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="837b7-180">В [!INCLUDE[d365fin](includes/d365fin_md.md)] выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Миграция данных**, затем выберите **Миграция данных**.</span><span class="sxs-lookup"><span data-stu-id="837b7-180">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="837b7-181">Выполните шаги облегчить в мастере настройки.</span><span class="sxs-lookup"><span data-stu-id="837b7-181">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="837b7-182">Обязательно выберите в качестве источника данных **Импорт из Microsoft Dynamcis C5 2012**.</span><span class="sxs-lookup"><span data-stu-id="837b7-182">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="837b7-183">Просмотр состояния миграции</span><span class="sxs-lookup"><span data-stu-id="837b7-183">Viewing the Status of the Migration</span></span>

<span data-ttu-id="837b7-184">Используйте страницу **Обзор миграции данных** для контроля успешности миграции.</span><span class="sxs-lookup"><span data-stu-id="837b7-184">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="837b7-185">На этой странице отображается такая информация, как количество объектов, которые будут включены в миграцию, состояние миграции, количество элементов, для который была произведена миграция, и была ли эта миграция успешной.</span><span class="sxs-lookup"><span data-stu-id="837b7-185">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="837b7-186">Также отображается число ошибок, позволяет вам определить, что пошло неправильно, и, когда это возможно, позволяет легко перейти к объекту для устранения проблем.</span><span class="sxs-lookup"><span data-stu-id="837b7-186">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="837b7-187">Дополнительные сведения см. в следующем разделе этой статьи.</span><span class="sxs-lookup"><span data-stu-id="837b7-187">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="837b7-188">Пока результаты миграции еще ожидаются, следует обновить страницу для отображения результатов.</span><span class="sxs-lookup"><span data-stu-id="837b7-188">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="837b7-189">Как избежать двойного учета</span><span class="sxs-lookup"><span data-stu-id="837b7-189">How to Avoid Double-Posting</span></span>

<span data-ttu-id="837b7-190">Во избежание двойного учета в главной книге для открытых транзакций используются следующие балансовые счета:</span><span class="sxs-lookup"><span data-stu-id="837b7-190">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  

* <span data-ttu-id="837b7-191">Для поставщиков используется счет кредиторской задолженности из учетной группы поставщиков.</span><span class="sxs-lookup"><span data-stu-id="837b7-191">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="837b7-192">Для клиентов используется счет дебиторской задолженности из учетной группы клиентов.</span><span class="sxs-lookup"><span data-stu-id="837b7-192">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="837b7-193">Для товаров мы создаем настройку общего учета, в которой счет корректировки — это счет, указанный в качестве товарного счета в настройке учета запасов.</span><span class="sxs-lookup"><span data-stu-id="837b7-193">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="837b7-194">Исправление ошибок</span><span class="sxs-lookup"><span data-stu-id="837b7-194">Correcting Errors</span></span>

<span data-ttu-id="837b7-195">Если что-то пошло не так и возникли ошибки, в поле **Состояние** отображается **Завершено с ошибками**, а в поле **Число ошибок** отображается количество ошибок.</span><span class="sxs-lookup"><span data-stu-id="837b7-195">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="837b7-196">Для просмотра списка ошибок можно открыть страницу **Ошибки миграции данных**, выбрав:</span><span class="sxs-lookup"><span data-stu-id="837b7-196">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="837b7-197">Номер в поле **Число ошибок** для объекта.</span><span class="sxs-lookup"><span data-stu-id="837b7-197">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="837b7-198">Объект, затем действие **Показать ошибки**.</span><span class="sxs-lookup"><span data-stu-id="837b7-198">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="837b7-199">На странице **Ошибки миграции данных** чтобы исправить ошибку, можно выбрать сообщение об ошибке, затем выбрать **Изменить запись** для просмотра перенесенных данных для объекта.</span><span class="sxs-lookup"><span data-stu-id="837b7-199">On the **Data Migration Errors** page, to fix an error you can choose an error message, and then choose **Edit Record** to view the migrated data for the entity.</span></span> <span data-ttu-id="837b7-200">Если имеется несколько ошибок, которые необходимо исправить, можно выбрать **Пакетное устранение ошибок** для редактирования объектов в списке.</span><span class="sxs-lookup"><span data-stu-id="837b7-200">If you have several errors to fix, you can choose **Bulk-Fix Errors** to edit the entities in a list.</span></span> <span data-ttu-id="837b7-201">Однако все равно необходимо открыть индивидуальные записи, если ошибка является следствием связанной записи.</span><span class="sxs-lookup"><span data-stu-id="837b7-201">You still need to open individual records if the error was caused by a related entry though.</span></span> <span data-ttu-id="837b7-202">Например, поставщик не будет перенесен, если адрес электронной почты одного из его контактов имеет неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="837b7-202">For example, a vendor will not be migrated if an email address one of their contacts has an invalid format.</span></span>

<span data-ttu-id="837b7-203">После исправления одной или нескольких ошибок можно выбрать **Миграция**, чтобы выполнить перенос только исправленных объектов, без необходимости полного повторного выполнения миграции.</span><span class="sxs-lookup"><span data-stu-id="837b7-203">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="837b7-204">Если исправлено несколько ошибок, можно использовать функцию **Выбрать больше**, чтобы выбрать несколько строк для миграции.</span><span class="sxs-lookup"><span data-stu-id="837b7-204">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="837b7-205">Если же ошибки не важны и их можно не исправлять, можно выбрать их, затем выбрать **Пропустить выбранные элементы**.</span><span class="sxs-lookup"><span data-stu-id="837b7-205">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="837b7-206">Если имеются товары, которые включены в спецификацию, может возникнуть необходимость выполнить миграцию несколько раз, если исходный товар не был создан до вариантов, которые ссылаются на него.</span><span class="sxs-lookup"><span data-stu-id="837b7-206">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="837b7-207">Если сначала создается вариант товара, то ссылка на исходный товару может привести к появлению сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="837b7-207">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="837b7-208">Проверка данных после миграции</span><span class="sxs-lookup"><span data-stu-id="837b7-208">Verifying Data After Migrating</span></span>

<span data-ttu-id="837b7-209">Если требуется проверять правильность миграции данных, можно просмотреть следующие страницы в C5 и [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="837b7-209">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="837b7-210">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="837b7-210">Microsoft Dynamics C5 2012</span></span> | <span data-ttu-id="837b7-211">Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="837b7-211">Dynamics 365 Business Central</span></span>| <span data-ttu-id="837b7-212">Используемое пакетное задание</span><span class="sxs-lookup"><span data-stu-id="837b7-212">Batch Job to Use</span></span> |
|---------------------------|------------------------------|------------------|
|<span data-ttu-id="837b7-213">Объекты клиента</span><span class="sxs-lookup"><span data-stu-id="837b7-213">Customer Entries</span></span>| <span data-ttu-id="837b7-214">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="837b7-214">General Journals</span></span>| <span data-ttu-id="837b7-215">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="837b7-215">CUSTMIGR</span></span> |
|<span data-ttu-id="837b7-216">Объекты поставщика</span><span class="sxs-lookup"><span data-stu-id="837b7-216">Vendor Entries</span></span>| <span data-ttu-id="837b7-217">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="837b7-217">General Journals</span></span>| <span data-ttu-id="837b7-218">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="837b7-218">VENDMIGR</span></span>|
|<span data-ttu-id="837b7-219">Операции товара</span><span class="sxs-lookup"><span data-stu-id="837b7-219">Item Entries</span></span>| <span data-ttu-id="837b7-220">Журналы товаров</span><span class="sxs-lookup"><span data-stu-id="837b7-220">Item Journals</span></span>| <span data-ttu-id="837b7-221">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="837b7-221">ITEMMIGR</span></span> |
|<span data-ttu-id="837b7-222">Операции ГК</span><span class="sxs-lookup"><span data-stu-id="837b7-222">G/L Entries</span></span>| <span data-ttu-id="837b7-223">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="837b7-223">General Journals</span></span>| <span data-ttu-id="837b7-224">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="837b7-224">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="837b7-225">Остановка миграции данных</span><span class="sxs-lookup"><span data-stu-id="837b7-225">Stopping Data Migration</span></span>

<span data-ttu-id="837b7-226">Можно остановить миграцию данных, выбрав **Остановить все операции миграции**.</span><span class="sxs-lookup"><span data-stu-id="837b7-226">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="837b7-227">Если это сделать, все ожидающие операции миграции также будут остановлены.</span><span class="sxs-lookup"><span data-stu-id="837b7-227">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="837b7-228">См. также</span><span class="sxs-lookup"><span data-stu-id="837b7-228">See Also</span></span>

<span data-ttu-id="837b7-229">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="837b7-229">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="837b7-230">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="837b7-230">Getting Started</span></span>](product-get-started.md)  
