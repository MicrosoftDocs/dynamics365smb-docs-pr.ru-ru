---
title: Автоматическое перемещение и объединенные операции | Документация Майкрософт
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
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: finance-transfer-and-post-cost-entries
ms.openlocfilehash: 0c07e470c1df8b9d9b5e7f7c833ff83b3c61be69
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2306440"
---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="a849a-105">Автоматическое перемещение и объединенные операции</span><span class="sxs-lookup"><span data-stu-id="a849a-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="a849a-106">В модуле "Учет затрат" можно переместить операции Главной книги по типу затрат с помощью комбинированного учета.</span><span class="sxs-lookup"><span data-stu-id="a849a-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="a849a-107">В поле **Объединить операции** в определении типа затрат можно указать, используются ли для типа затрат объединенные операции.</span><span class="sxs-lookup"><span data-stu-id="a849a-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="a849a-108">В следующей таблице описаны разные параметры.</span><span class="sxs-lookup"><span data-stu-id="a849a-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="a849a-109">Объединить операции</span><span class="sxs-lookup"><span data-stu-id="a849a-109">Combine entries</span></span>|<span data-ttu-id="a849a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a849a-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="a849a-111">Нет</span><span class="sxs-lookup"><span data-stu-id="a849a-111">None</span></span>|<span data-ttu-id="a849a-112">Каждая операция Главной книги переносится по отдельности на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="a849a-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="a849a-113">День</span><span class="sxs-lookup"><span data-stu-id="a849a-113">Day</span></span>|<span data-ttu-id="a849a-114">Записи Главной книги с одной и той же датой учета переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="a849a-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="a849a-115">Месяц</span><span class="sxs-lookup"><span data-stu-id="a849a-115">Month</span></span>|<span data-ttu-id="a849a-116">Все операции Главной книги в одном и том же календарном месяце переносятся как одна операция на соответствующий тип затрат.</span><span class="sxs-lookup"><span data-stu-id="a849a-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="a849a-117">Если установлен флажок **Автоматический перенос из ГК** на странице **Настройка учета затрат**, [!INCLUDE[d365fin](includes/d365fin_md.md)] обновляет учет затрат после каждого учета в главной книге.</span><span class="sxs-lookup"><span data-stu-id="a849a-117">If you have selected the **Auto Transfer from G/L** check box on the **Cost Accounting Setup** page, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="a849a-118">Объединенные операции невозможны.</span><span class="sxs-lookup"><span data-stu-id="a849a-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a849a-119">См. также</span><span class="sxs-lookup"><span data-stu-id="a849a-119">See Also</span></span>  
 <span data-ttu-id="a849a-120">[Перемещение и операции учета затрат](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="a849a-120">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="a849a-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a849a-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
