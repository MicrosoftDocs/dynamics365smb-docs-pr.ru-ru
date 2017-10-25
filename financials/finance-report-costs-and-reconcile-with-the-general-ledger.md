---
title: "Отчет о затратах и выверка с главной книгой | Документы Майкрософт"
description: "В конце учетных периодов, месяцев, лет и т. д. должна выполняться последовательность задач аудита и управления себестоимостью для создания отчетов с правильной и сбалансированной стоимостью запасов для финансового отдела. Отдельно от подпрограммы учета, которая передает операции стоимости отдельных товаров в выделенные счета главной книги, существует несколько отчетов, а также функции отслеживания и специальное средство выверки, доступные для аудиторов и контролеров, ответственных за выполнений этой чрезвычайно важной для бизнеса работы."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 3c3a02aa2251b9b6b18576e9f274d018a617b179
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="reporting-costs-and-reconciling-with-the-general-ledger"></a><span data-ttu-id="91f56-104">Отчет о затратах и выверка с главной книгой</span><span class="sxs-lookup"><span data-stu-id="91f56-104">Reporting Costs and Reconciling with the General Ledger</span></span>
<span data-ttu-id="91f56-105">В конце учетных периодов, месяцев, лет и т. д. должна выполняться последовательность задач аудита и управления себестоимостью для создания отчетов с правильной и сбалансированной стоимостью запасов для финансового отдела.</span><span class="sxs-lookup"><span data-stu-id="91f56-105">At the end of accounting periods, monthly, yearly or other, a sequence of cost control and auditing tasks must be performed to report a correct and balanced inventory value to the finance department.</span></span> <span data-ttu-id="91f56-106">Отдельно от подпрограммы учета, которая передает операции стоимости отдельных товаров в выделенные счета главной книги, существует несколько отчетов, а также функции отслеживания и специальное средство выверки, доступные для аудиторов и контролеров, ответственных за выполнений этой чрезвычайно важной для бизнеса работы.</span><span class="sxs-lookup"><span data-stu-id="91f56-106">Apart from the posting routine that transfers the individual item value entries to dedicated general ledger accounts, several reports, tracing functions, and a special reconciliation tool are available to the auditor or controller responsible for this business-critical work.</span></span>  

 <span data-ttu-id="91f56-107">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="91f56-107">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="91f56-108">**Задача**</span><span class="sxs-lookup"><span data-stu-id="91f56-108">**To**</span></span>|<span data-ttu-id="91f56-109">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="91f56-109">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="91f56-110">Просмотр стоимости запасов для выбранных товаров, включая сведения о количестве и стоимости увеличения и уменьшения запасов за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="91f56-110">View the inventory value of selected items, including information about the quantities and values of increases and decreases in inventory over a selected period.</span></span>|<span data-ttu-id="91f56-111">Отчет **Оценка стоимости товаров**</span><span class="sxs-lookup"><span data-stu-id="91f56-111">**Inventory Valuation** report</span></span>|  
|<span data-ttu-id="91f56-112">Просмотр стоимости запасов для выбранных заказов на производство в НЗП (незавершенном производстве), таких как количество и стоимость потребления, использование производственных мощностей и выход по текущим производственным заказам.</span><span class="sxs-lookup"><span data-stu-id="91f56-112">View the inventory value of selected production orders in your WIP (work in process) inventory, such as the quantities and values of consumption, capacity usage, and output in ongoing production orders.</span></span>|<span data-ttu-id="91f56-113">Отчет **Оценка стоимости запасов - НЗП**</span><span class="sxs-lookup"><span data-stu-id="91f56-113">**Inventory Valuation - WIP** report</span></span>|  
|<span data-ttu-id="91f56-114">Просмотр стоимости запасов для выбранных товаров, включая их фактическую и ожидаемую себестоимость на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="91f56-114">View the inventory value of selected items, including their actual and expected cost on the date specified.</span></span>|<span data-ttu-id="91f56-115">Отчет **Оценка запасов - специф. себест.**</span><span class="sxs-lookup"><span data-stu-id="91f56-115">**Invt. Valuation - Cost Spec.** report</span></span>|  
|<span data-ttu-id="91f56-116">Использование отчета для анализа причин отклонения себестоимости или анализа доли себестоимости для проданных товаров (себестоимости продажи).</span><span class="sxs-lookup"><span data-stu-id="91f56-116">Use a report to analyze the reasons for cost variances or to gain insight into the cost shares of sold items (COGS).</span></span>|<span data-ttu-id="91f56-117">Отчет **Анализ структуры себестоимости**</span><span class="sxs-lookup"><span data-stu-id="91f56-117">**Cost Shares Breakdown** report</span></span>|  
|<span data-ttu-id="91f56-118">Периодический учет операций стоимости транзакций товаров из книги инвентаризации в связанных счетах ГК для выверки двух книг.</span><span class="sxs-lookup"><span data-stu-id="91f56-118">Periodically post the value entries of item transactions from the inventory ledger to the related G/L accounts to reconcile the two ledgers.</span></span>|[<span data-ttu-id="91f56-119">Практическое руководство. Выверка себестоимости товаров с главной книгой</span><span class="sxs-lookup"><span data-stu-id="91f56-119">How to: Reconcile Inventory Costs with the General Ledger</span></span>](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|<span data-ttu-id="91f56-120">Использование одного окна для аудита выверки книги инвентаризации и главной книги.</span><span class="sxs-lookup"><span data-stu-id="91f56-120">Use one window to audit the reconciliation between the inventory ledger and the general ledger.</span></span>|[<span data-ttu-id="91f56-121">Практическое руководство. Выверка себестоимости товаров с главной книгой</span><span class="sxs-lookup"><span data-stu-id="91f56-121">How to: Reconcile Inventory Costs with the General Ledger</span></span>](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|<span data-ttu-id="91f56-122">Определение суммы НЗП, которую необходимо учесть в балансовых счетах для отчетности по завершении периода.</span><span class="sxs-lookup"><span data-stu-id="91f56-122">Determine the WIP amount that needs to be posted to balance sheet accounts for period-end reporting.</span></span>|[<span data-ttu-id="91f56-123">Практическое руководство. Отслеживание хода выполнения работ и производительности</span><span class="sxs-lookup"><span data-stu-id="91f56-123">How to: Monitor Job Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)|

## <a name="see-also"></a><span data-ttu-id="91f56-124">См. также</span><span class="sxs-lookup"><span data-stu-id="91f56-124">See Also</span></span>  
[<span data-ttu-id="91f56-125">Настройка оценки стоимости запасов и учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="91f56-125">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)  
[<span data-ttu-id="91f56-126">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="91f56-126">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="91f56-127">Финансы</span><span class="sxs-lookup"><span data-stu-id="91f56-127">Finance</span></span>](finance.md)  
<span data-ttu-id="91f56-128">[Наличие](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="91f56-128">[Inventory](inventory-manage-inventory.md) </span></span>  
<span data-ttu-id="91f56-129">[Продажи](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="91f56-129">[Sales](sales-manage-sales.md) </span></span>  
[<span data-ttu-id="91f56-130">Покупки</span><span class="sxs-lookup"><span data-stu-id="91f56-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="91f56-131">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="91f56-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

