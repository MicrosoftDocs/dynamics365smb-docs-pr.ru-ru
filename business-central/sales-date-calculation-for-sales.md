---
title: Расчет даты для продаж | Документация Майкрософт
description: Приложение автоматически вычисляет дату, когда следует заказать товар, чтобы иметь его на складе на определенную дату. Это дата, когда можно ожидать, что товары, заказанные на конкретную дату, будут доступны для подбора.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: a2a65f5025a8a79a7d0800d486bcac90fde23538
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3789054"
---
# <a name="date-calculation-for-sales"></a><span data-ttu-id="64280-104">Расчет даты для продаж</span><span class="sxs-lookup"><span data-stu-id="64280-104">Date Calculation for Sales</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="64280-105">автоматически вычисляет наиболее раннюю дату, на которую может быть произведена отгрузка товара, указанного в строке заказа за продажу.</span><span class="sxs-lookup"><span data-stu-id="64280-105">automatically calculates the earliest possible date that an item on a sales order line can be shipped.</span></span>

<span data-ttu-id="64280-106">Если клиент потребовал, чтобы поставка была произведена на конкретную дату, то дата, на которую товар должен быть в наличии для того, чтобы обеспечить выполнение этого требования, также будет вычислена.</span><span class="sxs-lookup"><span data-stu-id="64280-106">If the customer has requested a specific delivery date, then the date on which the items must be available to pick to meet that delivery date is calculated.</span></span>

<span data-ttu-id="64280-107">Если клиент не запрашивает, чтобы поставка была произведена на определенную дату, то будет автоматически рассчитана дата, на которую может быть произведена поставка товара, начиная с даты, когда товар будет в наличии.</span><span class="sxs-lookup"><span data-stu-id="64280-107">If the customer does not request a specific delivery date, then the date on which the items can be delivered is calculated, starting from the date on which the items are available for picking.</span></span>

## <a name="calculating-a-requested-delivery-date"></a><span data-ttu-id="64280-108">Вычисление требуемой даты доставки</span><span class="sxs-lookup"><span data-stu-id="64280-108">Calculating a Requested Delivery Date</span></span>
<span data-ttu-id="64280-109">Если в строке заказа продажи задана требуемая дата отгрузки, эта дата станет отправной точкой для следующих расчетов.</span><span class="sxs-lookup"><span data-stu-id="64280-109">If you specify a requested delivery date on the sales order line, that date becomes the starting point for the following calculations.</span></span>

- <span data-ttu-id="64280-110">требуемая дата доставки - время отгрузки = плановая дата поставки</span><span class="sxs-lookup"><span data-stu-id="64280-110">requested delivery date - shipping time = planned shipment date</span></span>
- <span data-ttu-id="64280-111">плановая дата поставки - исходящие - время обработки склада = дата поставки</span><span class="sxs-lookup"><span data-stu-id="64280-111">planned shipment date - outbound whse. handling time = shipment date</span></span>

<span data-ttu-id="64280-112">Если на дату отгрузки товар имеется в наличии, процесс продажи может быть продолжен.</span><span class="sxs-lookup"><span data-stu-id="64280-112">If the items are available to pick on the shipment date, then the sales process can continue.</span></span> <span data-ttu-id="64280-113">В противном случае отображается предупреждение об исчерпании запасов.</span><span class="sxs-lookup"><span data-stu-id="64280-113">Otherwise, a stock-out warning is displayed.</span></span>

> [!Note]
> <span data-ttu-id="64280-114">Если ваш процесс основан на обратном расчете, например, если вы используете запрошенную дату доставки для получения планируемой даты поставки, мы рекомендуем использовать формулы дат с фиксированной длительностью, такие как "5D" для пяти дней или "1W" для одной недели.</span><span class="sxs-lookup"><span data-stu-id="64280-114">If your process is based on backward calculation, for example, if you use the requested delivery date to get the planned shipment date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week.</span></span> <span data-ttu-id="64280-115">Формулы дат без фиксированной длительности, такие как "CW" для текущей недели или CM для текущего месяца, могут привести к неправильным вычислениям даты.</span><span class="sxs-lookup"><span data-stu-id="64280-115">Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations.</span></span> <span data-ttu-id="64280-116">Дополнительные сведения о формулах дат см. в разделе [Работа с календарными датами и значениями времени](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="64280-116">For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

## <a name="calculating-the-earliest-possible-delivery-date"></a><span data-ttu-id="64280-117">Расчет наиболее ранней возможной даты доставки</span><span class="sxs-lookup"><span data-stu-id="64280-117">Calculating the Earliest Possible Delivery Date</span></span>
<span data-ttu-id="64280-118">Если не указать требуемую дату доставки в строке заказа продажи, либо если соблюсти требуемая дата доставки невозможно, вычисляется самая ранняя дата, на которую доступны товары.</span><span class="sxs-lookup"><span data-stu-id="64280-118">If you do not specify a requested delivery date on the sales order line, or if the requested delivery date cannot be met, then the earliest date on which that the items are available is calculated.</span></span> <span data-ttu-id="64280-119">Затем эта дата вводится в поле Дата отгрузки в строке, и дата, в которую планируется отгрузки товаров, а также дата, в которую они будут доставлены клиенту, рассчитываются по следующим формулам.</span><span class="sxs-lookup"><span data-stu-id="64280-119">That date is then entered in the Shipment Date field on the line, and the date on which you plan to ship the items as well as the date on which they will be delivered to the customer are calculated using the following formulas.</span></span>

- <span data-ttu-id="64280-120">дата отгрузки + исходящие - время обработки склада = плановая дата отгрузки</span><span class="sxs-lookup"><span data-stu-id="64280-120">shipment date + outbound whse. handling time = planned shipment date</span></span>
- <span data-ttu-id="64280-121">плановая дата поставки + время отгрузки = плановая дата доставки</span><span class="sxs-lookup"><span data-stu-id="64280-121">planned shipment date + shipping time = planned delivery date</span></span>


## <a name="see-also"></a><span data-ttu-id="64280-122">См. также</span><span class="sxs-lookup"><span data-stu-id="64280-122">See Also</span></span>  
 <span data-ttu-id="64280-123">[Расчет даты для покупок](purchasing-date-calculation-for-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="64280-123">[Date Calculation for Purchases](purchasing-date-calculation-for-purchases.md) </span></span>  
 [<span data-ttu-id="64280-124">Расчет сроков планирования заказов</span><span class="sxs-lookup"><span data-stu-id="64280-124">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="64280-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="64280-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
