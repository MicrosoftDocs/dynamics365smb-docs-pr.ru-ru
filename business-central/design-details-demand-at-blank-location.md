---
title: Сведения о проектировании — спрос и предложение | Документы Майкрософт
description: В этом разделе вводится концепция спроса — это общий термин, используемый для любого типа общего спроса, такого как заказ на продажу и требуемый компонент в производственном заказе.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, demand, supply, inventory, planning
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 23e941b3ab6fc8e2176268f38647630419453d23
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "933890"
---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="a15fa-103">Сведения о проектировании: спрос и поставка</span><span class="sxs-lookup"><span data-stu-id="a15fa-103">Design Details: Demand and Supply</span></span>
<span data-ttu-id="a15fa-104">Спрос — это общий термин, используемый для любого типа общего спроса, такого как заказ на продажу и требуемый компонент в производственном заказе.</span><span class="sxs-lookup"><span data-stu-id="a15fa-104">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="a15fa-105">Кроме того, в программе предусмотрены более технические типы спроса, например отрицательные остатки и возврат покупки.</span><span class="sxs-lookup"><span data-stu-id="a15fa-105">In addition, the program allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  
  
<span data-ttu-id="a15fa-106">Предложение — это общий термин, используемый для любого положительного или входящего количества, такого как запасы, покупки, сборка, производство или входящие перемещения.</span><span class="sxs-lookup"><span data-stu-id="a15fa-106">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="a15fa-107">Кроме того, возврат продажи также может представлять поставку.</span><span class="sxs-lookup"><span data-stu-id="a15fa-107">In addition, a sales return may also represent supply.</span></span>  
  
<span data-ttu-id="a15fa-108">Для сортировки многочисленных источников спроса и предложения система планирования организует их в два временных ряда, которые называются профилями склада.</span><span class="sxs-lookup"><span data-stu-id="a15fa-108">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="a15fa-109">В одном профиле содержатся события спроса, в другом — соответствующие события поставок.</span><span class="sxs-lookup"><span data-stu-id="a15fa-109">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="a15fa-110">Каждое событие представляет один объект сети заказов, такой как строка заказа на продажу, операция книги товаров или строка производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="a15fa-110">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  
  
<span data-ttu-id="a15fa-111">При загрузке профилей запасов разные наборы спроса и предложения уравновешиваются, чтобы получить в результате план поставки, соответствующий перечисленным целям.</span><span class="sxs-lookup"><span data-stu-id="a15fa-111">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  
  
<span data-ttu-id="a15fa-112">Параметры планирования и уровни запасов являются типами спроса и поставки соответственно, для которых выполняется интегрированная балансировка для пополнения товаров склада.</span><span class="sxs-lookup"><span data-stu-id="a15fa-112">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="a15fa-113">Дополнительные сведения см. в разделе [Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="a15fa-113">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="a15fa-114">См. также</span><span class="sxs-lookup"><span data-stu-id="a15fa-114">See Also</span></span>  
<span data-ttu-id="a15fa-115">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="a15fa-115">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="a15fa-116">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="a15fa-116">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="a15fa-117">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="a15fa-117">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)