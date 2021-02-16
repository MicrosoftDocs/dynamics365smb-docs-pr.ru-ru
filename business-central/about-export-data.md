---
title: Экспорт данных из Business Central в Excel | Документация Майкрософт
description: Вы можете экспортировать финансовые отчеты и данные бизнес-аналитики из Business Central в Excel или открыть данные в Excel.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, reporting, financial report, business intelligence, BI, Excel
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0058fd8aa684fd12392e641dda3bbb0ee6862134
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753696"
---
# <a name="exporting-your-business-data-to-excel"></a><span data-ttu-id="2420e-103">Экспорт бизнес-данных в Excel</span><span class="sxs-lookup"><span data-stu-id="2420e-103">Exporting Your Business Data to Excel</span></span>
<span data-ttu-id="2420e-104">Если вы хотите работать с данными из [!INCLUDE[prod_short](includes/prod_short.md)] в Excel, вы можете открыть все списки в Excel и работать с ними там.</span><span class="sxs-lookup"><span data-stu-id="2420e-104">If you want to work with your data from [!INCLUDE[prod_short](includes/prod_short.md)] in Excel, you can open all lists in Excel and work with it there.</span></span> <span data-ttu-id="2420e-105">Аналогично, если требуется отменить подписку на [!INCLUDE[prod_short](includes/prod_short.md)], вы можете экспортировать данные в Excel, чтобы забрать их с собой.</span><span class="sxs-lookup"><span data-stu-id="2420e-105">Similarly, if you want to cancel your subscription for [!INCLUDE[prod_short](includes/prod_short.md)], you can export your data to Excel so that you can take it with you.</span></span>

## <a name="opening-lists-in-excel"></a><span data-ttu-id="2420e-106">Открытие списков в Excel</span><span class="sxs-lookup"><span data-stu-id="2420e-106">Opening Lists in Excel</span></span>
<span data-ttu-id="2420e-107">Можно открыть данные в Excel из любого журнала, списка или листа.</span><span class="sxs-lookup"><span data-stu-id="2420e-107">You can open data in Excel from any journal, list, or worksheet.</span></span> <span data-ttu-id="2420e-108">Для откройте требуемую станицу и выберите **Открыть в Excel**.</span><span class="sxs-lookup"><span data-stu-id="2420e-108">You just open the page that you want, and then choose **Open in Excel**.</span></span> <span data-ttu-id="2420e-109">Например, откройте список клиентов (поиск по слову **Клиенты**) и выберите **Открыть в Excel**.</span><span class="sxs-lookup"><span data-stu-id="2420e-109">For example, open the list of customers (search for **Customers**), and then choose **Open in Excel**.</span></span> <span data-ttu-id="2420e-110">Ваш браузер выдаст запрос на открытие или сохранение созданной книги Excel.</span><span class="sxs-lookup"><span data-stu-id="2420e-110">Your browser will prompt you to open or save the generated Excel workbook.</span></span>  

> [!NOTE]
> <span data-ttu-id="2420e-111">Этот вариант используется, когда не требуется вносить изменения и опубликовывать эти изменения обратно в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="2420e-111">Use this option when you do not want to make changes and publish those changes back to [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

<span data-ttu-id="2420e-112">Каждый список включает число столбцов, а экспорт в Excel будет включать все столбцы, имеющиеся в текущем представлении.</span><span class="sxs-lookup"><span data-stu-id="2420e-112">Each list includes a number of columns, and the export to Excel will include any columns that are in your current view.</span></span> <span data-ttu-id="2420e-113">Если вы хотите добавить или удалить столбцы перед открытием списка в Excel, достаточно открыть контекстное меню для любого столбца, а затем указать, какие столбцы требуется отображать.</span><span class="sxs-lookup"><span data-stu-id="2420e-113">If you want to add or remove columns before you open the list in Excel, you simply open the shortcut menu for any column and then specify which columns that you want to see.</span></span> <span data-ttu-id="2420e-114">Этот список столбцов отличается для большинства списков и отражает структуру в базе данных, в которой хранятся данные.</span><span class="sxs-lookup"><span data-stu-id="2420e-114">This list of columns is different for most lists, and it reflects the structure in the database where your data is stored.</span></span> <span data-ttu-id="2420e-115">Если вы не уверены, какой тип данных содержится в определенном столбце, вы можете добавить его в представление, а затем решить, требуется ли его снова удалить.</span><span class="sxs-lookup"><span data-stu-id="2420e-115">If you are not sure what type of data a certain column contains, you can add it to your view and then decide if you want to remove it again.</span></span>  

### <a name="edit-data-in-excel"></a><span data-ttu-id="2420e-116">Изменить данные в Excel</span><span class="sxs-lookup"><span data-stu-id="2420e-116">Edit Data in Excel</span></span>
<span data-ttu-id="2420e-117">Если [!INCLUDE[prod_short](includes/prod_short.md)] включает надстройку для Excel, можно изменять данные в Excel.</span><span class="sxs-lookup"><span data-stu-id="2420e-117">Your [!INCLUDE[prod_short](includes/prod_short.md)] experience includes an add-in for Excel so you can edit data in Excel.</span></span> <span data-ttu-id="2420e-118">Дополнительные сведения см. в разделе [Анализ финансовых выписок в Microsoft Excel](finance-analyze-excel.md).</span><span class="sxs-lookup"><span data-stu-id="2420e-118">For more information, see [Analyzing Financial Statements in Microsoft Excel](finance-analyze-excel.md).</span></span>  

## <a name="exporting-data-to-other-finance-systems"></a><span data-ttu-id="2420e-119">Экспорт данных в другие финансовые системы</span><span class="sxs-lookup"><span data-stu-id="2420e-119">Exporting Data to Other Finance Systems</span></span>
<span data-ttu-id="2420e-120">Если требуется отменить подписку на [!INCLUDE[prod_short](includes/prod_short.md)], вы можете экспортировать данные в Excel и перенести их в следующую финансовую систему.</span><span class="sxs-lookup"><span data-stu-id="2420e-120">If you decide to cancel your subscription for [!INCLUDE[prod_short](includes/prod_short.md)], you can export your data to Excel and take it with you to your next finance system.</span></span>  

<span data-ttu-id="2420e-121">Конечно же, можно экспортировать все страницы, но, возможно, вам не потребуются все они.</span><span class="sxs-lookup"><span data-stu-id="2420e-121">You can export all pages, of course, but that might be more than you really need.</span></span> <span data-ttu-id="2420e-122">Таким образом, рассмотрите возможность экспортировать следующие важные страницы и не забудьте добавить столбцы, как описано ранее:</span><span class="sxs-lookup"><span data-stu-id="2420e-122">So consider exporting the following essential pages, and remember to add all columns as described earlier:</span></span>  

* <span data-ttu-id="2420e-123">План счетов</span><span class="sxs-lookup"><span data-stu-id="2420e-123">Chart of Accounts</span></span>  
* <span data-ttu-id="2420e-124">Клиенты</span><span class="sxs-lookup"><span data-stu-id="2420e-124">Customers</span></span>  
* <span data-ttu-id="2420e-125">Поставщики</span><span class="sxs-lookup"><span data-stu-id="2420e-125">Vendors</span></span>  
* <span data-ttu-id="2420e-126">Банки</span><span class="sxs-lookup"><span data-stu-id="2420e-126">Banks</span></span>  
* <span data-ttu-id="2420e-127">Товары</span><span class="sxs-lookup"><span data-stu-id="2420e-127">Items</span></span>  

<span data-ttu-id="2420e-128">Если вам также требуются все финансовые транзакции, это большой объем данных, поэтому часто экспорт займет больше, чем несколько минут.</span><span class="sxs-lookup"><span data-stu-id="2420e-128">If you want all your financial transactions as well, this is a large amount of data, so the export will often take more than a few minutes of time.</span></span> <span data-ttu-id="2420e-129">Финансовые транзакции будут показаны на странице **Операции главной книги**.</span><span class="sxs-lookup"><span data-stu-id="2420e-129">The financial transactions are shown on the **General Ledger Entries** page.</span></span>  

<span data-ttu-id="2420e-130">Рекомендуется также рассмотреть возможность экспорта данных со следующих страниц:</span><span class="sxs-lookup"><span data-stu-id="2420e-130">We recommend that you also consider exporting data from the following pages:</span></span>  

* <span data-ttu-id="2420e-131">Книга операций по клиентам</span><span class="sxs-lookup"><span data-stu-id="2420e-131">Customer Ledger Entries</span></span>  
* <span data-ttu-id="2420e-132">Книга операций по поставщикам</span><span class="sxs-lookup"><span data-stu-id="2420e-132">Vendor Ledger Entries</span></span>  
* <span data-ttu-id="2420e-133">Книга операций по банку/кассе</span><span class="sxs-lookup"><span data-stu-id="2420e-133">Bank Account Ledger Entries</span></span>  
* <span data-ttu-id="2420e-134">Книга операций по товарам</span><span class="sxs-lookup"><span data-stu-id="2420e-134">Item Ledger Entries</span></span>  
* <span data-ttu-id="2420e-135">Общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="2420e-135">General Posting Setup</span></span>  
* <span data-ttu-id="2420e-136">Учетные группы клиента</span><span class="sxs-lookup"><span data-stu-id="2420e-136">Customer Posting Groups</span></span>  
* <span data-ttu-id="2420e-137">Учетные группы поставщика</span><span class="sxs-lookup"><span data-stu-id="2420e-137">Vendor Posting Groups</span></span>  
* <span data-ttu-id="2420e-138">Товарные учетные группы</span><span class="sxs-lookup"><span data-stu-id="2420e-138">Item Posting Groups</span></span>  
* <span data-ttu-id="2420e-139">Учетная группа банка</span><span class="sxs-lookup"><span data-stu-id="2420e-139">Bank Posting Group</span></span>  
* <span data-ttu-id="2420e-140">Бюджеты ГК</span><span class="sxs-lookup"><span data-stu-id="2420e-140">G/L Budgets</span></span>  
* <span data-ttu-id="2420e-141">Операции бюджета ГК</span><span class="sxs-lookup"><span data-stu-id="2420e-141">G/L Budget Entries</span></span>  
* <span data-ttu-id="2420e-142">Предложения по продаже</span><span class="sxs-lookup"><span data-stu-id="2420e-142">Sales Quotes</span></span>  
* <span data-ttu-id="2420e-143">Счета продажи</span><span class="sxs-lookup"><span data-stu-id="2420e-143">Sales Invoices</span></span>  
* <span data-ttu-id="2420e-144">Счета покупки</span><span class="sxs-lookup"><span data-stu-id="2420e-144">Purchase Invoices</span></span>  
* <span data-ttu-id="2420e-145">Контакты</span><span class="sxs-lookup"><span data-stu-id="2420e-145">Contacts</span></span>  
* <span data-ttu-id="2420e-146">Менеджеры</span><span class="sxs-lookup"><span data-stu-id="2420e-146">Salespeople</span></span>  

> [!NOTE]  
> <span data-ttu-id="2420e-147">Если настроено несколько организаций в [!INCLUDE[prod_short](includes/prod_short.md)], необходимо экспортировать соответствующие данные из каждой организации.</span><span class="sxs-lookup"><span data-stu-id="2420e-147">If you have set up more than one company in [!INCLUDE[prod_short](includes/prod_short.md)], you must export the relevant data from each company.</span></span>

> [!NOTE]
> <span data-ttu-id="2420e-148">Для открытия или редактирования данных в Excel у вас должно быть хотя бы одно из следующих разрешений:</span><span class="sxs-lookup"><span data-stu-id="2420e-148">You must have at least one of the following permissions to open or edit data in Excel:</span></span>
>    - <span data-ttu-id="2420e-149">Набор разрешений *Действие экспорта в D365 Excel*</span><span class="sxs-lookup"><span data-stu-id="2420e-149">Permission set *D365 Excel Export Action*</span></span>  
>    - <span data-ttu-id="2420e-150">Системное разрешение 6110 *Разрешить экспорт действий в Excel*.</span><span class="sxs-lookup"><span data-stu-id="2420e-150">System permission 6110 *Allow Action Export To Excel*.</span></span>  

<span data-ttu-id="2420e-151">Дополнительные сведения см. в разделе [Получение обзора разрешений пользователя](ui-define-granular-permissions.md#to-get-an-overview-of-a-users-permissions).</span><span class="sxs-lookup"><span data-stu-id="2420e-151">For more information, see [To get an overview of a user's permissions](ui-define-granular-permissions.md#to-get-an-overview-of-a-users-permissions).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="2420e-152">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="2420e-152">See Related Training at [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="2420e-153">См. также</span><span class="sxs-lookup"><span data-stu-id="2420e-153">See Also</span></span>
<span data-ttu-id="2420e-154">[Отмена подписки [!INCLUDE[prod_short](includes/prod_short.md)]](admin-cancel.md)</span><span class="sxs-lookup"><span data-stu-id="2420e-154">[Canceling Your Subscription for [!INCLUDE[prod_short](includes/prod_short.md)]](admin-cancel.md)</span></span>  
[<span data-ttu-id="2420e-155">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="2420e-155">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="2420e-156">Анализ финансовых отчетов в Microsoft Excel</span><span class="sxs-lookup"><span data-stu-id="2420e-156">Analyzing Financial Statements in Microsoft Excel</span></span>](finance-analyze-excel.md)  
[<span data-ttu-id="2420e-157">Финансы</span><span class="sxs-lookup"><span data-stu-id="2420e-157">Finance</span></span>](finance.md)  
[<span data-ttu-id="2420e-158">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="2420e-158">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="2420e-159">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2420e-159">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
