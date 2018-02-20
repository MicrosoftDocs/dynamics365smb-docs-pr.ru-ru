---
title: "Сведения о проектировании — краткие сведения о балансировке | Документы Майкрософт"
description: "Спрос предоставляется клиентами организации. Поставка — это то, что организация может создать или удалить для обеспечения баланса. Система планирования начинает с независимого спроса, а затем в обратном направлении выполняет отслеживание до предложения."
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: a87fb83e2fad2c99de9938f87ef6f83db9c64dc4
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---
# <a name="design-details-the-concept-of-balancing-in-brief"></a><span data-ttu-id="8de54-105">Сведения о проектировании: краткие сведения о балансировке</span><span class="sxs-lookup"><span data-stu-id="8de54-105">Design Details: The Concept of Balancing in Brief</span></span>
<span data-ttu-id="8de54-106">Спрос предоставляется клиентами организации.</span><span class="sxs-lookup"><span data-stu-id="8de54-106">Demand is given by a company’s customers.</span></span> <span data-ttu-id="8de54-107">Поставка — это то, что организация может создать или удалить для обеспечения баланса.</span><span class="sxs-lookup"><span data-stu-id="8de54-107">Supply is what the company can create and remove to establish balance.</span></span> <span data-ttu-id="8de54-108">Система планирования начинает с независимого спроса, а затем в обратном направлении выполняет отслеживание до предложения.</span><span class="sxs-lookup"><span data-stu-id="8de54-108">The planning system starts with the independent demand and then tracks backwards to the supply.</span></span>  
  
 <span data-ttu-id="8de54-109">Профили инвентаризации используются для хранения информации о спросе и предложении, количествах и времени.</span><span class="sxs-lookup"><span data-stu-id="8de54-109">The inventory profiles are used to contain information about the demands and supplies, quantities, and timing.</span></span> <span data-ttu-id="8de54-110">Эти профили составляют две стороны шкалы уравновешивания.</span><span class="sxs-lookup"><span data-stu-id="8de54-110">These profiles essentially make up the two sides of the balancing scale.</span></span>  
  
 <span data-ttu-id="8de54-111">Задача механизма планирования — уравновешивать спрос и предложение товара, чтобы убедиться, что предложение соответствует спросу и это достигается целесообразным способом, как определено параметрами и правилами планирования.</span><span class="sxs-lookup"><span data-stu-id="8de54-111">The objective of the planning mechanism is to counterbalance the demand and supply of an item to ensure that supply will match demand in a feasible way as defined by the planning parameters and rules.</span></span>  
  
 <span data-ttu-id="8de54-112">![](media/nav_app_supply_planning_2_balancing.png "NAV_APP_supply_planning_2_balancing")</span><span class="sxs-lookup"><span data-stu-id="8de54-112">![](media/nav_app_supply_planning_2_balancing.png "NAV_APP_supply_planning_2_balancing")</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="8de54-113">См. также</span><span class="sxs-lookup"><span data-stu-id="8de54-113">See Also</span></span>  
 <span data-ttu-id="8de54-114">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="8de54-114">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="8de54-115">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="8de54-115">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="8de54-116">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="8de54-116">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
