---
title: Расчет даты для покупок | Документация Майкрософт
description: Приложение автоматически вычисляет дату, когда следует заказать товар, чтобы иметь его на складе на определенную дату. Это дата, когда можно ожидать, что товары, заказанные на конкретную дату, будут доступны для подбора.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 7b39bcd593489e40d218cf29a3d288dd128cce04
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3192775"
---
# <a name="date-calculation-for-purchases"></a><span data-ttu-id="3b536-104">Расчет даты для покупок</span><span class="sxs-lookup"><span data-stu-id="3b536-104">Date Calculation for Purchases</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="3b536-105">автоматически вычисляет дату, когда следует заказать товар, чтобы иметь его на складе на определенную дату.</span><span class="sxs-lookup"><span data-stu-id="3b536-105">automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span></span> <span data-ttu-id="3b536-106">Это дата, когда можно ожидать, что товары, заказанные на конкретную дату, будут доступны для подбора.</span><span class="sxs-lookup"><span data-stu-id="3b536-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span></span>  

<span data-ttu-id="3b536-107">Если в заголовке заказа на покупку указана требуемая дата приемки, рассчитанная дата заказа является датой, на которую заказ должен быть размещен, чтобы товары вовремя поступили на склад.</span><span class="sxs-lookup"><span data-stu-id="3b536-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span></span> <span data-ttu-id="3b536-108">Затем дата, в которую товары будут в наличии для подбора, вычисляется и вводится в поле **Ожидаемая дата поставки**.</span><span class="sxs-lookup"><span data-stu-id="3b536-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span></span>  

<span data-ttu-id="3b536-109">Если требуемая дата приемки не указана, в качестве начальной точки расчета ожидаемой даты поставки товаров и даты, при наступлении которой товары станут доступны для подбора, используется дата заказа в строке документа.</span><span class="sxs-lookup"><span data-stu-id="3b536-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span></span>  

## <a name="calculating-with-a-requested-receipt-date"></a><span data-ttu-id="3b536-110">Вычисление с требуемой датой приемки</span><span class="sxs-lookup"><span data-stu-id="3b536-110">Calculating with a Requested Receipt Date</span></span>  
<span data-ttu-id="3b536-111">Если в строке заказа на покупку указана требуемая дата приемки, она будет использоваться как отправная точка для следующих расчетов.</span><span class="sxs-lookup"><span data-stu-id="3b536-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span></span>  

- <span data-ttu-id="3b536-112">требуемая дата приемки - расчет времени упреждения = дата заказа</span><span class="sxs-lookup"><span data-stu-id="3b536-112">requested receipt date - lead time calculation = order date</span></span>  
- <span data-ttu-id="3b536-113">требуемая дата приемки + входящие - время обработки склада + страховой запас времени упреждения = Ожидаемая дата приемки</span><span class="sxs-lookup"><span data-stu-id="3b536-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="3b536-114">Если в заголовок заказа на покупку введена требуемая дата приемки, то она будет скопирована в соответствующее поле всех строк заказа.</span><span class="sxs-lookup"><span data-stu-id="3b536-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span></span> <span data-ttu-id="3b536-115">Эту дату можно изменить или удалить в любой строке.</span><span class="sxs-lookup"><span data-stu-id="3b536-115">You can change this date on any of the lines, or you can remove the date on the line.</span></span>  

> [!Note]
> <span data-ttu-id="3b536-116">Если ваш процесс основан на обратном расчете, например, если вы используете запрошенную дату получения для получения даты заказа, мы рекомендуем использовать формулы дат с фиксированной длительностью, такие как "5D" для пяти дней или "1W" для одной недели.</span><span class="sxs-lookup"><span data-stu-id="3b536-116">If your process is based on backward calculation, for example, if you use the requested receipt date to get the order date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week.</span></span> <span data-ttu-id="3b536-117">Формулы дат без фиксированной длительности, такие как "CW" для текущей недели или CM для текущего месяца, могут привести к неправильным вычислениям даты.</span><span class="sxs-lookup"><span data-stu-id="3b536-117">Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations.</span></span> <span data-ttu-id="3b536-118">Дополнительные сведения о формулах дат см. в разделе [Работа с календарными датами и значениями времени](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="3b536-118">For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

## <a name="calculating-without-a-requested-delivery-date"></a><span data-ttu-id="3b536-119">Вычисление без требуемой даты доставки</span><span class="sxs-lookup"><span data-stu-id="3b536-119">Calculating without a Requested Delivery Date</span></span>  
<span data-ttu-id="3b536-120">При вводе строки заказа на покупку без требуемой даты доставки в поле **Дата заказа** в строке копируется дата из поля **Дата заказа** в заголовке заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="3b536-120">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span></span> <span data-ttu-id="3b536-121">Это может быть введенная вами дата или рабочая дата.</span><span class="sxs-lookup"><span data-stu-id="3b536-121">This is either the date that you entered or the work date.</span></span> <span data-ttu-id="3b536-122">Затем рассчитываются следующие даты для строки заказа на покупку с датой заказа в качестве начальной точки.</span><span class="sxs-lookup"><span data-stu-id="3b536-122">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span></span>  

- <span data-ttu-id="3b536-123">дата заказа + расчет времени обработки заказа = плановая дата приемки.</span><span class="sxs-lookup"><span data-stu-id="3b536-123">order date + lead time calculation = planned receipt date</span></span>  
- <span data-ttu-id="3b536-124">требуемая дата поставки + вход. время обработки склада + страховой запас времени = ожидаемая дата приемки</span><span class="sxs-lookup"><span data-stu-id="3b536-124">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="3b536-125">В случае изменения даты заказа в строке, например из-за того, что товары недоступны у поставщика до более поздней даты, соответствующие даты в строке пересчитываются автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b536-125">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span></span>  

<span data-ttu-id="3b536-126">В случае изменения даты заказа в заголовке документа, эта дата копируется в поле **Дата заказа** во всех строках, а все взаимосвязанные поля дат вычисляются заново.</span><span class="sxs-lookup"><span data-stu-id="3b536-126">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3b536-127">См. также</span><span class="sxs-lookup"><span data-stu-id="3b536-127">See Also</span></span>  
 <span data-ttu-id="3b536-128">[Расчет даты для продаж](sales-date-calculation-for-sales.md) </span><span class="sxs-lookup"><span data-stu-id="3b536-128">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span></span>  
 [<span data-ttu-id="3b536-129">Расчет сроков планирования заказов</span><span class="sxs-lookup"><span data-stu-id="3b536-129">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
 <span data-ttu-id="3b536-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="3b536-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
