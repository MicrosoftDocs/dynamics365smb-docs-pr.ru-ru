---
title: Определение центров затрат и объектов затрат для плана счетов | Документы Майкрософт
description: Можно автоматически передавать операции доходов и расходов из главной книги в модуль учета затрат или для каждого учета главной книги или с помощью пакетного задания. При выполнении перемещения система выполняет перемещение только тех записей, которые уже связаны с центром затрат или объектом затрат. Чтобы настроить содержательное перемещение, необходимо обеспечить, чтобы места возникновения затрат и объекты затрат были правильно определены.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
redirect_url: finance-set-up-cost-accounting
ms.openlocfilehash: 00c0ac4a37476c2ab21ddc850e80e7abeb5eda18
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1242058"
---
# <a name="defining-cost-centers-and-cost-objects-for-chart-of-accounts"></a><span data-ttu-id="8552c-105">Определение центров затрат и объектов затрат для плана счетов</span><span class="sxs-lookup"><span data-stu-id="8552c-105">Defining Cost Centers and Cost Objects for Chart of Accounts</span></span>
<span data-ttu-id="8552c-106">Можно автоматически передавать операции доходов и расходов из главной книги в модуль учета затрат или для каждого учета главной книги или с помощью пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="8552c-106">You can automatically transfer the expense and income entries from the general ledger to cost accounting either for each general ledger posting or with a batch job.</span></span> <span data-ttu-id="8552c-107">При выполнении перемещения [!INCLUDE[d365fin](includes/d365fin_md.md)] выполняет перемещение только тех записей, которые уже связаны с центром затрат или объектом затрат.</span><span class="sxs-lookup"><span data-stu-id="8552c-107">When you do the transfer, [!INCLUDE[d365fin](includes/d365fin_md.md)] only transfers the entries that are already linked to a cost center or a cost object.</span></span> <span data-ttu-id="8552c-108">Чтобы настроить содержательное перемещение, необходимо обеспечить, чтобы места возникновения затрат и объекты затрат были правильно определены.</span><span class="sxs-lookup"><span data-stu-id="8552c-108">To establish a meaningful transfer, you must ensure that the cost centers and cost objects are correctly defined.</span></span>  

## <a name="defining-default-dimension-values-for-general-ledger-accounts"></a><span data-ttu-id="8552c-109">Определение значений измерений по умолчанию для счетов главной книги</span><span class="sxs-lookup"><span data-stu-id="8552c-109">Defining Default Dimension Values for General Ledger Accounts</span></span>  
<span data-ttu-id="8552c-110">Для каждого счета главной книги можно определить значения измерений по умолчанию в таблице **Измерение по умолчанию**.</span><span class="sxs-lookup"><span data-stu-id="8552c-110">For each general ledger account, you can define default dimension values in the **Default Dimension** table.</span></span> <span data-ttu-id="8552c-111">В следующем примере представлен способ определения того, чтобы всегда было место возникновения затрат ПОДРАЗДЕЛЕНИЕ, но никогда — место возникновения затрат ПРОЕКТ, при учете на счете главной книги.</span><span class="sxs-lookup"><span data-stu-id="8552c-111">The following example shows how to define that there should always be a DEPARTMENT cost center, but never be a PROJECT cost object when posting to a general ledger account.</span></span>  

|<span data-ttu-id="8552c-112">**Код измерения**</span><span class="sxs-lookup"><span data-stu-id="8552c-112">**Dimension Code**</span></span>|<span data-ttu-id="8552c-113">**Учет значения**</span><span class="sxs-lookup"><span data-stu-id="8552c-113">**Value Posting**</span></span>|  
|------------------------------------------|-----------------------------------------|  
|<span data-ttu-id="8552c-114">Отдел</span><span class="sxs-lookup"><span data-stu-id="8552c-114">Department</span></span>|<span data-ttu-id="8552c-115">Код обязателен</span><span class="sxs-lookup"><span data-stu-id="8552c-115">Code Mandatory</span></span>|  
|<span data-ttu-id="8552c-116">Проект</span><span class="sxs-lookup"><span data-stu-id="8552c-116">Project</span></span>|<span data-ttu-id="8552c-117">Нет кода</span><span class="sxs-lookup"><span data-stu-id="8552c-117">No Code</span></span>|  

## <a name="defining-dimension-values-for-overhead-costs-and-direct-costs"></a><span data-ttu-id="8552c-118">Определение значений измерений для накладных расходов и прямой себестоимости</span><span class="sxs-lookup"><span data-stu-id="8552c-118">Defining Dimension Values for Overhead Costs and Direct Costs</span></span>  
 <span data-ttu-id="8552c-119">Можно перенести накладные расходы в место возникновения затрат и прямую себестоимость в объект затрат.</span><span class="sxs-lookup"><span data-stu-id="8552c-119">You can transfer overhead costs to a cost center and direct costs to a cost object.</span></span> <span data-ttu-id="8552c-120">В следующей таблице представлена оптимальная комбинация значений набора измерений.</span><span class="sxs-lookup"><span data-stu-id="8552c-120">The following table shows the optimal combination of the dimension setup values.</span></span>  

|<span data-ttu-id="8552c-121">Переместить в</span><span class="sxs-lookup"><span data-stu-id="8552c-121">Transfer To</span></span>|<span data-ttu-id="8552c-122">Учет места возникновения затрат</span><span class="sxs-lookup"><span data-stu-id="8552c-122">Cost Center Posting</span></span>|<span data-ttu-id="8552c-123">Учет объектов затрат</span><span class="sxs-lookup"><span data-stu-id="8552c-123">Cost Object Posting</span></span>|  
|-----------------|-------------------------|-------------------------|  
|<span data-ttu-id="8552c-124">Место возникновения затрат</span><span class="sxs-lookup"><span data-stu-id="8552c-124">Cost Center</span></span>|<span data-ttu-id="8552c-125">Код обязателен</span><span class="sxs-lookup"><span data-stu-id="8552c-125">Code Mandatory</span></span>|<span data-ttu-id="8552c-126">Нет кода</span><span class="sxs-lookup"><span data-stu-id="8552c-126">No Code</span></span>|  
|<span data-ttu-id="8552c-127">Объект затрат</span><span class="sxs-lookup"><span data-stu-id="8552c-127">Cost Object</span></span>|<span data-ttu-id="8552c-128">Нет кода</span><span class="sxs-lookup"><span data-stu-id="8552c-128">No Code</span></span>|<span data-ttu-id="8552c-129">Код обязателен</span><span class="sxs-lookup"><span data-stu-id="8552c-129">Code Mandatory</span></span>|  

> [!NOTE]  
>  <span data-ttu-id="8552c-130">Чтобы убедиться в том, что предопределенный центр затрат и объект затрат, настраиваемые в главной книге, автоматически перенесены в модуль учета затрат, установите флажок **Проверка разносок ГК** на странице "Настройка учета затрат".</span><span class="sxs-lookup"><span data-stu-id="8552c-130">To make sure that the predefined cost center and cost object that you set up in the general ledger are automatically carried over to cost accounting, select the **Check G/L Postings** check box in the Cost Accounting Setup page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8552c-131">См. также</span><span class="sxs-lookup"><span data-stu-id="8552c-131">See Also</span></span>  
[<span data-ttu-id="8552c-132">Учет по затратам</span><span class="sxs-lookup"><span data-stu-id="8552c-132">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
[<span data-ttu-id="8552c-133">Настройка учета затрат</span><span class="sxs-lookup"><span data-stu-id="8552c-133">Setting Up Cost Accounting</span></span>](finance-set-up-cost-accounting.md)  
<span data-ttu-id="8552c-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8552c-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
