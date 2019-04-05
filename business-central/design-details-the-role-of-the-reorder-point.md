---
title: Сведения о проектировании — роль точки дозаказа | Документы Майкрософт
description: В этом разделе подчеркивается важность задания момента повторного заказа, чтобы знать, когда заказывать дополнительные запасы.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: e39a7efdc796e8745bd9d8f7d74cdcfb171d851f
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805310"
---
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="e0858-103">Сведения о проектировании: роль точки дозаказа</span><span class="sxs-lookup"><span data-stu-id="e0858-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="e0858-104">В дополнение к общей балансировке спроса и поставки система планирования также отслеживает уровни запасов для соответствующих товаров, чтобы соблюсти требования политики дозаказа.</span><span class="sxs-lookup"><span data-stu-id="e0858-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  

<span data-ttu-id="e0858-105">Точка дозаказа представляет спрос во время подготовки.</span><span class="sxs-lookup"><span data-stu-id="e0858-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="e0858-106">Когда прогнозируемые запасы опускаются ниже уровня запасов, определенного точкой повторного заказа, время заказывать дополнительное количество.</span><span class="sxs-lookup"><span data-stu-id="e0858-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="e0858-107">В то же время ожидается, что запас будет постепенно уменьшатся и, возможно, достигнет нуля (или уровня страхового запаса), пока не поступит пополнение.</span><span class="sxs-lookup"><span data-stu-id="e0858-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  

<span data-ttu-id="e0858-108">Соответственно, система планирования предложит заказ на поставку с прямым планированием в момент перехода прогнозируемых запасов ниже точки дозаказа.</span><span class="sxs-lookup"><span data-stu-id="e0858-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  

<span data-ttu-id="e0858-109">Точка повторного заказа отражает определенный уровень запасов.</span><span class="sxs-lookup"><span data-stu-id="e0858-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="e0858-110">Однако уровни запасов могут сильно перемещаться в горизонте планирования, и, следовательно, система планирования должна постоянно контролировать прогнозируемые доступные запасы.</span><span class="sxs-lookup"><span data-stu-id="e0858-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e0858-111">См. также</span><span class="sxs-lookup"><span data-stu-id="e0858-111">See Also</span></span>  
<span data-ttu-id="e0858-112">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="e0858-112">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="e0858-113">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="e0858-113">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="e0858-114">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="e0858-114">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="e0858-115">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="e0858-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
