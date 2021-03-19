---
title: Сведения о проектировании — отслеживание товаров на складе | Документация Майкрософт
description: Обработка серийных номеров и номеров партий изначально является складской задачей, и, следовательно, все входящие и исходящие складские документы имеют стандартные функции назначения и выбора номеров трассировки товара. Однако поскольку система резервирования основывается на операциях книги товаров, документы складской операций, в которых регистрируются только складские операции, не поддерживаются полностью.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 6deebef5b1413ac04febe3333d21fe730e3bdea7
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5390953"
---
# <a name="design-details-item-tracking-in-the-warehouse"></a><span data-ttu-id="60ae7-104">Сведения о проектировании: трассировка товара на складе</span><span class="sxs-lookup"><span data-stu-id="60ae7-104">Design Details: Item Tracking in the Warehouse</span></span>
<span data-ttu-id="60ae7-105">Обработка серийных номеров и номеров партий изначально является складской задачей, и, следовательно, все входящие и исходящие складские документы имеют стандартные функции назначения и выбора номеров трассировки товара.</span><span class="sxs-lookup"><span data-stu-id="60ae7-105">Serial number and lot number handling is primarily a warehouse task and therefore all inbound and outbound warehouse documents have standard functionality for assigning and selecting item tracking numbers.</span></span>  

<span data-ttu-id="60ae7-106">Однако поскольку система резервирования основывается на операциях книги товаров, документы складской операций, в которых регистрируются только складские операции, не поддерживаются полностью.</span><span class="sxs-lookup"><span data-stu-id="60ae7-106">However, because the reservation system is based on item ledger entries, warehouse activity documents that register only warehouse entries are not fully supported.</span></span> <span data-ttu-id="60ae7-107">Поскольку резервирования и номера трассировки товара можно обработать только на уровне склада, а не на уровне ячейки и зоны, страницу **Строки трассировки товаров** невозможно открыть из документов складских операций.</span><span class="sxs-lookup"><span data-stu-id="60ae7-107">Because reservations and item tracking numbers can be handled only at the location level, not at the bin and zone level, the **Item Tracking Lines** page cannot be opened from warehouse activity documents.</span></span> <span data-ttu-id="60ae7-108">То же самое актуально в отношении страницы **Резервирование**.</span><span class="sxs-lookup"><span data-stu-id="60ae7-108">The same applies to the **Reservation** page.</span></span>  

<span data-ttu-id="60ae7-109">После добавления серийного номера или номера партии в товар в расположении склада его можно свободно перемещать и реклассифицировать в рамках склада с помощью независимой структуры трассировки товаров, не связанной с системой резервирования.</span><span class="sxs-lookup"><span data-stu-id="60ae7-109">After a serial or lot number has been added to an item at a warehouse location, it can be moved and reclassified freely within the warehouse by using an independent item tracking structure that is unrelated to the reservation system.</span></span> <span data-ttu-id="60ae7-110">Поля **Серийный номер** и **Номер партии** можно открыть непосредственно в строках складского документа.</span><span class="sxs-lookup"><span data-stu-id="60ae7-110">**Serial No.** and **Lot No.** fields are accessed directly on warehouse document lines.</span></span> <span data-ttu-id="60ae7-111">Если серийный номер или номер партии используется в исходящем учете, он синхронизируется с системой резервирования как часть корректировки обычной ячейки.</span><span class="sxs-lookup"><span data-stu-id="60ae7-111">When the serial or lot number later partakes in outbound posting, it is synchronized with the reservation system as a part of ordinary bin adjustment.</span></span> <span data-ttu-id="60ae7-112">Дополнительные сведения см. в разделе [Сведения о проектировании: интеграция с запасом](design-details-integration-with-inventory.md).</span><span class="sxs-lookup"><span data-stu-id="60ae7-112">For more information, see [Design Details: Integration with Inventory](design-details-integration-with-inventory.md).</span></span>  

<span data-ttu-id="60ae7-113">Однако система резервирования принимает во внимание складские операции при расчете наличия.</span><span class="sxs-lookup"><span data-stu-id="60ae7-113">However, the reservation system does take warehouse activities into consideration when it calculates availability.</span></span> <span data-ttu-id="60ae7-114">Например, товары, выделенные для подбора или зарегистрированные как подобранные, невозможно зарезервировать.</span><span class="sxs-lookup"><span data-stu-id="60ae7-114">For example, items that are allocated to picks, or registered as picked, cannot be reserved.</span></span> <span data-ttu-id="60ae7-115">Дополнительные сведения см. в разделе [Сведения о проектировании: наличие на складе](design-details-availability-in-the-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="60ae7-115">For more information, see [Design Details: Warehouse Availability](design-details-availability-in-the-warehouse.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="60ae7-116">См. также</span><span class="sxs-lookup"><span data-stu-id="60ae7-116">See Also</span></span>  
[<span data-ttu-id="60ae7-117">Сведения о проектировании: трассировка товара</span><span class="sxs-lookup"><span data-stu-id="60ae7-117">Design Details: Item Tracking</span></span>](design-details-item-tracking.md)  
[<span data-ttu-id="60ae7-118">Сведения о проектировании: интеграция с запасом</span><span class="sxs-lookup"><span data-stu-id="60ae7-118">Design Details: Integration with Inventory</span></span>](design-details-integration-with-inventory.md)  
[<span data-ttu-id="60ae7-119">Сведения о проектировании: наличие на складе</span><span class="sxs-lookup"><span data-stu-id="60ae7-119">Design Details: Warehouse Availability</span></span>](design-details-availability-in-the-warehouse.md)  
[<span data-ttu-id="60ae7-120">Сведения о проектировании: разработка трассировки товара</span><span class="sxs-lookup"><span data-stu-id="60ae7-120">Design Details: Item Tracking Design</span></span>](design-details-item-tracking-design.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]