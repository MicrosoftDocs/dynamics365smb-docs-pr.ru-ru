---
title: Сведения о проектировании — наличие на складе | Документы Майкрософт
description: Система должна постоянно контролировать доступность товаров на складе, чтобы исходящие заказы могли эффективно обрабатываться и обеспечивать оптимальные поставки.
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
ms.openlocfilehash: 38218c497f7d3892b19d0b594ff3863004f69ac4
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "929940"
---
# <a name="design-details-availability-in-the-warehouse"></a><span data-ttu-id="8432f-103">Сведения о проектировании: наличие на складе</span><span class="sxs-lookup"><span data-stu-id="8432f-103">Design Details: Availability in the Warehouse</span></span>
<span data-ttu-id="8432f-104">Система должна постоянно контролировать доступность товаров на складе, чтобы исходящие заказы могли эффективно обрабатываться и обеспечивать оптимальные поставки.</span><span class="sxs-lookup"><span data-stu-id="8432f-104">The system must keep a constant control of item availability in the warehouse, so that outbound orders can flow efficiently and provide optimal deliveries.</span></span>  

 <span data-ttu-id="8432f-105">Наличие отличается в зависимости от распределений на уровне ячеек, если выполняются складские операции, такие как подбор и перемещение, и если система резервирования налагает ограничения, которые следует соблюдать.</span><span class="sxs-lookup"><span data-stu-id="8432f-105">Availability varies depending on allocations at the bin level when warehouse activities such as picks and movements occur and when the inventory reservation system imposes restrictions to comply with.</span></span> <span data-ttu-id="8432f-106">Довольно сложный алгоритм проверяет выполнение всех условий перед распределением количеств по подборам для расходов товаров.</span><span class="sxs-lookup"><span data-stu-id="8432f-106">A rather complex algorithm verifies that all conditions are met before allocating quantities to picks for outbound flows.</span></span>  

## <a name="bin-content-and-reservations"></a><span data-ttu-id="8432f-107">Содержимое ячейки и резервирования</span><span class="sxs-lookup"><span data-stu-id="8432f-107">Bin Content and Reservations</span></span>  
 <span data-ttu-id="8432f-108">В любой установке приложения управления складом количества товаров существуют и как складские операции в области приложения "Склад", и как операции книги товаров в области приложения "Товары".</span><span class="sxs-lookup"><span data-stu-id="8432f-108">In any installation of warehouse management, item quantities exist both as warehouse entries, in the Warehouse application area, and as item ledger entries, in the Inventory application area.</span></span> <span data-ttu-id="8432f-109">Эти два типа операций содержат разные сведения о том, где существуют товары и доступны ли они.</span><span class="sxs-lookup"><span data-stu-id="8432f-109">These two entry types contain different information about where items exist and whether they are available.</span></span> <span data-ttu-id="8432f-110">Складские операции определяют доступность товара по ячейкам и типу ячеек, что называется содержимым ячейки.</span><span class="sxs-lookup"><span data-stu-id="8432f-110">Warehouse entries define an item’s availability by bin and bin type, which is called bin content.</span></span> <span data-ttu-id="8432f-111">Операции книги товаров определяют наличие товара по его резервированиям в исходящих документах.</span><span class="sxs-lookup"><span data-stu-id="8432f-111">Item ledger entries define an item’s availability by its reservation to outbound documents.</span></span>  

 <span data-ttu-id="8432f-112">Специальная функция в алгоритме подбора существует для расчета количества, доступного для подбора, когда содержимое ячейки связывается с резервированиями.</span><span class="sxs-lookup"><span data-stu-id="8432f-112">Special functionality in the picking algorithm exists to calculate the quantity that is available to pick when bin content is coupled with reservations.</span></span>  

## <a name="quantity-available-to-pick"></a><span data-ttu-id="8432f-113">Количество, доступное для подбора</span><span class="sxs-lookup"><span data-stu-id="8432f-113">Quantity Available to Pick</span></span>  
 <span data-ttu-id="8432f-114">Например, если в алгоритме подбора не учитываются количества товаров, которые были зарезервированы для ожидающей отгрузки заказа на продажу, эти товары могут быть подобраны для другого заказа на продажу, который отгружается раньше, в результате чего не выполняется первый заказ.</span><span class="sxs-lookup"><span data-stu-id="8432f-114">If, for example, the picking algorithm does not consider item quantities that are reserved for a pending sales order shipment, then those items might be picked for another sales order that is shipped earlier, which prevents the first sales from being fulfilled.</span></span> <span data-ttu-id="8432f-115">Чтобы избежать этой ситуации, алгоритм подбора вычитает зарезервированные для других исходящих документов количества, количества в существующих документах отбора и количества, отобранные, но еще не отгруженные и не потребленные.</span><span class="sxs-lookup"><span data-stu-id="8432f-115">To avoid this situation, the picking algorithm subtracts quantities that are reserved for other outbound documents, quantities on existing pick documents, and quantities that are picked but not yet shipped or consumed.</span></span>  

 <span data-ttu-id="8432f-116">Результат отображается в поле **Доступное кол-во для подбора** на странице **Журнал подбора**, где это поле вычисляется динамически.</span><span class="sxs-lookup"><span data-stu-id="8432f-116">The result is displayed in the **Available Qty. to Pick** field on the **Pick Worksheet** page, where the field is calculated dynamically.</span></span> <span data-ttu-id="8432f-117">Стоимость также вычисляется, когда пользователи создают складские подборы непосредственно для исходящих документов.</span><span class="sxs-lookup"><span data-stu-id="8432f-117">The value is also calculated when users create warehouse picks directly for outbound documents.</span></span> <span data-ttu-id="8432f-118">К таким исходящим документам могут относиться заказы на продажу, производственные потребления или исходящие перемещения, в которых результат показан в связанных полях количества, например **Кол-во для обработки**.</span><span class="sxs-lookup"><span data-stu-id="8432f-118">Such outbound documents could be sales orders, production consumption, or outbound transfers, where the result is reflected in the related quantity fields, such as **Qty. to Handle**.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8432f-119">Что касается приоритета резервирований, количество для резервирования вычитается из количества, доступного для подбора.</span><span class="sxs-lookup"><span data-stu-id="8432f-119">Concerning the priority of reservations, the quantity to reserve is subtracted from the quantity available to pick.</span></span> <span data-ttu-id="8432f-120">Например, если количество, доступное в ячейках подбора, составляет 5 единиц, а 100 единиц находятся в ячейках размещения, то при попытке зарезервировать более 5 единиц для другого заказа отобразится сообщение об ошибке, поскольку должно быть доступно дополнительное количество в ячейках подбора.</span><span class="sxs-lookup"><span data-stu-id="8432f-120">For example, if the quantity available in pick bins is 5 units, but 100 units are in put-away bins, then when you try to reserve more than 5 units for another order, an error message is displayed because the additional quantity must be available in pick bins.</span></span>  

### <a name="calculating-the-quantity-available-to-pick"></a><span data-ttu-id="8432f-121">Расчет количества, доступного для подбора</span><span class="sxs-lookup"><span data-stu-id="8432f-121">Calculating the Quantity Available to Pick</span></span>  
 <span data-ttu-id="8432f-122">Доступное для подбора количество вычисляется следующим образом.</span><span class="sxs-lookup"><span data-stu-id="8432f-122">The quantity available to pick is calculated as follows:</span></span>  

 <span data-ttu-id="8432f-123">количество, доступное для подбора = количество в ячейках подбора - количество в подборах и перемещениях - (зарезервированное количество в ячейках подбора + зарезервированное количество в подборах и перемещениях)</span><span class="sxs-lookup"><span data-stu-id="8432f-123">quantity available to pick = quantity in pick bins - quantity on picks and movements – (reserved quantity in pick bins + reserved quantity on picks and movements)</span></span>  

 <span data-ttu-id="8432f-124">На следующей схеме показаны разные элементы вычислений.</span><span class="sxs-lookup"><span data-stu-id="8432f-124">The following diagram shows the different elements of the calculation.</span></span>  

 <span data-ttu-id="8432f-125">![Доступно для подбора, с перекрытием резервирования](media/design_details_warehouse_management_availability_2.png "Доступно для подбора, с перекрытием резервирования")</span><span class="sxs-lookup"><span data-stu-id="8432f-125">![Available to pick with reservation overlap](media/design_details_warehouse_management_availability_2.png "Available to pick with reservation overlap")</span></span>  

## <a name="quantity-available-to-reserve"></a><span data-ttu-id="8432f-126">Количество, доступное для резервирования</span><span class="sxs-lookup"><span data-stu-id="8432f-126">Quantity Available to Reserve</span></span>  
 <span data-ttu-id="8432f-127">Поскольку основные понятия содержимого ячейки и резервирования сосуществуют, количество товаров, доступных для резервирования, должно быть согласовано с распределениями в исходящих документах склада.</span><span class="sxs-lookup"><span data-stu-id="8432f-127">Because the concepts of bin content and reservation co-exist, the quantity of items that are available to reserve must be aligned with allocations to outbound warehouse documents.</span></span>  

 <span data-ttu-id="8432f-128">Должно быть возможно зарезервировать все товары в запасах за исключением тех, для которых уже начата исходящая обработка.</span><span class="sxs-lookup"><span data-stu-id="8432f-128">It should be possible to reserve all items in inventory, except those that have started outbound processing.</span></span> <span data-ttu-id="8432f-129">Соответственно, количество, доступное для резервирования, определяется как количество во всех документах и всех типах ячеек за исключением следующих исходящих количеств:</span><span class="sxs-lookup"><span data-stu-id="8432f-129">Accordingly, the quantity that is available to reserve is defined as the quantity on all documents and all bin types, except the following outbound quantities:</span></span>  

-   <span data-ttu-id="8432f-130">Количество в незарегистрированных документах подбора</span><span class="sxs-lookup"><span data-stu-id="8432f-130">Quantity on unregistered pick documents</span></span>  
-   <span data-ttu-id="8432f-131">Количество в ячейках отгрузки</span><span class="sxs-lookup"><span data-stu-id="8432f-131">Quantity in shipment bins</span></span>  
-   <span data-ttu-id="8432f-132">Количество во входящих производственных ячейках</span><span class="sxs-lookup"><span data-stu-id="8432f-132">Quantity in to-production bins</span></span>  
-   <span data-ttu-id="8432f-133">Количество в ячейках общего доступа</span><span class="sxs-lookup"><span data-stu-id="8432f-133">Quantity in open shop floor bins</span></span>  
-   <span data-ttu-id="8432f-134">Количества в ячейках сборки</span><span class="sxs-lookup"><span data-stu-id="8432f-134">Quantity in to-assembly bins</span></span>  
-   <span data-ttu-id="8432f-135">Количество в ячейках коррекции</span><span class="sxs-lookup"><span data-stu-id="8432f-135">Quantity in adjustment bins</span></span>  

 <span data-ttu-id="8432f-136">Результат отображается в поле **Общее доступное кол-во** на странице **Резервирование**.</span><span class="sxs-lookup"><span data-stu-id="8432f-136">The result is displayed in the **Total Available Quantity** field on the **Reservation** page.</span></span>  

 <span data-ttu-id="8432f-137">В строке резервирования количество, которое невозможно зарезервировать, поскольку оно распределено на склад, отображается в поле **Кол-во, распред. на складе** на странице **Reservation**.</span><span class="sxs-lookup"><span data-stu-id="8432f-137">On a reservation line, the quantity that cannot be reserved, because it is allocated in the warehouse, is displayed in the **Qty. Allocated in Warehouse** field on the **Reservation** page.</span></span>  

### <a name="calculating-the-quantity-available-to-reserve"></a><span data-ttu-id="8432f-138">Расчет количества, доступного для резервирования</span><span class="sxs-lookup"><span data-stu-id="8432f-138">Calculating the Quantity Available to Reserve</span></span>  
 <span data-ttu-id="8432f-139">Доступное для резервирования количество вычисляется следующим образом.</span><span class="sxs-lookup"><span data-stu-id="8432f-139">The quantity available to reserve is calculated as follows:</span></span>  

 <span data-ttu-id="8432f-140">количество, доступное для резервирования = общее количество в запасах - количество в подборах и перемещениях для документов-источников - зарезервированное количество - количество в исходящих ячейках</span><span class="sxs-lookup"><span data-stu-id="8432f-140">quantity available to reserve = total quantity in inventory - quantity on picks and movements for source documents - reserved quantity - quantity in outbound bins</span></span>  

 <span data-ttu-id="8432f-141">На следующей схеме показаны разные элементы вычислений.</span><span class="sxs-lookup"><span data-stu-id="8432f-141">The following diagram shows the different elements of the calculation.</span></span>  

 <span data-ttu-id="8432f-142">![Доступно для резервирования, на распределения склада](media/design_details_warehouse_management_availability_3.png "Доступно для резервирования, на распределения склада")</span><span class="sxs-lookup"><span data-stu-id="8432f-142">![Avaliable to reserve per warehouse allocation](media/design_details_warehouse_management_availability_3.png "Avaliable to reserve per warehouse allocation")</span></span>  

## <a name="see-also"></a><span data-ttu-id="8432f-143">См. также</span><span class="sxs-lookup"><span data-stu-id="8432f-143">See Also</span></span>  
 [<span data-ttu-id="8432f-144">Сведения о проектировании: управление складом</span><span class="sxs-lookup"><span data-stu-id="8432f-144">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)
