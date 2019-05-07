---
title: Автоматическое перемещение и объединенные операции | Документы Майкрософт
description: В модуле "Учет затрат" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета. В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции. В следующей таблице описаны разные параметры.
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
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 8f6b5328b3a7b8cdcb4582deda363bdd0361ed9a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "941158"
---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="5d52c-105">Автоматическое перемещение и объединенные операции</span><span class="sxs-lookup"><span data-stu-id="5d52c-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="5d52c-106">В модуле "Учет затрат" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета.</span><span class="sxs-lookup"><span data-stu-id="5d52c-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="5d52c-107">В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции.</span><span class="sxs-lookup"><span data-stu-id="5d52c-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="5d52c-108">В следующей таблице описаны разные параметры.</span><span class="sxs-lookup"><span data-stu-id="5d52c-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="5d52c-109">Объединить операции</span><span class="sxs-lookup"><span data-stu-id="5d52c-109">Combine entries</span></span>|<span data-ttu-id="5d52c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d52c-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="5d52c-111">Нет</span><span class="sxs-lookup"><span data-stu-id="5d52c-111">None</span></span>|<span data-ttu-id="5d52c-112">Каждая операция Главной книги переносится по отдельности на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="5d52c-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="5d52c-113">День</span><span class="sxs-lookup"><span data-stu-id="5d52c-113">Day</span></span>|<span data-ttu-id="5d52c-114">Записи Главной книги с одной и той же датой учета переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="5d52c-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="5d52c-115">Месяц</span><span class="sxs-lookup"><span data-stu-id="5d52c-115">Month</span></span>|<span data-ttu-id="5d52c-116">Все операции Главной книги в одном и том же календарном месяце переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="5d52c-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="5d52c-117">Если установлен флажок **Автоматический перенос из ГК** на странице **Настройка учета затрат**, [!INCLUDE[d365fin](includes/d365fin_md.md)] обновляет учет затрат после каждого учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="5d52c-117">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="5d52c-118">Объединенные операции невозможны.</span><span class="sxs-lookup"><span data-stu-id="5d52c-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5d52c-119">См. также</span><span class="sxs-lookup"><span data-stu-id="5d52c-119">See Also</span></span>  
 <span data-ttu-id="5d52c-120">[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="5d52c-120">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="5d52c-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5d52c-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
