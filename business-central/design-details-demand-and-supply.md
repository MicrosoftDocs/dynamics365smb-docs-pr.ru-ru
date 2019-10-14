---
title: Сведения о проектировании — спрос и предложение | Документация Майкрософт
description: Спрос — это общий термин, используемый для любого типа общего спроса, такого как заказ на продажу и требуемый компонент в производственном заказе. Кроме того, в приложении предусмотрены более специализированные типы спроса, например отрицательные остатки и возвраты покупок.
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
ms.openlocfilehash: 8ef7211aa812b1faf784ecf36f1873a6e2dcc6fc
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2303633"
---
# <a name="design-details-demand-and-supply"></a><span data-ttu-id="f3c90-104">Сведения о проектировании: спрос и поставка</span><span class="sxs-lookup"><span data-stu-id="f3c90-104">Design Details: Demand and Supply</span></span>
<span data-ttu-id="f3c90-105">Спрос — это общий термин, используемый для любого типа общего спроса, такого как заказ на продажу и требуемый компонент в производственном заказе.</span><span class="sxs-lookup"><span data-stu-id="f3c90-105">Demand is the common term used for any kind of gross demand, such as a sales order and component need from a production order.</span></span> <span data-ttu-id="f3c90-106">Кроме того, в приложении предусмотрены более специализированные типы спроса, например отрицательные остатки и возвраты покупок.</span><span class="sxs-lookup"><span data-stu-id="f3c90-106">In addition, application allows more technical types of demand, such as negative inventory and purchase returns.</span></span>  

 <span data-ttu-id="f3c90-107">Предложение — это общий термин, используемый для любого положительного или входящего количества, такого как запасы, покупки, сборка, производство или входящие перемещения.</span><span class="sxs-lookup"><span data-stu-id="f3c90-107">Supply is the common term used for any kind of positive or inbound quantity, such as inventory, purchases, assembly, production, or inbound transfers.</span></span> <span data-ttu-id="f3c90-108">Кроме того, возврат продажи также может представлять поставку.</span><span class="sxs-lookup"><span data-stu-id="f3c90-108">In addition, a sales return may also represent supply.</span></span>  

 <span data-ttu-id="f3c90-109">Для сортировки многочисленных источников спроса и предложения система планирования организует их в два временных ряда, которые называются профилями склада.</span><span class="sxs-lookup"><span data-stu-id="f3c90-109">To sort out the many sources of demand and supply, the planning system organizes them on two time lines called inventory profiles.</span></span> <span data-ttu-id="f3c90-110">В одном профиле содержатся события спроса, в другом — соответствующие события поставок.</span><span class="sxs-lookup"><span data-stu-id="f3c90-110">One profile holds demand events, and the other holds the corresponding supply events.</span></span> <span data-ttu-id="f3c90-111">Каждое событие представляет один объект сети заказов, такой как строка заказа на продажу, операция книги товаров или строка производственного заказа.</span><span class="sxs-lookup"><span data-stu-id="f3c90-111">Each event represents one order network entity, such as a sales order line, an item ledger entry, or a production order line.</span></span>  

 <span data-ttu-id="f3c90-112">При загрузке профилей запасов разные наборы спроса и предложения уравновешиваются, чтобы получить в результате план поставки, соответствующий перечисленным целям.</span><span class="sxs-lookup"><span data-stu-id="f3c90-112">When inventory profiles are loaded, the different demand-supply sets are balanced to output a supply plan that fulfills the listed goals.</span></span>  

 <span data-ttu-id="f3c90-113">Параметры планирования и уровни запасов являются типами спроса и поставки соответственно, для которых выполняется интегрированная балансировка для пополнения товаров склада.</span><span class="sxs-lookup"><span data-stu-id="f3c90-113">Planning parameters and inventory levels are other types of demand and supply respectively, which undergo integrated balancing to replenish stock items.</span></span> <span data-ttu-id="f3c90-114">Дополнительные сведения см. в разделе [Сведения о проектировании: обработка политик дозаказа](design-details-handling-reordering-policies.md).</span><span class="sxs-lookup"><span data-stu-id="f3c90-114">For more information, see [Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="f3c90-115">См. также</span><span class="sxs-lookup"><span data-stu-id="f3c90-115">See Also</span></span>  
 <span data-ttu-id="f3c90-116">[Сведения о проектировании: балансировка спроса и поставки](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="f3c90-116">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
 <span data-ttu-id="f3c90-117">[Сведения о проектировании: основные понятия системы планирования](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="f3c90-117">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
 [<span data-ttu-id="f3c90-118">Сведения о проектировании: планирование поставок</span><span class="sxs-lookup"><span data-stu-id="f3c90-118">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)
