---
title: Как включить подбор по методу FEFO | Документация Майкрософт
description: FEFO (First-Expired-First-Out) — это метод сортировки, который обеспечивает, чтобы наиболее старые товары (с наиболее ранними датами истечения срока) подбирались первыми.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 3a47c9daeeab036055a0644e1b389735f7440106
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5784071"
---
# <a name="enable-picking-items-by-fefo"></a><span data-ttu-id="0c1f8-103">Включение подбора товаров по методу FEFO</span><span class="sxs-lookup"><span data-stu-id="0c1f8-103">Enable Picking Items by FEFO</span></span>
<span data-ttu-id="0c1f8-104">FEFO (First-Expired-First-Out) — это метод сортировки, который обеспечивает, чтобы наиболее старые товары (с наиболее ранними датами истечения срока) подбирались первыми.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-104">First-Expired-First-Out (FEFO) is a sorting method that ensures that the oldest items, those with the earliest expiration dates, are picked first.</span></span>  

 <span data-ttu-id="0c1f8-105">Эта функция работает только при выполнении следующих условий:</span><span class="sxs-lookup"><span data-stu-id="0c1f8-105">This functionality only works when the following criteria are met:</span></span>  

-   <span data-ttu-id="0c1f8-106">Товар должен иметь серийный номер или номер партии.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-106">The item must have a serial/lot number.</span></span>  
-   <span data-ttu-id="0c1f8-107">В настройке кода трассировки товара необходимо выбрать поле **Трассировка по СН склада** или **Склад партии - трассировка**.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-107">On the item’s item tracking code setup, the **SN Warehouse Tracking** field or the **Lot Warehouse Tracking** field must be selected.</span></span>  
-   <span data-ttu-id="0c1f8-108">Товар необходимо учесть на складе со сроком годности.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-108">The item must be posted to inventory with an expiration date.</span></span>  
-   <span data-ttu-id="0c1f8-109">В местоположении переключатели **Требуется подбор**, **Выбрать по методу FEFO** и **Ячейка обязательна** должны быть включены.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-109">On the location, the **Require Pick**, **Pick According to FEFO**, and **Bin Mandatory** toggles must be turned on.</span></span>  

 <span data-ttu-id="0c1f8-110">Когда вся критерии будут соблюдены, пронумерованные по партии или серийному номеру товары, которые необходимо собрать, сортируются таким образом, что первыми следуют самые ранние элементы во всех выборках и движениях, за исключением товаров, для которых используется отслеживание по серийному номеру или номеру партии.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-110">When all the criteria are met, then serial/lot-numbered items to be picked are sorted with the oldest first in all picks and movements, except for items that use SN-specific or lot-specific tracking.</span></span>  

> [!NOTE]  
> <span data-ttu-id="0c1f8-111">Если товары с серийным номером или номером партии используют специальную трассировку, эти номера является первым и следующим за ним, остальные не указанные серийные номера и номера партии перечислены согласно методу FEFO.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-111">If some serial or lot-numbered items use specific tracking, then those are respected first and under them, the remaining, non-specific, serial/lot numbers are listed according to FEFO.</span></span>
<br /><br />
<span data-ttu-id="0c1f8-112">Если срок годности двух товаров совпадает, приложение выбирает товар с наименьшим серийным номером или номером партии.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-112">If two serial or lot-numbered items have the same expiration date, then the application selects the item with the lowest serial or lot number.</span></span>
<br /><br />
<span data-ttu-id="0c1f8-113">При подборе товаров с серийными номерами или номерами партий на складах, настроенных для расширенного подбора и размещения, по методу FEFO подбираются только количества в ячейках типа *Подбор*.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-113">When picking serial or lot-numbered items in locations set up for directed put-away and pick, only quantities on bins of type *Pick* are picked according to FEFO.</span></span>  
<br /><br />
<span data-ttu-id="0c1f8-114">Для включения перемещений согласно методу FEFO оставьте пустым поле **Из ячейки** на странице **Перемещение запасов** или на страницах **Журнал перемещений**.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-114">To enable movements according to FEFO, leave the **From Bin** field empty on the **Inventory Movement** page or the **Movement Worksheet** pages.</span></span>  
<br /><br />
<span data-ttu-id="0c1f8-115">Если поле **Строгий учет срока годности** выбрано на **Карточке кода трассировки товаров**, в подборку будут включены только товары, срок годности которых не истек, а строки сортируются по принципу FEFO.</span><span class="sxs-lookup"><span data-stu-id="0c1f8-115">If the **Strict Expiration Posting** field is selected on the **Item Tracking Code Card**, only items that are not expired will be included in the pick, and the lines are sorted according to the FEFO principle.</span></span>

## <a name="see-also"></a><span data-ttu-id="0c1f8-116">См. также</span><span class="sxs-lookup"><span data-stu-id="0c1f8-116">See Also</span></span>  
<span data-ttu-id="0c1f8-117">[Подбор товаров](warehouse-pick-items.md) </span><span class="sxs-lookup"><span data-stu-id="0c1f8-117">[Picking Items](warehouse-pick-items.md) </span></span>  
<span data-ttu-id="0c1f8-118">[Подбор товаров для складской отгрузки](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span><span class="sxs-lookup"><span data-stu-id="0c1f8-118">[Pick Items for Warehouse Shipment](warehouse-how-to-pick-items-for-warehouse-shipment.md) </span></span>  
<span data-ttu-id="0c1f8-119">[Подбор товаров с помощью подбора запасов](warehouse-how-to-pick-items-with-inventory-picks.md) </span><span class="sxs-lookup"><span data-stu-id="0c1f8-119">[Pick Items with Inventory Picks](warehouse-how-to-pick-items-with-inventory-picks.md) </span></span>  
[<span data-ttu-id="0c1f8-120">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="0c1f8-120">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
[<span data-ttu-id="0c1f8-121">Наличие</span><span class="sxs-lookup"><span data-stu-id="0c1f8-121">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="0c1f8-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0c1f8-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]