---
title: "Сведения о проектировании — роль точки дозаказа | Документы Майкрософт"
description: "В этом разделе подчеркивается важность задания момента повторного заказа, чтобы знать, когда заказывать дополнительные запасы."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: a64d71ca9f163793c959126da09ffa4ef281b5e0
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-the-role-of-the-reorder-point"></a><span data-ttu-id="a9e26-103">Сведения о проектировании: роль точки дозаказа</span><span class="sxs-lookup"><span data-stu-id="a9e26-103">Design Details: The Role of the Reorder Point</span></span>
<span data-ttu-id="a9e26-104">В дополнение к общей балансировке спроса и поставки система планирования также отслеживает уровни запасов для соответствующих товаров, чтобы соблюсти требования политики дозаказа.</span><span class="sxs-lookup"><span data-stu-id="a9e26-104">In addition to the general balancing of supply and demand, the planning system must also monitor inventory levels for the affected items to respect the defined reordering policies.</span></span>  
  
<span data-ttu-id="a9e26-105">Точка дозаказа представляет спрос во время подготовки.</span><span class="sxs-lookup"><span data-stu-id="a9e26-105">A reorder point represents demand during lead time.</span></span> <span data-ttu-id="a9e26-106">Когда прогнозируемые запасы опускаются ниже уровня запасов, определенного точкой повторного заказа, время заказывать дополнительное количество.</span><span class="sxs-lookup"><span data-stu-id="a9e26-106">When the projected inventory passes below the inventory level defined by the reorder point, it is time to order more quantity.</span></span> <span data-ttu-id="a9e26-107">В то же время ожидается, что запас будет постепенно уменьшатся и, возможно, достигнет нуля (или уровня страхового запаса), пока не поступит пополнение.</span><span class="sxs-lookup"><span data-stu-id="a9e26-107">Meanwhile, the inventory is expected to decrease gradually and possibly reach zero (or the safety stock level), until the replenishment arrives.</span></span>  
  
<span data-ttu-id="a9e26-108">Соответственно, система планирования предложит заказ на поставку с прямым планированием в момент перехода прогнозируемых запасов ниже точки дозаказа.</span><span class="sxs-lookup"><span data-stu-id="a9e26-108">Accordingly, the planning system will suggest a forward-scheduled supply order at the point when the projected inventory passes below the reorder point.</span></span>  
  
<span data-ttu-id="a9e26-109">Точка повторного заказа отражает определенный уровень запасов.</span><span class="sxs-lookup"><span data-stu-id="a9e26-109">The reorder point reflects a certain inventory level.</span></span> <span data-ttu-id="a9e26-110">Однако уровни запасов могут сильно перемещаться в горизонте планирования, и, следовательно, система планирования должна постоянно контролировать прогнозируемые доступные запасы.</span><span class="sxs-lookup"><span data-stu-id="a9e26-110">However, inventory levels can move significantly during the time bucket and, therefore, the planning system must constantly monitor the projected available inventory.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a9e26-111">См. также</span><span class="sxs-lookup"><span data-stu-id="a9e26-111">See Also</span></span>  
<span data-ttu-id="a9e26-112">[Сведения о проектировании: политики дозаказа](design-details-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a9e26-112">[Design Details: Reordering Policies](design-details-reordering-policies.md) </span></span>  
<span data-ttu-id="a9e26-113">[Сведения о проектировании: параметры планирования](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="a9e26-113">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="a9e26-114">[Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="a9e26-114">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="a9e26-115">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="a9e26-115">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
