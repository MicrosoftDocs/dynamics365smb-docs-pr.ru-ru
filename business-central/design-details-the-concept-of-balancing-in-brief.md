---
title: Сведения о проектировании — краткие сведения о балансировке | Документация Майкрософт
description: Спрос предоставляется клиентами организации. Поставка — это то, что организация может создать или удалить для обеспечения баланса. Система планирования начинает с независимого спроса, а затем в обратном направлении выполняет отслеживание до предложения.
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
redirect_url: design-details-balancing-demand-and-supply
ms.openlocfilehash: af63bf59def37fe873cb66366864855db52bd245
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302960"
---
# <a name="design-details-the-concept-of-balancing-in-brief"></a><span data-ttu-id="55a70-105">Сведения о проектировании: краткие сведения о балансировке</span><span class="sxs-lookup"><span data-stu-id="55a70-105">Design Details: The Concept of Balancing in Brief</span></span>
<span data-ttu-id="55a70-106">Спрос предоставляется клиентами организации.</span><span class="sxs-lookup"><span data-stu-id="55a70-106">Demand is given by a company’s customers.</span></span> <span data-ttu-id="55a70-107">Поставка — это то, что организация может создать или удалить для обеспечения баланса.</span><span class="sxs-lookup"><span data-stu-id="55a70-107">Supply is what the company can create and remove to establish balance.</span></span> <span data-ttu-id="55a70-108">Система планирования начинает с независимого спроса, а затем в обратном направлении выполняет отслеживание до предложения.</span><span class="sxs-lookup"><span data-stu-id="55a70-108">The planning system starts with the independent demand and then tracks backwards to the supply.</span></span>  

 <span data-ttu-id="55a70-109">Профили инвентаризации используются для хранения информации о спросе и предложении, количествах и времени.</span><span class="sxs-lookup"><span data-stu-id="55a70-109">The inventory profiles are used to contain information about the demands and supplies, quantities, and timing.</span></span> <span data-ttu-id="55a70-110">Эти профили составляют две стороны шкалы уравновешивания.</span><span class="sxs-lookup"><span data-stu-id="55a70-110">These profiles essentially make up the two sides of the balancing scale.</span></span>  

 <span data-ttu-id="55a70-111">Задача механизма планирования — уравновешивать спрос и предложение товара, чтобы убедиться, что предложение соответствует спросу и это достигается целесообразным способом, как определено параметрами и правилами планирования.</span><span class="sxs-lookup"><span data-stu-id="55a70-111">The objective of the planning mechanism is to counterbalance the demand and supply of an item to ensure that supply will match demand in a feasible way as defined by the planning parameters and rules.</span></span>  

 <span data-ttu-id="55a70-112">![Обзор уравновешивания спроса и предложения](media/nav_app_supply_planning_2_balancing.png "Обзор уравновешивания спроса и предложения")</span><span class="sxs-lookup"><span data-stu-id="55a70-112">![Overview of supply-demand balancing](media/nav_app_supply_planning_2_balancing.png "Overview of supply-demand balancing")</span></span>  

## <a name="see-also"></a><span data-ttu-id="55a70-113">См. также</span><span class="sxs-lookup"><span data-stu-id="55a70-113">See Also</span></span>  
 <span data-ttu-id="55a70-114">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="55a70-114">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="55a70-115">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="55a70-115">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="55a70-116">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="55a70-116">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
