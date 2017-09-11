---
title: "Необязательные действия для закрытия периодов | Документы Майкрософт"
description: "В этом разделе описываются необязательные процессы и действия по закрытию учетных периодов в Financials."
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments
ms.date: 06/02/2017
ms.author: jswymer
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 678cebc065594ed0ed6fea897676f109ff2c1dce
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="overview-of-tasks-to-close-accounting-periods"></a><span data-ttu-id="eb734-103">Обзор задач по закрытию учетных периодов</span><span class="sxs-lookup"><span data-stu-id="eb734-103">Overview of Tasks to Close Accounting Periods</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="eb734-104"> не требует принудительного закрытия периодов, однако предусмотрено множество действий на конец периода (месяца), которые можно выполнить.</span><span class="sxs-lookup"><span data-stu-id="eb734-104"> does not force you to close periods, however, there are many period-end (month-end) activities that you can do.</span></span> <span data-ttu-id="eb734-105">В этом разделе представлен обзор дополнительных процессов и действий для закрытия периодов.</span><span class="sxs-lookup"><span data-stu-id="eb734-105">This topic provides an overview of optional processes and activities for closing periods.</span></span>  

## <a name="general-ledger"></a><span data-ttu-id="eb734-106">Главная книга</span><span class="sxs-lookup"><span data-stu-id="eb734-106">General Ledger</span></span>
* <span data-ttu-id="eb734-107">Укажите системные и пользовательские периоды учета.</span><span class="sxs-lookup"><span data-stu-id="eb734-107">Specify system-wide and user-specific posting periods.</span></span>  

    <span data-ttu-id="eb734-108">Они определяют даты, между которыми возможен учет.</span><span class="sxs-lookup"><span data-stu-id="eb734-108">This specifies the dates between which you allow posting.</span></span> <span data-ttu-id="eb734-109">В зависимости от бизнеса можно разрешить учет в начале процесса или ближе к концу.</span><span class="sxs-lookup"><span data-stu-id="eb734-109">Depending on your business, you may want to allow posting at the start of the period, or toward the end.</span></span> <span data-ttu-id="eb734-110">Дополнительные сведения см. в разделе [Практическое руководство. Определение периодов учета](finance-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="eb734-110">For more information, see [How to: Specify Posting Periods](finance-how-specify-posting-periods.md).</span></span>  
* <span data-ttu-id="eb734-111">Внесите все необходимые корректировки в ГК.</span><span class="sxs-lookup"><span data-stu-id="eb734-111">Make all necessary G/L adjustments.</span></span>  
* <span data-ttu-id="eb734-112">Обновите и учтите типовые журналы.</span><span class="sxs-lookup"><span data-stu-id="eb734-112">Update and post Recurring Journals.</span></span>  
  <!--* Process Consolidations-->
* <span data-ttu-id="eb734-113">Создайте финансовые отчеты следующим образом:</span><span class="sxs-lookup"><span data-stu-id="eb734-113">Run account schedules as follows:</span></span>  
  * <span data-ttu-id="eb734-114">Откройте окно **Финансовый отчет** и выберите действие **Печать**.</span><span class="sxs-lookup"><span data-stu-id="eb734-114">Open the **Account Schedule** window, and then choose the **Print** action.</span></span>  

## <a name="sales-and-receivables"></a><span data-ttu-id="eb734-115">Продажи и дебиторская задолженность</span><span class="sxs-lookup"><span data-stu-id="eb734-115">Sales and Receivables</span></span>
* <span data-ttu-id="eb734-116">Учтите все заказы на продажу, счета, кредит-ноты и заказы на возврат.</span><span class="sxs-lookup"><span data-stu-id="eb734-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="eb734-117">Выполните учет всех журналов кассовых поступлений.</span><span class="sxs-lookup"><span data-stu-id="eb734-117">Post all cash receipt journals.</span></span>  
* <span data-ttu-id="eb734-118">Выполните обновление и учет типовых журналов, относящихся к продажам и расчетам с дебиторами.</span><span class="sxs-lookup"><span data-stu-id="eb734-118">Update and post recurring journals that are related to sales and receivables.</span></span>  
* <span data-ttu-id="eb734-119">Выполните выверку дебиторской задолженности с главной книгой.</span><span class="sxs-lookup"><span data-stu-id="eb734-119">Reconcile accounts receivable to the general ledger.</span></span>  
* <span data-ttu-id="eb734-120">Выполните пакетное задание **Удаление заказов на продажу, по которым выставлены счета**.</span><span class="sxs-lookup"><span data-stu-id="eb734-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>  

## <a name="purchases-and-payables"></a><span data-ttu-id="eb734-121">Покупки и кредиторская задолженность</span><span class="sxs-lookup"><span data-stu-id="eb734-121">Purchases and Payables</span></span>
* <span data-ttu-id="eb734-122">Выполните учет всех заказов на покупку, счетов, кредит-нот и заказов на возврат.</span><span class="sxs-lookup"><span data-stu-id="eb734-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>  
* <span data-ttu-id="eb734-123">Выполните учет всех журналов оплат.</span><span class="sxs-lookup"><span data-stu-id="eb734-123">Post all payment journals.</span></span>  
* <span data-ttu-id="eb734-124">Выполните обновление и учет типовых журналов, относящихся к покупкам и расчетам с кредиторами.</span><span class="sxs-lookup"><span data-stu-id="eb734-124">Update and post recurring journals that are related to purchases & payables.</span></span>  
* <span data-ttu-id="eb734-125">Выполните отчет **Кредиторская задолженность по срокам давности** и проведите выверку кредиторской задолженности с главной книгой.</span><span class="sxs-lookup"><span data-stu-id="eb734-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>  
* <span data-ttu-id="eb734-126">Выполните пакетное задание **Удалить заказы на покупку, по которым выставлены счета**.</span><span class="sxs-lookup"><span data-stu-id="eb734-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>  

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="eb734-127">Расчет и обработка налога с продаж</span><span class="sxs-lookup"><span data-stu-id="eb734-127">Calculate and Process Sales Tax</span></span>
* <span data-ttu-id="eb734-128">Завершите отчеты по НДС.</span><span class="sxs-lookup"><span data-stu-id="eb734-128">Complete Tax Statements.</span></span>  

## <a name="see-also"></a><span data-ttu-id="eb734-129">См. также</span><span class="sxs-lookup"><span data-stu-id="eb734-129">See Also</span></span>
[<span data-ttu-id="eb734-130">Закрытие года и периодов</span><span class="sxs-lookup"><span data-stu-id="eb734-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="eb734-131">Закрытие книг</span><span class="sxs-lookup"><span data-stu-id="eb734-131">Closing Books</span></span>](year-close-books.md)  
<span data-ttu-id="eb734-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="eb734-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

