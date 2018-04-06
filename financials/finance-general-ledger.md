---
title: "Подробнее о главной книге и плане счетов | Документы Майкрософт"
description: "Описывает главную книгу, план счетов и категории счетов."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 63d414f4c81a9e20b4bb81b632edd9c91fb34a87
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="understanding-the-general-ledger-and-the-coa"></a><span data-ttu-id="8dd96-103">Сведения о главной книге и плане счетов</span><span class="sxs-lookup"><span data-stu-id="8dd96-103">Understanding the General Ledger and the COA</span></span>
<span data-ttu-id="8dd96-104">В главной книге хранятся финансовые данные, а в план счетов показывает счета, на которых учитываются все операции главной книги.</span><span class="sxs-lookup"><span data-stu-id="8dd96-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="8dd96-105"> включает стандартный план счетов, готовый к использованию в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="8dd96-105"> includes a standard chart of accounts that is ready to support your business.</span></span>

## <a name="general-ledger-setup-and-general-posting-setup"></a><span data-ttu-id="8dd96-106">Настройка главной книги и общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="8dd96-106">General Ledger Setup and General Posting Setup</span></span>
<span data-ttu-id="8dd96-107">Настройка главной книги — основа финансовых процессов, поскольку она определяет способ учета данных.</span><span class="sxs-lookup"><span data-stu-id="8dd96-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span></span>  

<span data-ttu-id="8dd96-108">В окне **Настройка ГК** вы указываете, как требуется обрабатывать определенные ситуации учета в вашей организации, например:</span><span class="sxs-lookup"><span data-stu-id="8dd96-108">In the **General Ledger Setup** window, you specify how to handle certain accounting issues in your company, such as:</span></span>  

* <span data-ttu-id="8dd96-109">Сведения об округлении счета</span><span class="sxs-lookup"><span data-stu-id="8dd96-109">Invoice rounding details</span></span>  
* <span data-ttu-id="8dd96-110">Форматы адреса</span><span class="sxs-lookup"><span data-stu-id="8dd96-110">Address formats</span></span>  
* <span data-ttu-id="8dd96-111">Финансовая отчетность</span><span class="sxs-lookup"><span data-stu-id="8dd96-111">Financial reporting</span></span>  

<span data-ttu-id="8dd96-112">Аналогично в окне **Общая настройка учета** вы указываете, ка нужно настроить комбинации общих бизнес-групп и общих товарных групп.</span><span class="sxs-lookup"><span data-stu-id="8dd96-112">Similarly, in the **General Posting Setup** window, you specify how you want to set up combinations of general business and general product posting groups.</span></span> <span data-ttu-id="8dd96-113">Учетные группы сопоставляют объекты, такие как клиенты, поставщики, товары, ресурсы и документов продажи и покупки со счетами главной книги.</span><span class="sxs-lookup"><span data-stu-id="8dd96-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span></span> <span data-ttu-id="8dd96-114">Следует заполнять строку по каждой комбинации бизнес-группы и товарной группы.</span><span class="sxs-lookup"><span data-stu-id="8dd96-114">You fill in a line for each combination of business posting group and product posting group.</span></span> <span data-ttu-id="8dd96-115">Дополнительные сведения см. в разделе [Настройка учетных групп](finance-posting-groups.md)</span><span class="sxs-lookup"><span data-stu-id="8dd96-115">For more information, see [Posting Group Setups](finance-posting-groups.md)</span></span>  

## <a name="the-chart-of-accounts"></a><span data-ttu-id="8dd96-116">План счетов</span><span class="sxs-lookup"><span data-stu-id="8dd96-116">The Chart of Accounts</span></span>
<span data-ttu-id="8dd96-117">В плане счетов отображаются все счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="8dd96-117">The chart of accounts shows all general ledger accounts.</span></span> <span data-ttu-id="8dd96-118">В плане счетов можно выполнять следующие действия:</span><span class="sxs-lookup"><span data-stu-id="8dd96-118">From the chart of accounts, you can do things like:</span></span>  

* <span data-ttu-id="8dd96-119">Просмотреть отчеты, в которых отображаются операции главной книги и сальдо.</span><span class="sxs-lookup"><span data-stu-id="8dd96-119">View reports that show general ledger entries and balances.</span></span>  
* <span data-ttu-id="8dd96-120">Закрыть отчет о прибылях и убытках.</span><span class="sxs-lookup"><span data-stu-id="8dd96-120">Close your income statement.</span></span>  
* <span data-ttu-id="8dd96-121">Открыть карточку счета ГК для добавления или изменения настроек.</span><span class="sxs-lookup"><span data-stu-id="8dd96-121">Open the G/L account card to add or change settings.</span></span>  
* <span data-ttu-id="8dd96-122">Просмотрите список учетных групп по этому счету.</span><span class="sxs-lookup"><span data-stu-id="8dd96-122">See a list of posting groups that post to that account.</span></span>
* <span data-ttu-id="8dd96-123">Просмотр отдельных дебетового сальдо и кредитового сальдо для одного счета</span><span class="sxs-lookup"><span data-stu-id="8dd96-123">View separate debit and credit balances for a single account</span></span>  

<span data-ttu-id="8dd96-124">Можно добавить, изменить или удалить счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="8dd96-124">You can add, change, or delete general ledger accounts.</span></span> <span data-ttu-id="8dd96-125">Однако для предотвращения расхождений невозможно удалить счет главной книги, если его данные используются в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="8dd96-125">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span></span>  

## <a name="account-categories"></a><span data-ttu-id="8dd96-126">Категории счетов</span><span class="sxs-lookup"><span data-stu-id="8dd96-126">Account Categories</span></span>
<span data-ttu-id="8dd96-127">Можно настроить структуру финансовых отчетов, сопоставив счета главной книги с категориями счетов.</span><span class="sxs-lookup"><span data-stu-id="8dd96-127">You can personalize the structure of your financial statements by mapping general ledger accounts to account categories.</span></span>  

<span data-ttu-id="8dd96-128">В окне **Категории счетов ГК** отображаются категории и подкатегории, а также счета ГК, назначенные им.</span><span class="sxs-lookup"><span data-stu-id="8dd96-128">The **G/L Account Categories** window shows your categories and subcategories, and the G/L accounts that are assigned to them.</span></span> <span data-ttu-id="8dd96-129">Вы можете создать новые подкатегории и назначить их существующим счетам.</span><span class="sxs-lookup"><span data-stu-id="8dd96-129">You can create new subcategories and assign those categories to existing accounts.</span></span>  

<span data-ttu-id="8dd96-130">Группы категорий создаются с помощью отступа подкатегорий под строкой в окне **Категории счетов ГК**.</span><span class="sxs-lookup"><span data-stu-id="8dd96-130">You create a category group by indenting other subcategories under a line in the **G/L Account Categories** window.</span></span> <span data-ttu-id="8dd96-131">Это облегчает обзор данных, так как для каждой группы показывается общее сальдо.</span><span class="sxs-lookup"><span data-stu-id="8dd96-131">This makes it easy for you to get an overview, because each grouping shows a total balance.</span></span> <span data-ttu-id="8dd96-132">Например, можно создать подкатегории для различных типов основных средств, а затем создать группы категорий для основных средств и текущих активов.</span><span class="sxs-lookup"><span data-stu-id="8dd96-132">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span></span>  

<span data-ttu-id="8dd96-133">Можно указать, должны ли счета в каждой подкатегории включаться в определенные типы отчетов.</span><span class="sxs-lookup"><span data-stu-id="8dd96-133">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span></span> <span data-ttu-id="8dd96-134">Категории счетов помогают определить макеты финансовых отчетов.</span><span class="sxs-lookup"><span data-stu-id="8dd96-134">The account categories help define the layout of your financial statements.</span></span>  

<span data-ttu-id="8dd96-135">Например, балансовый отчет по умолчанию содержит подкатегорию "Касса" категории "Текущие активы".</span><span class="sxs-lookup"><span data-stu-id="8dd96-135">For example, the default balance statement has a subcategory for Cash under Current Assets.</span></span> <span data-ttu-id="8dd96-136">Если требуется, чтобы в балансовом отчете учитывались мелкие доходы и чеки, можно:</span><span class="sxs-lookup"><span data-stu-id="8dd96-136">If you want the balance statement consider petty cash and checking, you can:</span></span>  

1. <span data-ttu-id="8dd96-137">Добавить две новые подкатегории.</span><span class="sxs-lookup"><span data-stu-id="8dd96-137">Add two new subcategories.</span></span> <span data-ttu-id="8dd96-138">Одну — для кассы, вторую — для чеков.</span><span class="sxs-lookup"><span data-stu-id="8dd96-138">One for petty cash, and one for your checking account.</span></span>  
2. <span data-ttu-id="8dd96-139">Определить дополнительное описание отчета **Кассы** для этих подкатегорий.</span><span class="sxs-lookup"><span data-stu-id="8dd96-139">Specify the additional report definition **Cash Accounts** for these subcategories.</span></span>  
3. <span data-ttu-id="8dd96-140">Поместить их в подкатегорию **Касса**.</span><span class="sxs-lookup"><span data-stu-id="8dd96-140">Indent them under the **Cash** subcategory.</span></span>  

<span data-ttu-id="8dd96-141">При следующем создании финансовых отчетов балансовый отчет будет содержать общее сальдо для кассы и две строки для сальдо по мелким доходам и чекам.</span><span class="sxs-lookup"><span data-stu-id="8dd96-141">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the checking account.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8dd96-142">См. также</span><span class="sxs-lookup"><span data-stu-id="8dd96-142">See Also</span></span>
[<span data-ttu-id="8dd96-143">Финансы</span><span class="sxs-lookup"><span data-stu-id="8dd96-143">Finance</span></span>](finance.md)  
[<span data-ttu-id="8dd96-144">Настройка или изменение плана счетов</span><span class="sxs-lookup"><span data-stu-id="8dd96-144">Setting Up or Changing the Chart of Accounts</span></span>](finance-setup-chart-accounts.md)  
[<span data-ttu-id="8dd96-145">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="8dd96-145">Business Intelligence</span></span>](bi.md)  

