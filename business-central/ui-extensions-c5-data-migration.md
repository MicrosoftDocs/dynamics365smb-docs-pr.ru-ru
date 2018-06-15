---
title: "Использование расширения \"Миграция данных C5\" | Microsoft Docs"
description: "Используйте это расширение для переноса клиентов, поставщиков, товаров и счетов главной книги из Microsoft Dynamics C5 2012 в Business Central."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 04/09/208
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: fa6779ee8fb2bbb453014e32cb7f3cf8dcfa18da
ms.openlocfilehash: 698bde6949c6053501881d07135586810fc81bdd
ms.contentlocale: ru-ru
ms.lasthandoff: 04/11/2018

---

# <a name="the-c5-data-migration-extension-for-business-central"></a><span data-ttu-id="4eca7-103">Расширение "Миграция данных C5" для Business Central</span><span class="sxs-lookup"><span data-stu-id="4eca7-103">The C5 Data Migration Extension for Business Central</span></span>
<span data-ttu-id="4eca7-104">Это расширение упрощает перенос клиентов, поставщиков, товаров и ваших счетов главной книги из Microsoft Dynamics C5 2012 в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4eca7-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="4eca7-105">Также можно перенести архивные операции для счетов главной книги.</span><span class="sxs-lookup"><span data-stu-id="4eca7-105">You can also migrate historical entries for general ledger accounts.</span></span>

> [!Note]
> <span data-ttu-id="4eca7-106">Организация в [!INCLUDE[d365fin](includes/d365fin_md.md)] не должна содержать никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4eca7-106">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="4eca7-107">Кроме того, после запуска миграции не создавайте клиентов, поставщиков, товаров или счетов, пока миграция не закончит работу.</span><span class="sxs-lookup"><span data-stu-id="4eca7-107">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="what-data-is-migrated"></a><span data-ttu-id="4eca7-108">Какие данные можно перенести?</span><span class="sxs-lookup"><span data-stu-id="4eca7-108">What Data is Migrated?</span></span>
<span data-ttu-id="4eca7-109">Следующие данные можно перенести для каждого объекта:</span><span class="sxs-lookup"><span data-stu-id="4eca7-109">The following data is migrated for each entity:</span></span>

<span data-ttu-id="4eca7-110">**Клиенты**</span><span class="sxs-lookup"><span data-stu-id="4eca7-110">**Customers**</span></span>
* <span data-ttu-id="4eca7-111">Склады</span><span class="sxs-lookup"><span data-stu-id="4eca7-111">Location</span></span>
* <span data-ttu-id="4eca7-112">Страна</span><span class="sxs-lookup"><span data-stu-id="4eca7-112">Country</span></span>
* <span data-ttu-id="4eca7-113">Измерения клиента (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="4eca7-113">Customer dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="4eca7-114">Метод поставки</span><span class="sxs-lookup"><span data-stu-id="4eca7-114">Shipment method</span></span>
* <span data-ttu-id="4eca7-115">Продавец</span><span class="sxs-lookup"><span data-stu-id="4eca7-115">Sales Person</span></span>
* <span data-ttu-id="4eca7-116">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="4eca7-116">Payment terms</span></span>
* <span data-ttu-id="4eca7-117">Способ оплаты</span><span class="sxs-lookup"><span data-stu-id="4eca7-117">Payment method</span></span>
* <span data-ttu-id="4eca7-118">Ценовая группа клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-118">Customer price group</span></span>
* <span data-ttu-id="4eca7-119">Скидка по счету клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-119">Customer invoice discount</span></span>

<span data-ttu-id="4eca7-120">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="4eca7-120">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="4eca7-121">Настройка учета клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-121">Customer posting setup</span></span>
* <span data-ttu-id="4eca7-122">Раздел финансового журнала</span><span class="sxs-lookup"><span data-stu-id="4eca7-122">General journal batch</span></span>
* <span data-ttu-id="4eca7-123">Открытые транзакции (операции книги клиентов)</span><span class="sxs-lookup"><span data-stu-id="4eca7-123">Open transactions (customer ledger entries)</span></span>

<span data-ttu-id="4eca7-124">**Поставщики**</span><span class="sxs-lookup"><span data-stu-id="4eca7-124">**Vendors**</span></span>
* <span data-ttu-id="4eca7-125">Склады</span><span class="sxs-lookup"><span data-stu-id="4eca7-125">Location</span></span>
* <span data-ttu-id="4eca7-126">Страна</span><span class="sxs-lookup"><span data-stu-id="4eca7-126">Country</span></span>
* <span data-ttu-id="4eca7-127">Измерения поставщика (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="4eca7-127">Vendor dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="4eca7-128">Скидка по счету</span><span class="sxs-lookup"><span data-stu-id="4eca7-128">Invoice discount</span></span>
* <span data-ttu-id="4eca7-129">Метод поставки</span><span class="sxs-lookup"><span data-stu-id="4eca7-129">Shipment method</span></span>
* <span data-ttu-id="4eca7-130">Закупщик</span><span class="sxs-lookup"><span data-stu-id="4eca7-130">Purchaser</span></span>
* <span data-ttu-id="4eca7-131">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="4eca7-131">Payment terms</span></span>
* <span data-ttu-id="4eca7-132">Способ оплаты</span><span class="sxs-lookup"><span data-stu-id="4eca7-132">Payment method</span></span>
* <span data-ttu-id="4eca7-133">Скидка по счету поставщика</span><span class="sxs-lookup"><span data-stu-id="4eca7-133">Vendor invoice discount</span></span>

<span data-ttu-id="4eca7-134">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="4eca7-134">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="4eca7-135">Настройка учета поставщика</span><span class="sxs-lookup"><span data-stu-id="4eca7-135">Vendor posting setup</span></span>
* <span data-ttu-id="4eca7-136">Раздел финансового журнала</span><span class="sxs-lookup"><span data-stu-id="4eca7-136">General journal batch</span></span>
* <span data-ttu-id="4eca7-137">Открытые транзакции (операции книги поставщиков)</span><span class="sxs-lookup"><span data-stu-id="4eca7-137">Open transactions (vendor ledger entries)</span></span>

<span data-ttu-id="4eca7-138">**Товаров**</span><span class="sxs-lookup"><span data-stu-id="4eca7-138">**Items**</span></span>
* <span data-ttu-id="4eca7-139">Склады</span><span class="sxs-lookup"><span data-stu-id="4eca7-139">Location</span></span>
* <span data-ttu-id="4eca7-140">Страна</span><span class="sxs-lookup"><span data-stu-id="4eca7-140">Country</span></span>
* <span data-ttu-id="4eca7-141">Измерения товара (отдел, центр, назначение)</span><span class="sxs-lookup"><span data-stu-id="4eca7-141">Item dimensions (department, center, purpose)</span></span>
* <span data-ttu-id="4eca7-142">Скидки строки продаж</span><span class="sxs-lookup"><span data-stu-id="4eca7-142">Sales line discounts</span></span>
* <span data-ttu-id="4eca7-143">Группы скидок клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-143">Customer discount groups</span></span>
* <span data-ttu-id="4eca7-144">Группы скидок по товару</span><span class="sxs-lookup"><span data-stu-id="4eca7-144">Item discount groups</span></span>
* <span data-ttu-id="4eca7-145">Цена продажи</span><span class="sxs-lookup"><span data-stu-id="4eca7-145">Sales price</span></span>
* <span data-ttu-id="4eca7-146">Код тарифа</span><span class="sxs-lookup"><span data-stu-id="4eca7-146">Tariff number</span></span>
* <span data-ttu-id="4eca7-147">Единицы измерения</span><span class="sxs-lookup"><span data-stu-id="4eca7-147">Units of measure</span></span>
* <span data-ttu-id="4eca7-148">Код трассировки товара</span><span class="sxs-lookup"><span data-stu-id="4eca7-148">Item tracking code</span></span>
* <span data-ttu-id="4eca7-149">Ценовая группа клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-149">Customer price group</span></span>

<span data-ttu-id="4eca7-150">При переносе учетной записи также переносятся следующие данные:</span><span class="sxs-lookup"><span data-stu-id="4eca7-150">If you migrate accounts, the following data is also migrated:</span></span>

* <span data-ttu-id="4eca7-151">Настройка учета запасов</span><span class="sxs-lookup"><span data-stu-id="4eca7-151">Inventory posting setup</span></span>
* <span data-ttu-id="4eca7-152">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="4eca7-152">General posting setup</span></span>
* <span data-ttu-id="4eca7-153">Раздел журнала товаров</span><span class="sxs-lookup"><span data-stu-id="4eca7-153">Item journal batch</span></span>
* <span data-ttu-id="4eca7-154">Открытые транзакции (операции книги товаров)</span><span class="sxs-lookup"><span data-stu-id="4eca7-154">Open transactions (item ledger entries)</span></span>

> [!Note]
> <span data-ttu-id="4eca7-155">При наличии открытых транзакций, использующих иностранные валюты, также переносятся валютные курсы для этих валют.</span><span class="sxs-lookup"><span data-stu-id="4eca7-155">If there are open transactions that use foreign currencies, the exchange rates for those currencies are also migrated.</span></span> <span data-ttu-id="4eca7-156">Другие валютные курсы не переносятся.</span><span class="sxs-lookup"><span data-stu-id="4eca7-156">Other exchange rates are not migrated.</span></span>

<span data-ttu-id="4eca7-157">**План счетов**</span><span class="sxs-lookup"><span data-stu-id="4eca7-157">**Chart of Accounts**</span></span>  
* <span data-ttu-id="4eca7-158">Стандартные измерения: подразделение, центр затрат, назначение</span><span class="sxs-lookup"><span data-stu-id="4eca7-158">Standard dimensions: Department, Cost Center, Purpose</span></span>  
* <span data-ttu-id="4eca7-159">Исторические транзакции ГК</span><span class="sxs-lookup"><span data-stu-id="4eca7-159">Historical G/L transactions</span></span>  

> [!Note]
> <span data-ttu-id="4eca7-160">Исторические транзакции ГК обрабатываются несколько иначе.</span><span class="sxs-lookup"><span data-stu-id="4eca7-160">Historical G/L transactions are treated a little differently.</span></span> <span data-ttu-id="4eca7-161">При переносе данных вы задаете параметр **Текущий период**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-161">When you migrate data you set a **Current Period** parameter.</span></span> <span data-ttu-id="4eca7-162">Этот параметр определяет порядок обработки транзакций ГК.</span><span class="sxs-lookup"><span data-stu-id="4eca7-162">This parameter specifies how to process G/L transactions.</span></span> <span data-ttu-id="4eca7-163">Транзакции после этой даты переносятся по отдельности.</span><span class="sxs-lookup"><span data-stu-id="4eca7-163">Transactions after this date are migrated individually.</span></span> <span data-ttu-id="4eca7-164">Транзакции до этой даты агрегируются по счету и переносятся как единая сумма.</span><span class="sxs-lookup"><span data-stu-id="4eca7-164">Transactions before this date are aggregated per account and migrated as a single amount.</span></span> <span data-ttu-id="4eca7-165">Например, предположим, что были транзакции в 2015, 2016, 2017, 2018 и в поле "Текущий период" вы указали 1 января 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4eca7-165">For example, let's say there are transactions in 2015, 2016, 2017, 2018, and you specify January 01, 2017 in the Current Period field.</span></span> <span data-ttu-id="4eca7-166">Для каждого счета, суммы по транзакциям, имевшим место по 31 декабря 2016 г. включительно, агрегируются в одну строку финансового журнала для каждого счета ГК.</span><span class="sxs-lookup"><span data-stu-id="4eca7-166">For each account, amounts for transactions on or before December 31, 2106, will be aggregated in a single general journal line for each G/L account.</span></span> <span data-ttu-id="4eca7-167">Все транзакции после этой даты будут перенесены по отдельности.</span><span class="sxs-lookup"><span data-stu-id="4eca7-167">All trascations after this date will be migrated individually.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="4eca7-168">Для миграции данных</span><span class="sxs-lookup"><span data-stu-id="4eca7-168">To migrate data</span></span>
<span data-ttu-id="4eca7-169">Для экспорта данных из C5 и импорта их в [!INCLUDE[d365fin](includes/d365fin_md.md)] нужно выполнить всего несколько шагов:</span><span class="sxs-lookup"><span data-stu-id="4eca7-169">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span>  

1. <span data-ttu-id="4eca7-170">В C5, используйте функцию **Экспорт базы данных**, чтобы экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="4eca7-170">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="4eca7-171">Затем отправьте папку экспорта в сжатую (ZIP) папку.</span><span class="sxs-lookup"><span data-stu-id="4eca7-171">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="4eca7-172">В [!INCLUDE[d365fin](includes/d365fin_md.md)] выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Миграция данных**, затем выберите **Миграция данных**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-172">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>  
3. <span data-ttu-id="4eca7-173">Выполните шаги облегчить в мастере настройки.</span><span class="sxs-lookup"><span data-stu-id="4eca7-173">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="4eca7-174">Обязательно выберите в качестве источника данных **Импорт из Microsoft Dynamcis C5 2012**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-174">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note]
> <span data-ttu-id="4eca7-175">Организации часто добавляют поля для настройки C5 для определенной сферы деятельности.</span><span class="sxs-lookup"><span data-stu-id="4eca7-175">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="4eca7-176"> не производит миграцию данных из настраиваемых полей.</span><span class="sxs-lookup"><span data-stu-id="4eca7-176"> does not migrate data from custom fields.</span></span> <span data-ttu-id="4eca7-177">Кроме того, миграция потерпит неудачу, если имеется более 10 настраиваемых полей.</span><span class="sxs-lookup"><span data-stu-id="4eca7-177">Also, migration will fail if you have more than 10 custom fields.</span></span>

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="4eca7-178">Просмотр состояния миграции</span><span class="sxs-lookup"><span data-stu-id="4eca7-178">Viewing the Status of the Migration</span></span>
<span data-ttu-id="4eca7-179">Используйте страницу **Обзор миграции данных** для контроля успешности миграции.</span><span class="sxs-lookup"><span data-stu-id="4eca7-179">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="4eca7-180">На этой странице отображается такая информация, как количество объектов, которые будут включены в миграцию, состояние миграции, количество элементов, для который была произведена миграция, и была ли эта миграция успешной.</span><span class="sxs-lookup"><span data-stu-id="4eca7-180">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="4eca7-181">Также отображается число ошибок, позволяет вам определить, что пошло неправильно, и, когда это возможно, позволяет легко перейти к объекту для устранения проблем.</span><span class="sxs-lookup"><span data-stu-id="4eca7-181">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="4eca7-182">Дополнительные сведения см. в следующем разделе этой статьи.</span><span class="sxs-lookup"><span data-stu-id="4eca7-182">For more information, see the next section in this topic.</span></span>  

> [!Note]
> <span data-ttu-id="4eca7-183">Пока результаты миграции еще ожидаются, следует обновить страницу для отображения результатов.</span><span class="sxs-lookup"><span data-stu-id="4eca7-183">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="how-to-avoid-double-posting"></a><span data-ttu-id="4eca7-184">Как избежать двойного учета</span><span class="sxs-lookup"><span data-stu-id="4eca7-184">How to Avoid Double-Posting</span></span>
<span data-ttu-id="4eca7-185">Во избежание двойного учета в главной книге для открытых транзакций используются следующие балансовые счета:</span><span class="sxs-lookup"><span data-stu-id="4eca7-185">To help avoid double-posting to the general ledger, the following balance accounts are used for open transactions:</span></span>  
  
* <span data-ttu-id="4eca7-186">Для поставщиков используется счет кредиторской задолженности из учетной группы поставщиков.</span><span class="sxs-lookup"><span data-stu-id="4eca7-186">For vendors, we use the A/P account from the vendor posting group.</span></span>  
* <span data-ttu-id="4eca7-187">Для клиентов используется счет дебиторской задолженности из учетной группы клиентов.</span><span class="sxs-lookup"><span data-stu-id="4eca7-187">For customers, we use the A/R account from the customer posting group.</span></span>  
* <span data-ttu-id="4eca7-188">Для товаров мы создаем настройку общего учета, в которой счет корректировки — это счет, указанный в качестве товарного счета в настройке учета запасов.</span><span class="sxs-lookup"><span data-stu-id="4eca7-188">For items, we create a general posting setup where the adjustment account is the account specified as the inventory account on the inventory posting setup.</span></span>  

## <a name="correcting-errors"></a><span data-ttu-id="4eca7-189">Исправление ошибок</span><span class="sxs-lookup"><span data-stu-id="4eca7-189">Correcting Errors</span></span>
<span data-ttu-id="4eca7-190">Если что-то пошло не так и возникли ошибки, в поле **Состояние** отображается **Завершено с ошибками**, а в поле **Число ошибок** отображается количество ошибок.</span><span class="sxs-lookup"><span data-stu-id="4eca7-190">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="4eca7-191">Для просмотра списка ошибок можно открыть страницу **Ошибки миграции данных**, выбрав:</span><span class="sxs-lookup"><span data-stu-id="4eca7-191">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>  

* <span data-ttu-id="4eca7-192">Номер в поле **Число ошибок** для объекта.</span><span class="sxs-lookup"><span data-stu-id="4eca7-192">The number in the **Error Count** field for the entity.</span></span>  
* <span data-ttu-id="4eca7-193">Объект, затем действие **Показать ошибки**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-193">The entity, and then the **Show Errors** action.</span></span>  

<span data-ttu-id="4eca7-194">На странице **Ошибки миграции данных** чтобы исправить ошибку, можно выбрать сообщение об ошибке, затем выбрать **Изменить запись** для открытия страницы, которая показывает перенесенные данные для объекта.</span><span class="sxs-lookup"><span data-stu-id="4eca7-194">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="4eca7-195">После исправления одной или нескольких ошибок можно выбрать **Миграция**, чтобы выполнить перенос только исправленных объектов, без необходимости полного повторного выполнения миграции.</span><span class="sxs-lookup"><span data-stu-id="4eca7-195">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="4eca7-196">Если исправлено несколько ошибок, можно использовать функцию **Выбрать больше**, чтобы выбрать несколько строк для миграции.</span><span class="sxs-lookup"><span data-stu-id="4eca7-196">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="4eca7-197">Если же ошибки не важны и их можно не исправлять, можно выбрать их, затем выбрать **Пропустить выбранные элементы**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-197">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="4eca7-198">Если имеются товары, которые включены в спецификацию, может возникнуть необходимость выполнить миграцию несколько раз, если исходный товар не был создан до вариантов, которые ссылаются на него.</span><span class="sxs-lookup"><span data-stu-id="4eca7-198">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="4eca7-199">Если сначала создается вариант товара, то ссылка на исходный товару может привести к появлению сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4eca7-199">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="4eca7-200">Проверка данных после миграции</span><span class="sxs-lookup"><span data-stu-id="4eca7-200">Verifying Data After Migrating</span></span>
<span data-ttu-id="4eca7-201">Если требуется проверять правильность миграции данных, можно просмотреть следующие страницы в C5 и [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4eca7-201">One way to verify that your data migrated correctly is to look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="4eca7-202">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="4eca7-202">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]| <span data-ttu-id="4eca7-203">Используемое пакетное задание</span><span class="sxs-lookup"><span data-stu-id="4eca7-203">Batch Job to Use</span></span> |
|-----|-----|-----|
|<span data-ttu-id="4eca7-204">Объекты клиента</span><span class="sxs-lookup"><span data-stu-id="4eca7-204">Customer Entries</span></span>| <span data-ttu-id="4eca7-205">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="4eca7-205">General Journals</span></span>| <span data-ttu-id="4eca7-206">CUSTMIGR</span><span class="sxs-lookup"><span data-stu-id="4eca7-206">CUSTMIGR</span></span> |
|<span data-ttu-id="4eca7-207">Объекты поставщика</span><span class="sxs-lookup"><span data-stu-id="4eca7-207">Vendor Entries</span></span>| <span data-ttu-id="4eca7-208">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="4eca7-208">General Journals</span></span>| <span data-ttu-id="4eca7-209">VENDMIGR</span><span class="sxs-lookup"><span data-stu-id="4eca7-209">VENDMIGR</span></span>|
|<span data-ttu-id="4eca7-210">Операции товара</span><span class="sxs-lookup"><span data-stu-id="4eca7-210">Item Entries</span></span>| <span data-ttu-id="4eca7-211">Журналы товаров</span><span class="sxs-lookup"><span data-stu-id="4eca7-211">Item Journals</span></span>| <span data-ttu-id="4eca7-212">ITEMMIGR</span><span class="sxs-lookup"><span data-stu-id="4eca7-212">ITEMMIGR</span></span> |
|<span data-ttu-id="4eca7-213">Операции ГК</span><span class="sxs-lookup"><span data-stu-id="4eca7-213">G/L Entries</span></span>| <span data-ttu-id="4eca7-214">Финансовые журналы</span><span class="sxs-lookup"><span data-stu-id="4eca7-214">General Journals</span></span>| <span data-ttu-id="4eca7-215">GLACMIGR</span><span class="sxs-lookup"><span data-stu-id="4eca7-215">GLACMIGR</span></span> |

## <a name="stopping-data-migration"></a><span data-ttu-id="4eca7-216">Остановка миграции данных</span><span class="sxs-lookup"><span data-stu-id="4eca7-216">Stopping Data Migration</span></span>
<span data-ttu-id="4eca7-217">Можно остановить миграцию данных, выбрав **Остановить все операции миграции**.</span><span class="sxs-lookup"><span data-stu-id="4eca7-217">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="4eca7-218">Если это сделать, все ожидающие операции миграции также будут остановлены.</span><span class="sxs-lookup"><span data-stu-id="4eca7-218">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="4eca7-219">См. также</span><span class="sxs-lookup"><span data-stu-id="4eca7-219">See Also</span></span>
<span data-ttu-id="4eca7-220">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="4eca7-220">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="4eca7-221">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="4eca7-221">Getting Started</span></span>](product-get-started.md) 

