---
title: Подробнее о главной книге и плане счетов | Документация Майкрософт
description: Описывает главную книгу, план счетов и категории счетов.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 29658ea0c7689ebdcb84384dfb26ec26089685c3
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5376816"
---
# <a name="understanding-the-general-ledger-and-the-coa"></a><span data-ttu-id="cb322-103">Сведения о главной книге и плане счетов</span><span class="sxs-lookup"><span data-stu-id="cb322-103">Understanding the General Ledger and the COA</span></span>

<span data-ttu-id="cb322-104">В главной книге хранятся финансовые данные, а в план счетов показывает счета, на которых учитываются все операции главной книги.</span><span class="sxs-lookup"><span data-stu-id="cb322-104">The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="cb322-105">включает стандартный план счетов, готовый к использованию в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="cb322-105">includes a standard chart of accounts that is ready to support your business.</span></span>

## <a name="general-ledger-setup-and-general-posting-setup"></a><span data-ttu-id="cb322-106">Настройка главной книги и общая настройка учета</span><span class="sxs-lookup"><span data-stu-id="cb322-106">General Ledger Setup and General Posting Setup</span></span>

<span data-ttu-id="cb322-107">Настройка главной книги — основа финансовых процессов, поскольку она определяет способ учета данных.</span><span class="sxs-lookup"><span data-stu-id="cb322-107">The setup of the general ledger is at the core of financial processes because it defines how you post data.</span></span>  

<span data-ttu-id="cb322-108">На странице **Настройка ГК** вы указываете, как требуется обрабатывать определенные ситуации учета в вашей организации, например:</span><span class="sxs-lookup"><span data-stu-id="cb322-108">On the **General Ledger Setup** page, you specify how to handle certain accounting issues in your company, such as:</span></span>  

* <span data-ttu-id="cb322-109">Сведения об округлении счета</span><span class="sxs-lookup"><span data-stu-id="cb322-109">Invoice rounding details</span></span>  
* <span data-ttu-id="cb322-110">Форматы адреса</span><span class="sxs-lookup"><span data-stu-id="cb322-110">Address formats</span></span>  
* <span data-ttu-id="cb322-111">Финансовая отчетность</span><span class="sxs-lookup"><span data-stu-id="cb322-111">Financial reporting</span></span>  

<span data-ttu-id="cb322-112">Аналогично на странице **Общая настройка учета** вы указываете, ка нужно настроить комбинации общих бизнес-групп и общих товарных групп.</span><span class="sxs-lookup"><span data-stu-id="cb322-112">Similarly, on the **General Posting Setup** page, you specify how you want to set up combinations of general business and general product posting groups.</span></span> <span data-ttu-id="cb322-113">Учетные группы сопоставляют объекты, такие как клиенты, поставщики, товары, ресурсы и документов продажи и покупки со счетами главной книги.</span><span class="sxs-lookup"><span data-stu-id="cb322-113">Posting groups map entities like customers, vendors, items, resources, and sales and purchase documents to general ledger accounts.</span></span> <span data-ttu-id="cb322-114">Следует заполнять строку по каждой комбинации бизнес-группы и товарной группы.</span><span class="sxs-lookup"><span data-stu-id="cb322-114">You fill in a line for each combination of business posting group and product posting group.</span></span> <span data-ttu-id="cb322-115">Дополнительные сведения см. в разделе [Настройка учетных групп](finance-posting-groups.md).</span><span class="sxs-lookup"><span data-stu-id="cb322-115">For more information, see [Posting Group Setups](finance-posting-groups.md).</span></span>  

> [!TIP]
> <span data-ttu-id="cb322-116">На странице **Настройка ГК** содержатся общие поля и поля, относящиеся к вашей стране или региону.</span><span class="sxs-lookup"><span data-stu-id="cb322-116">The **General Ledger Setup** page includes generic fields and fields that are particular to your country or region.</span></span> <span data-ttu-id="cb322-117">Если вы не уверены в назначении какого-либо поля, советуем вам поговорить со своим бухгалтером, чтобы определить, актуально ли оно для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="cb322-117">If you are not sure of the meaning of a field, we suggest you work with your accountant to determine whether it is of relevance to your organization.</span></span>  

## <a name="the-chart-of-accounts"></a><span data-ttu-id="cb322-118">План счетов</span><span class="sxs-lookup"><span data-stu-id="cb322-118">The Chart of Accounts</span></span>

<span data-ttu-id="cb322-119">В плане счетов отображаются все счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="cb322-119">The chart of accounts shows all general ledger accounts.</span></span> <span data-ttu-id="cb322-120">В плане счетов можно выполнять следующие действия:</span><span class="sxs-lookup"><span data-stu-id="cb322-120">From the chart of accounts, you can do things like:</span></span>  

* <span data-ttu-id="cb322-121">Просмотреть отчеты, в которых отображаются операции главной книги и сальдо.</span><span class="sxs-lookup"><span data-stu-id="cb322-121">View reports that show general ledger entries and balances.</span></span>  
* <span data-ttu-id="cb322-122">Закрыть отчет о прибылях и убытках.</span><span class="sxs-lookup"><span data-stu-id="cb322-122">Close your income statement.</span></span>  
* <span data-ttu-id="cb322-123">Открыть карточку счета ГК для добавления или изменения настроек.</span><span class="sxs-lookup"><span data-stu-id="cb322-123">Open the G/L account card to add or change settings.</span></span>  
* <span data-ttu-id="cb322-124">Просмотрите список учетных групп по этому счету.</span><span class="sxs-lookup"><span data-stu-id="cb322-124">See a list of posting groups that post to that account.</span></span>
* <span data-ttu-id="cb322-125">Просмотр отдельных дебетового сальдо и кредитового сальдо для одного счета</span><span class="sxs-lookup"><span data-stu-id="cb322-125">View separate debit and credit balances for a single account</span></span>  

<span data-ttu-id="cb322-126">Можно добавить, изменить или удалить счета главной книги.</span><span class="sxs-lookup"><span data-stu-id="cb322-126">You can add, change, or delete general ledger accounts.</span></span> <span data-ttu-id="cb322-127">Однако для предотвращения расхождений невозможно удалить счет главной книги, если его данные используются в плане счетов.</span><span class="sxs-lookup"><span data-stu-id="cb322-127">However, to prevent discrepancies, you can't delete a general ledger account if it's data is used in the chart of accounts.</span></span>  

## <a name="account-categories"></a><span data-ttu-id="cb322-128">Категории счетов</span><span class="sxs-lookup"><span data-stu-id="cb322-128">Account Categories</span></span>

<span data-ttu-id="cb322-129">Можно настроить структуру финансовых отчетов, сопоставив счета главной книги с категориями счетов.</span><span class="sxs-lookup"><span data-stu-id="cb322-129">You can personalize the structure of your financial statements by mapping general ledger accounts to account categories.</span></span>  

<span data-ttu-id="cb322-130">На странице **Категории счетов ГК** отображаются категории и подкатегории, а также счета ГК, назначенные им.</span><span class="sxs-lookup"><span data-stu-id="cb322-130">The **G/L Account Categories** page shows your categories and subcategories, and the G/L accounts that are assigned to them.</span></span> <span data-ttu-id="cb322-131">Вы можете создать новые подкатегории и назначить их существующим счетам.</span><span class="sxs-lookup"><span data-stu-id="cb322-131">You can create new subcategories and assign those categories to existing accounts.</span></span>  

<span data-ttu-id="cb322-132">Группы категорий создаются с помощью отступа подкатегорий под строкой на странице **Категории счетов ГК**.</span><span class="sxs-lookup"><span data-stu-id="cb322-132">You create a category group by indenting other subcategories under a line on the **G/L Account Categories** page.</span></span> <span data-ttu-id="cb322-133">Это облегчает обзор данных, так как для каждой группы показывается общее сальдо.</span><span class="sxs-lookup"><span data-stu-id="cb322-133">This makes it easy for you to get an overview, because each grouping shows a total balance.</span></span> <span data-ttu-id="cb322-134">Например, можно создать подкатегории для различных типов основных средств, а затем создать группы категорий для основных средств и текущих активов.</span><span class="sxs-lookup"><span data-stu-id="cb322-134">For example, you can create subcategories for different types of assets, and then create category groups for fixed assets versus current assets.</span></span>  

<span data-ttu-id="cb322-135">Можно указать, должны ли счета в каждой подкатегории включаться в определенные типы отчетов.</span><span class="sxs-lookup"><span data-stu-id="cb322-135">You can specify whether the accounts in each subcategory must be included in specific types of reports.</span></span> <span data-ttu-id="cb322-136">Категории счетов помогают определить макеты финансовых отчетов.</span><span class="sxs-lookup"><span data-stu-id="cb322-136">The account categories help define the layout of your financial statements.</span></span>  

<span data-ttu-id="cb322-137">Например, балансовый отчет по умолчанию содержит подкатегорию "Касса" категории "Текущие активы".</span><span class="sxs-lookup"><span data-stu-id="cb322-137">For example, the default balance statement has a subcategory for Cash under Current Assets.</span></span> <span data-ttu-id="cb322-138">Если требуется, чтобы в балансовом отчете учитывались мелкие доходы и чеки, можно:</span><span class="sxs-lookup"><span data-stu-id="cb322-138">If you want the balance statement consider petty cash and checking, you can:</span></span>  

1. <span data-ttu-id="cb322-139">Добавить две новые подкатегории.</span><span class="sxs-lookup"><span data-stu-id="cb322-139">Add two new subcategories.</span></span> <span data-ttu-id="cb322-140">Одну — для кассы, вторую — для чеков.</span><span class="sxs-lookup"><span data-stu-id="cb322-140">One for petty cash, and one for your checking account.</span></span>  
2. <span data-ttu-id="cb322-141">Определить дополнительное описание отчета **Кассы** для этих подкатегорий.</span><span class="sxs-lookup"><span data-stu-id="cb322-141">Specify the additional report definition **Cash Accounts** for these subcategories.</span></span>  
3. <span data-ttu-id="cb322-142">Поместить их в подкатегорию **Касса**.</span><span class="sxs-lookup"><span data-stu-id="cb322-142">Indent them under the **Cash** subcategory.</span></span>  

<span data-ttu-id="cb322-143">При следующем создании финансовых отчетов балансовый отчет будет содержать общее сальдо для кассы и две строки для сальдо по мелким доходам и чекам.</span><span class="sxs-lookup"><span data-stu-id="cb322-143">The next time you generate account schedules your balance statement will show a total balance for cash and two lines with balances for petty cash and the checking account.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cb322-144">См. также</span><span class="sxs-lookup"><span data-stu-id="cb322-144">See Also</span></span>

[<span data-ttu-id="cb322-145">Финансы</span><span class="sxs-lookup"><span data-stu-id="cb322-145">Finance</span></span>](finance.md)  
[<span data-ttu-id="cb322-146">Настройка или изменение плана счетов</span><span class="sxs-lookup"><span data-stu-id="cb322-146">Setting Up or Changing the Chart of Accounts</span></span>](finance-setup-chart-accounts.md)  
[<span data-ttu-id="cb322-147">Бизнес-аналитика</span><span class="sxs-lookup"><span data-stu-id="cb322-147">Business Intelligence</span></span>](bi.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]