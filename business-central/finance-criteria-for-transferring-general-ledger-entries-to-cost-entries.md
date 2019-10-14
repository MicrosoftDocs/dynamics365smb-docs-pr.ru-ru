---
title: Критерии для переноса операций главной книги в операции затрат | Документация Майкрософт
description: Важно понимать критерии для переноса операций Главной книги в операции затрат. Во время перемещения пакетное задание **Перенести записи ГК в CA** использует следующие критерии, чтобы определить, перемещаются ли операции главной книги и если да, то как.
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
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: fe7a7d0c3d7a56f129a1ae94d1e7f015eb145bda
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302456"
---
# <a name="criteria-for-transferring-general-ledger-entries-to-cost-entries"></a><span data-ttu-id="28c9e-104">Критерии для переноса операций главной книги в операции затрат</span><span class="sxs-lookup"><span data-stu-id="28c9e-104">Criteria for Transferring General Ledger Entries to Cost Entries</span></span>
<span data-ttu-id="28c9e-105">Важно понимать критерии для переноса операций Главной книги в операции затрат.</span><span class="sxs-lookup"><span data-stu-id="28c9e-105">It is important to understand the criteria for transferring general ledger entries to cost entries.</span></span> <span data-ttu-id="28c9e-106">Во время перемещения пакетное задание **Перенести записи ГК в CA** использует следующие критерии, чтобы определить, перемещаются ли операции главной книги и если да, то как.</span><span class="sxs-lookup"><span data-stu-id="28c9e-106">During the transfer, the **Transfer GL Entries to CA** batch job uses the following criteria to determine if and how the general ledger entries are transferred.</span></span>  

<span data-ttu-id="28c9e-107">Записи Главной книги переносятся, если:</span><span class="sxs-lookup"><span data-stu-id="28c9e-107">General ledger entries are transferred if:</span></span>  

-   <span data-ttu-id="28c9e-108">Для операций предусмотрены значения измерения, соответствующие либо месту возникновения затрат, либо объекту затрат.</span><span class="sxs-lookup"><span data-stu-id="28c9e-108">The entries have dimension values corresponding to either a cost center or a cost object.</span></span>  
-   <span data-ttu-id="28c9e-109">Для операций предусмотрены значения измерения, соответствующие месту возникновения затрат и объекту затрат.</span><span class="sxs-lookup"><span data-stu-id="28c9e-109">The entries have dimension values that correspond to a cost center and a cost object.</span></span> <span data-ttu-id="28c9e-110">Для этих записей место возникновения затрат имеет преимущество.</span><span class="sxs-lookup"><span data-stu-id="28c9e-110">For these entries, the cost center takes precedence.</span></span> <span data-ttu-id="28c9e-111">Это помогает избежать ситуации, в которой тип затрат появляется как в объекте затрат, так и в месте возникновения затрат, и поэтому дважды учитывается в статистике.</span><span class="sxs-lookup"><span data-stu-id="28c9e-111">This helps avoid a situation where a cost type appears in both a cost object and a cost center and is therefore counted twice in the statistics.</span></span>  
-   <span data-ttu-id="28c9e-112">Номер документа в операциях является пустым, поэтому он будет отображаться как 0000 в операциях затрат.</span><span class="sxs-lookup"><span data-stu-id="28c9e-112">The document number in the entries is empty, so it will appear with a document number of 0000 in the cost entries.</span></span>  
-   <span data-ttu-id="28c9e-113">Операции переносятся в тип затрат, который позволяет использовать совмещенные операции, и такие операции переносятся как совмещенная операция ежемесячно или ежедневно.</span><span class="sxs-lookup"><span data-stu-id="28c9e-113">The entries are transferred to a cost type that allows for combined entries and these entries are transferred as a combined entry either monthly or daily.</span></span>  

<span data-ttu-id="28c9e-114">Записи Главной книги не переносятся, если:</span><span class="sxs-lookup"><span data-stu-id="28c9e-114">General ledger entries are not transferred if:</span></span>  

-   <span data-ttu-id="28c9e-115">Для операций предусмотрены значения измерения, не соответствующие месту возникновения затрат или объекту затрат.</span><span class="sxs-lookup"><span data-stu-id="28c9e-115">The entries have dimension values that do not correspond to a cost center or a cost object.</span></span>  
-   <span data-ttu-id="28c9e-116">Операции имеют нулевую сумму.</span><span class="sxs-lookup"><span data-stu-id="28c9e-116">The entries have an amount of zero.</span></span>  
-   <span data-ttu-id="28c9e-117">У операций имеется счет главной книги, который был удален.</span><span class="sxs-lookup"><span data-stu-id="28c9e-117">The entries have a general ledger account that has been deleted.</span></span>  
-   <span data-ttu-id="28c9e-118">У операций имеется счет главной книги, тип которого отличается от **Счет прибылей и убытков**.</span><span class="sxs-lookup"><span data-stu-id="28c9e-118">The entries have a general ledger account that is not of the type **Income Statement**.</span></span>  
-   <span data-ttu-id="28c9e-119">У операций имеется счет главной книги, для которого не задан тип себестоимости.</span><span class="sxs-lookup"><span data-stu-id="28c9e-119">The entries have a general ledger account that is not assigned a cost type.</span></span>  
-   <span data-ttu-id="28c9e-120">У операций имеется дата учета до **Начальная дата для перемещения ГК**.</span><span class="sxs-lookup"><span data-stu-id="28c9e-120">The entries have a posting date before the **Starting Date for G/L Transfer**.</span></span>  
-   <span data-ttu-id="28c9e-121">Операции были учтены с датой закрытия.</span><span class="sxs-lookup"><span data-stu-id="28c9e-121">The entries have been posted with a closing date.</span></span> <span data-ttu-id="28c9e-122">Обычно это операции, которые обнуляют баланс отчета о прибылях в конце года.</span><span class="sxs-lookup"><span data-stu-id="28c9e-122">These are typically entries that set back the balance of the income statement at the end of the year.</span></span>  

## <a name="see-also"></a><span data-ttu-id="28c9e-123">См. также</span><span class="sxs-lookup"><span data-stu-id="28c9e-123">See Also</span></span>  
[<span data-ttu-id="28c9e-124">Учет по затратам</span><span class="sxs-lookup"><span data-stu-id="28c9e-124">Accounting for Costs</span></span>](finance-manage-cost-accounting.md)  
 <span data-ttu-id="28c9e-125">[Перенос операций ГК в операции затрат](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="28c9e-125">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="28c9e-126">[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="28c9e-126">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 [<span data-ttu-id="28c9e-127">Об учете затрат</span><span class="sxs-lookup"><span data-stu-id="28c9e-127">About Cost Accounting</span></span>](finance-about-cost-accounting.md)  
 <span data-ttu-id="28c9e-128">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="28c9e-128">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
