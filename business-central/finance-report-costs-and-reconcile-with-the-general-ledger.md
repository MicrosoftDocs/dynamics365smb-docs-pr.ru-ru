---
title: Отчет о затратах и выверка с главной книгой | Документация Майкрософт
description: В конце учетных периодов, месяцев, лет и т. д. должна выполняться последовательность задач аудита и управления себестоимостью для создания отчетов с правильной и сбалансированной стоимостью запасов для финансового отдела. Отдельно от подпрограммы учета, которая передает операции стоимости отдельных товаров в выделенные счета главной книги, существует несколько отчетов, а также функции отслеживания и специальное средство выверки, доступные для аудиторов и контролеров, ответственных за выполнений этой чрезвычайно важной для бизнеса работы.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: eafcf0bdd26e26903c17e43d37ca7e35b96f240c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301832"
---
# <a name="reporting-costs-and-reconciling-with-the-general-ledger"></a><span data-ttu-id="df1d6-104">Отчет о затратах и выверка с главной книгой</span><span class="sxs-lookup"><span data-stu-id="df1d6-104">Reporting Costs and Reconciling with the General Ledger</span></span>
<span data-ttu-id="df1d6-105">В конце учетных периодов, месяцев, лет и т. д. должна выполняться последовательность задач аудита и управления себестоимостью для создания отчетов с правильной и сбалансированной стоимостью запасов для финансового отдела.</span><span class="sxs-lookup"><span data-stu-id="df1d6-105">At the end of accounting periods, monthly, yearly or other, a sequence of cost control and auditing tasks must be performed to report a correct and balanced inventory value to the finance department.</span></span> <span data-ttu-id="df1d6-106">Отдельно от подпрограммы учета, которая передает операции стоимости отдельных товаров в выделенные счета главной книги, существует несколько отчетов, а также функции отслеживания и специальное средство выверки, доступные для аудиторов и контролеров, ответственных за выполнений этой чрезвычайно важной для бизнеса работы.</span><span class="sxs-lookup"><span data-stu-id="df1d6-106">Apart from the posting routine that transfers the individual item value entries to dedicated general ledger accounts, several reports, tracing functions, and a special reconciliation tool are available to the auditor or controller responsible for this business-critical work.</span></span>  

 <span data-ttu-id="df1d6-107">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="df1d6-107">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="df1d6-108">**Задача**</span><span class="sxs-lookup"><span data-stu-id="df1d6-108">**To**</span></span>|<span data-ttu-id="df1d6-109">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="df1d6-109">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="df1d6-110">Просмотр стоимости запасов для выбранных товаров, включая сведения о количестве и стоимости увеличения и уменьшения запасов за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="df1d6-110">View the inventory value of selected items, including information about the quantities and values of increases and decreases in inventory over a selected period.</span></span>|<span data-ttu-id="df1d6-111">Отчет **Оценка стоимости товаров**</span><span class="sxs-lookup"><span data-stu-id="df1d6-111">**Inventory Valuation** report</span></span>|  
|<span data-ttu-id="df1d6-112">Просмотр стоимости запасов для выбранных заказов на производство в НЗП (незавершенном производстве), таких как количество и стоимость потребления, использование производственных мощностей и выход по текущим производственным заказам.</span><span class="sxs-lookup"><span data-stu-id="df1d6-112">View the inventory value of selected production orders in your WIP (work in process) inventory, such as the quantities and values of consumption, capacity usage, and output in ongoing production orders.</span></span>|<span data-ttu-id="df1d6-113">Отчет **Оценка стоимости запасов - НЗП**</span><span class="sxs-lookup"><span data-stu-id="df1d6-113">**Inventory Valuation - WIP** report</span></span>|  
|<span data-ttu-id="df1d6-114">Просмотр стоимости запасов для выбранных товаров, включая их фактическую и ожидаемую себестоимость на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="df1d6-114">View the inventory value of selected items, including their actual and expected cost on the date specified.</span></span>|<span data-ttu-id="df1d6-115">Отчет **Оценка запасов - специф. себест.**</span><span class="sxs-lookup"><span data-stu-id="df1d6-115">**Invt. Valuation - Cost Spec.** report</span></span>|  
|<span data-ttu-id="df1d6-116">Использование отчета для анализа причин отклонения себестоимости или анализа доли себестоимости для проданных товаров (себестоимости продажи).</span><span class="sxs-lookup"><span data-stu-id="df1d6-116">Use a report to analyze the reasons for cost variances or to gain insight into the cost shares of sold items (COGS).</span></span>|<span data-ttu-id="df1d6-117">Отчет **Анализ структуры себестоимости**</span><span class="sxs-lookup"><span data-stu-id="df1d6-117">**Cost Shares Breakdown** report</span></span>|  
|<span data-ttu-id="df1d6-118">Периодический учет операций стоимости транзакций товаров из книги инвентаризации в связанных счетах ГК для выверки двух книг.</span><span class="sxs-lookup"><span data-stu-id="df1d6-118">Periodically post the value entries of item transactions from the inventory ledger to the related G/L accounts to reconcile the two ledgers.</span></span>|[<span data-ttu-id="df1d6-119">Выверка себестоимости товаров с главной книгой</span><span class="sxs-lookup"><span data-stu-id="df1d6-119">Reconcile Inventory Costs with the General Ledger</span></span>](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|<span data-ttu-id="df1d6-120">Определение суммы НЗП, которую необходимо учесть в балансовых счетах для отчетности по завершении периода.</span><span class="sxs-lookup"><span data-stu-id="df1d6-120">Determine the WIP amount that needs to be posted to balance sheet accounts for period-end reporting.</span></span>|[<span data-ttu-id="df1d6-121">Отслеживание хода выполнения работ и производительности</span><span class="sxs-lookup"><span data-stu-id="df1d6-121">Monitor Job Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)|

## <a name="see-also"></a><span data-ttu-id="df1d6-122">См. также</span><span class="sxs-lookup"><span data-stu-id="df1d6-122">See Also</span></span>  
[<span data-ttu-id="df1d6-123">Настройка оценки стоимости запасов и учета себестоимости</span><span class="sxs-lookup"><span data-stu-id="df1d6-123">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)  
[<span data-ttu-id="df1d6-124">Управление себестоимостью товаров</span><span class="sxs-lookup"><span data-stu-id="df1d6-124">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="df1d6-125">Финансы</span><span class="sxs-lookup"><span data-stu-id="df1d6-125">Finance</span></span>](finance.md)  
<span data-ttu-id="df1d6-126">[Наличие](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="df1d6-126">[Inventory](inventory-manage-inventory.md) </span></span>  
<span data-ttu-id="df1d6-127">[Продажи](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="df1d6-127">[Sales](sales-manage-sales.md) </span></span>  
[<span data-ttu-id="df1d6-128">Покупки</span><span class="sxs-lookup"><span data-stu-id="df1d6-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="df1d6-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="df1d6-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
