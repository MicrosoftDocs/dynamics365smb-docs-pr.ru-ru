---
title: "Автоматическое перемещение и объединенные операции | Документы Майкрософт"
description: "В модуле \"Учет затрат\" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета. В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции. В следующей таблице описаны разные параметры."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: d33fa549f48731c49734e7ecaf65b461c375ec90
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="cad02-105">Автоматическое перемещение и объединенные операции</span><span class="sxs-lookup"><span data-stu-id="cad02-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="cad02-106">В модуле "Учет затрат" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета.</span><span class="sxs-lookup"><span data-stu-id="cad02-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="cad02-107">В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции.</span><span class="sxs-lookup"><span data-stu-id="cad02-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="cad02-108">В следующей таблице описаны разные параметры.</span><span class="sxs-lookup"><span data-stu-id="cad02-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="cad02-109">Объединить операции</span><span class="sxs-lookup"><span data-stu-id="cad02-109">Combine entries</span></span>|<span data-ttu-id="cad02-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cad02-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="cad02-111">Нет</span><span class="sxs-lookup"><span data-stu-id="cad02-111">None</span></span>|<span data-ttu-id="cad02-112">Каждая операция Главной книги переносится по отдельности на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="cad02-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="cad02-113">День</span><span class="sxs-lookup"><span data-stu-id="cad02-113">Day</span></span>|<span data-ttu-id="cad02-114">Записи Главной книги с одной и той же датой учета переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="cad02-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="cad02-115">Месяц</span><span class="sxs-lookup"><span data-stu-id="cad02-115">Month</span></span>|<span data-ttu-id="cad02-116">Все операции Главной книги в одном и том же календарном месяце переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="cad02-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="cad02-117">Если установлен флажок **Автоматический перенос из ГК** в окне **Настройка учета затрат**, [!INCLUDE[d365fin](includes/d365fin_md.md)] обновляет учет затрат после каждого учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="cad02-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="cad02-118">Объединенные операции невозможны.</span><span class="sxs-lookup"><span data-stu-id="cad02-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="cad02-119">См. также</span><span class="sxs-lookup"><span data-stu-id="cad02-119">See Also</span></span>  
 <span data-ttu-id="cad02-120">[Перенос операций ГК в операции затрат](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="cad02-120">[Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="cad02-121">[Критерии для переноса операций главной книги в операции затрат](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="cad02-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="cad02-122">[Результаты перемещения](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="cad02-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="cad02-123">Перемещение и операции учета затрат</span><span class="sxs-lookup"><span data-stu-id="cad02-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="cad02-124">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="cad02-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

