---
title: "Автоматическое перемещение и объединенные операции | Документы Майкрософт"
description: "В модуле \"Учет затрат\" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета. В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции. В следующей таблице описаны разные параметры."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: f4796d9796788d2fbbf5706688aec75a4ed9a6d8
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="150b6-105">Автоматическое перемещение и объединенные операции</span><span class="sxs-lookup"><span data-stu-id="150b6-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="150b6-106">В модуле "Учет затрат" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета.</span><span class="sxs-lookup"><span data-stu-id="150b6-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="150b6-107">В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции.</span><span class="sxs-lookup"><span data-stu-id="150b6-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="150b6-108">В следующей таблице описаны разные параметры.</span><span class="sxs-lookup"><span data-stu-id="150b6-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="150b6-109">Объединить операции</span><span class="sxs-lookup"><span data-stu-id="150b6-109">Combine entries</span></span>|<span data-ttu-id="150b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="150b6-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="150b6-111">Нет</span><span class="sxs-lookup"><span data-stu-id="150b6-111">None</span></span>|<span data-ttu-id="150b6-112">Каждая операция Главной книги переносится по отдельности на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="150b6-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="150b6-113">День</span><span class="sxs-lookup"><span data-stu-id="150b6-113">Day</span></span>|<span data-ttu-id="150b6-114">Записи Главной книги с одной и той же датой учета переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="150b6-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="150b6-115">Месяц</span><span class="sxs-lookup"><span data-stu-id="150b6-115">Month</span></span>|<span data-ttu-id="150b6-116">Все операции Главной книги в одном и том же календарном месяце переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="150b6-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="150b6-117">Если установлен флажок **Автоматический перенос из ГК** в окне **Настройка учета затрат**, [!INCLUDE[d365fin](includes/d365fin_md.md)] обновляет учет затрат после каждого учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="150b6-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="150b6-118">Объединенные операции невозможны.</span><span class="sxs-lookup"><span data-stu-id="150b6-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="150b6-119">См. также</span><span class="sxs-lookup"><span data-stu-id="150b6-119">See Also</span></span>  
 <span data-ttu-id="150b6-120">[Перенос операций ГК в операции затрат](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="150b6-120">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="150b6-121">[Критерии для переноса операций главной книги в операции затрат](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="150b6-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="150b6-122">[Результаты перемещения](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="150b6-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="150b6-123">Перемещение и операции учета затрат</span><span class="sxs-lookup"><span data-stu-id="150b6-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="150b6-124">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="150b6-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

