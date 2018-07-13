---
title: "Использование Excel для импорта данных в Business Central | Microsoft Docs"
description: "Используйте пакет конфигурации по умолчанию для добавления данных в Excel и импорта данных обратно в Business Central."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 05/17/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2286b728a464943841b192031cfea13644441013
ms.openlocfilehash: 45a236dfeb7a5ce489cf8917d6a08a92ca5c4e8b
ms.contentlocale: ru-ru
ms.lasthandoff: 06/28/2018

---
# <a name="importing-business-data-from-other-finance-systems"></a><span data-ttu-id="27f0f-103">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="27f0f-103">Importing Business Data from Other Finance Systems</span></span>
<span data-ttu-id="27f0f-104">При регистрации в [!INCLUDE[d365fin](includes/d365fin_md.md)] вы можете создать пустую организации, чтоб загрузить собственные данные и протестировать новую организацию [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="27f0f-104">When you sign up for [!INCLUDE[d365fin](includes/d365fin_md.md)], you can choose to create an empty company so that you can upload your own data and to test your new [!INCLUDE[d365fin](includes/d365fin_md.md)] company.</span></span> <span data-ttu-id="27f0f-105">В зависимости от финансового решения, которое вы используете сейчас, вы можете перенести информацию о клиентах, поставщиках, запасах и банковских счетах.</span><span class="sxs-lookup"><span data-stu-id="27f0f-105">Depending on the finance solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.</span></span>  

<span data-ttu-id="27f0f-106">Из ролевого центра вы можете запустить руководство по настройке, помогающее перенести бизнес-данные из файла Excel или из других форматов.</span><span class="sxs-lookup"><span data-stu-id="27f0f-106">From the Role Center, you can start an assisted setup guide that helps you transfer the business data from an Excel file or from other formats.</span></span> <span data-ttu-id="27f0f-107">Тип файлов, которые можно загружать, зависит от доступных расширений.</span><span class="sxs-lookup"><span data-stu-id="27f0f-107">The type of files you can upload depends on the extensions that are available.</span></span> <span data-ttu-id="27f0f-108">Например, вы можете перенести данные из QuickBooks, поскольку [!INCLUDE[d365fin](includes/d365fin_md.md)] включает расширение, которое обрабатывает преобразование из QuickBooks.</span><span class="sxs-lookup"><span data-stu-id="27f0f-108">For example, you can migrate data from QuickBooks because [!INCLUDE[d365fin](includes/d365fin_md.md)] includes an extension that handles the conversion from QuickBooks.</span></span> <span data-ttu-id="27f0f-109">Если вам нужно перенести данные из других финансовых решений, вы должны проверить, есть ли расширение для этого решения, или импортировать из Excel.</span><span class="sxs-lookup"><span data-stu-id="27f0f-109">If you want to migrate data from other finance solutions, you must either check if an extension is available for that solution or import from Excel.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="27f0f-110"> включает шаблоны для счетов, клиентов, поставщиков и складских товаров, которые можно выбрать для применения при импорте данных.</span><span class="sxs-lookup"><span data-stu-id="27f0f-110"> includes templates for accounts, customers, vendors, and inventory items that you can choose to apply when you import your data.</span></span>

<span data-ttu-id="27f0f-111">Можно импортировать основные данные и некоторые транзакционные данные из других финансовых систем на основе пакета конфигурации по умолчанию в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="27f0f-111">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="27f0f-112">В окне **Пакеты конфигураций** можно использовать пакет для импорта и проверки данных перед применением пакета.</span><span class="sxs-lookup"><span data-stu-id="27f0f-112">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span></span>  

> [!TIP]  
> <span data-ttu-id="27f0f-113">Кроме того, можно использовать мастеры миграции данных для импорта данных из QuickBooks или Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="27f0f-113">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span></span> <span data-ttu-id="27f0f-114">Дополнительные сведения см. в разделе [Миграция данных QuickBooks](ui-extensions-quickbooks-data-migration.md) или [Миграция данных Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="27f0f-114">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span></span>

> [!NOTE]  
> <span data-ttu-id="27f0f-115">Для более крупной работы по реализации можно использовать службы RapidStart Services для [!INCLUDE[d365fin](includes/d365fin_md.md)], которые представляют собой обширный набор средств для настройки новых решений, основанных на бизнес-требованиях и данных настройки клиентов.</span><span class="sxs-lookup"><span data-stu-id="27f0f-115">For larger implementation work, you can use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], which is an extensive toolkit for setting up new solutions based on customers' business requirements and setup data.</span></span> <span data-ttu-id="27f0f-116">Службы RapidStart Services также предоставляют функциональные возможности для импорта бизнес-данных.</span><span class="sxs-lookup"><span data-stu-id="27f0f-116">RapidStart Services also offers functionality for import of business data.</span></span> <span data-ttu-id="27f0f-117">Дополнительные сведения см. в разделе [Настройка организации со службами RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span><span class="sxs-lookup"><span data-stu-id="27f0f-117">For more information, see [Setting Up a Company With RapidStart Services](admin-set-up-a-company-with-rapidstart.md).</span></span>

## <a name="importing-data-from-configuration-packages"></a><span data-ttu-id="27f0f-118">Импорт данных из пакетов конфигураций</span><span class="sxs-lookup"><span data-stu-id="27f0f-118">Importing Data from Configuration Packages</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="27f0f-119"> включает пакет конфигурации, который можно экспортировать в Excel, а затем настроить там данные.</span><span class="sxs-lookup"><span data-stu-id="27f0f-119"> includes a configuration package that you can export to Excel and set up your data there.</span></span> <span data-ttu-id="27f0f-120">После этого можно импортировать данные обратно из Excel.</span><span class="sxs-lookup"><span data-stu-id="27f0f-120">Then, you can import the data from Excel again.</span></span> <span data-ttu-id="27f0f-121">Пакет состоит из 27 таблиц, включая основные данные, такие как клиенты, поставщики, товары и счета, другие таблицы настройки, такие как методы отгрузки, и таблицы транзакций, такие как заголовок и строки продаж.</span><span class="sxs-lookup"><span data-stu-id="27f0f-121">The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="27f0f-122">Работа с пакетами конфигураций — расширенная функция, и рекомендуется связаться с администратором.</span><span class="sxs-lookup"><span data-stu-id="27f0f-122">Working with configuration packages is advanced functionality, and we recommend that you contact your administrator.</span></span> <span data-ttu-id="27f0f-123">Дополнительные сведения см. в разделе [Импорт данных из устаревшего ПО учета с использованием пакета конфигурации](across-import-data-configuration-packages.md).</span><span class="sxs-lookup"><span data-stu-id="27f0f-123">For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).</span></span>

## <a name="working-with-data-in-excel"></a><span data-ttu-id="27f0f-124">Работа с данными в Excel</span><span class="sxs-lookup"><span data-stu-id="27f0f-124">Working with Data in Excel</span></span>
<span data-ttu-id="27f0f-125">При экспорте пакета конфигурации по умолчанию в Excel созданная книга содержит лист для каждой таблицы в пакете.</span><span class="sxs-lookup"><span data-stu-id="27f0f-125">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="27f0f-126">Чтобы упростить задачи, можно воспользоваться преимуществами инструментов управления XML, которые встроены в Excel.</span><span class="sxs-lookup"><span data-stu-id="27f0f-126">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="27f0f-127">Также можно воспользоваться встроенными функциями Excel, чтобы помочь с форматом данных и поместить данные в правильную ячейку.</span><span class="sxs-lookup"><span data-stu-id="27f0f-127">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="27f0f-128">Например, добавьте пустой лист и скопируйте в него устаревшие данные.</span><span class="sxs-lookup"><span data-stu-id="27f0f-128">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="27f0f-129">Затем создайте формулу Excel для сопоставления данных в листе преобразования между полями в экспортированном листе и устаревшими данными клиента.</span><span class="sxs-lookup"><span data-stu-id="27f0f-129">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="27f0f-130">После сопоставления всех данных скопируйте диапазон данных в табличный журнал.</span><span class="sxs-lookup"><span data-stu-id="27f0f-130">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="27f0f-131">Не изменяйте столбцы в журналах.</span><span class="sxs-lookup"><span data-stu-id="27f0f-131">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="27f0f-132">Если они перемещаются, изменяются или удаляются, то импортировать лист в [!INCLUDE[d365fin](includes/d365fin_md.md)] невозможно.</span><span class="sxs-lookup"><span data-stu-id="27f0f-132">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="27f0f-133">Таблицы в пакете конфигурации по умолчанию</span><span class="sxs-lookup"><span data-stu-id="27f0f-133">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="27f0f-134">Пакет конфигурации по умолчанию поддерживает следующие таблицы:</span><span class="sxs-lookup"><span data-stu-id="27f0f-134">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="27f0f-135">Условия оплаты</span><span class="sxs-lookup"><span data-stu-id="27f0f-135">Payment Terms</span></span>
-   <span data-ttu-id="27f0f-136">Ценовая группа клиента</span><span class="sxs-lookup"><span data-stu-id="27f0f-136">Customer Price Group</span></span>
-   <span data-ttu-id="27f0f-137">Метод поставки</span><span class="sxs-lookup"><span data-stu-id="27f0f-137">Shipment Method</span></span>
-   <span data-ttu-id="27f0f-138">Менеджер по продажам/закупкам</span><span class="sxs-lookup"><span data-stu-id="27f0f-138">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="27f0f-139">Склады</span><span class="sxs-lookup"><span data-stu-id="27f0f-139">Location</span></span>
-   <span data-ttu-id="27f0f-140">Счет ГК</span><span class="sxs-lookup"><span data-stu-id="27f0f-140">GL Account</span></span>
-   <span data-ttu-id="27f0f-141">Клиент</span><span class="sxs-lookup"><span data-stu-id="27f0f-141">Customer</span></span>
-   <span data-ttu-id="27f0f-142">Поставщик</span><span class="sxs-lookup"><span data-stu-id="27f0f-142">Vendor</span></span>
-   <span data-ttu-id="27f0f-143">Пункт меню</span><span class="sxs-lookup"><span data-stu-id="27f0f-143">Item</span></span>
-   <span data-ttu-id="27f0f-144">Заголовок продажи</span><span class="sxs-lookup"><span data-stu-id="27f0f-144">Sales Header</span></span>
-   <span data-ttu-id="27f0f-145">Строка продажи</span><span class="sxs-lookup"><span data-stu-id="27f0f-145">Sales Line</span></span>
-   <span data-ttu-id="27f0f-146">Заголовок покупки</span><span class="sxs-lookup"><span data-stu-id="27f0f-146">Purchase Header</span></span>
-   <span data-ttu-id="27f0f-147">Строка покупки</span><span class="sxs-lookup"><span data-stu-id="27f0f-147">Purchase Line</span></span>
-   <span data-ttu-id="27f0f-148">Строка финансового журнала</span><span class="sxs-lookup"><span data-stu-id="27f0f-148">Gen. Journal Line</span></span>
-   <span data-ttu-id="27f0f-149">Строка журнала товаров</span><span class="sxs-lookup"><span data-stu-id="27f0f-149">Item Journal Line</span></span>
-   <span data-ttu-id="27f0f-150">Учетная группа клиента</span><span class="sxs-lookup"><span data-stu-id="27f0f-150">Customer Posting Group</span></span>
-   <span data-ttu-id="27f0f-151">Учетная группа поставщика</span><span class="sxs-lookup"><span data-stu-id="27f0f-151">Vendor Posting Group</span></span>
-   <span data-ttu-id="27f0f-152">Учетная группа товаров</span><span class="sxs-lookup"><span data-stu-id="27f0f-152">Inventory Posting Group</span></span>
-   <span data-ttu-id="27f0f-153">Единица измерения</span><span class="sxs-lookup"><span data-stu-id="27f0f-153">Unit of Measure</span></span>
-   <span data-ttu-id="27f0f-154">Общая бизнес-группа</span><span class="sxs-lookup"><span data-stu-id="27f0f-154">Gen. Business Posting Group</span></span>
-   <span data-ttu-id="27f0f-155">Общая товарная группа</span><span class="sxs-lookup"><span data-stu-id="27f0f-155">Gen. Product Posting Group</span></span>
-   <span data-ttu-id="27f0f-156">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="27f0f-156">General Posting Setup</span></span>
-   <span data-ttu-id="27f0f-157">Территория</span><span class="sxs-lookup"><span data-stu-id="27f0f-157">Territory</span></span>
-   <span data-ttu-id="27f0f-158">Категория товара</span><span class="sxs-lookup"><span data-stu-id="27f0f-158">Item Category</span></span>
-   <span data-ttu-id="27f0f-159">Цена продажи</span><span class="sxs-lookup"><span data-stu-id="27f0f-159">Sales Price</span></span>
-   <span data-ttu-id="27f0f-160">Цена покупки</span><span class="sxs-lookup"><span data-stu-id="27f0f-160">Purchase Price</span></span>

## <a name="see-also"></a><span data-ttu-id="27f0f-161">См. также</span><span class="sxs-lookup"><span data-stu-id="27f0f-161">See Also</span></span>
[<span data-ttu-id="27f0f-162">Настройка компании с помощью служб RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="27f0f-162">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="27f0f-163">Миграция данных QuickBooks</span><span class="sxs-lookup"><span data-stu-id="27f0f-163">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="27f0f-164">Миграция данных Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="27f0f-164">Dynamics GP Data Migration</span></span>](ui-extensions-dynamicsgp-data-migration.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 

