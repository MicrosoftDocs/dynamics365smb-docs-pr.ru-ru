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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 22153df1e56d274256b53d426e2dff30cad3e4bc
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758596"
---
# <a name="date-calculation-for-purchases"></a><span data-ttu-id="1a705-104">Расчет даты для покупок</span><span class="sxs-lookup"><span data-stu-id="1a705-104">Date Calculation for Purchases</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="1a705-105">автоматически вычисляет дату, когда следует заказать товар, чтобы иметь его на складе на определенную дату.</span><span class="sxs-lookup"><span data-stu-id="1a705-105">automatically calculates the date on which you must order an item to have it in inventory on a certain date.</span></span> <span data-ttu-id="1a705-106">Это дата, когда можно ожидать, что товары, заказанные на конкретную дату, будут доступны для подбора.</span><span class="sxs-lookup"><span data-stu-id="1a705-106">This is the date on which you can expect items ordered on a particular date to be available for picking.</span></span>  

<span data-ttu-id="1a705-107">Если в заголовке заказа на покупку указана требуемая дата приемки, рассчитанная дата заказа является датой, на которую заказ должен быть размещен, чтобы товары вовремя поступили на склад.</span><span class="sxs-lookup"><span data-stu-id="1a705-107">If you specify a requested receipt date on a purchase order header, then the calculated order date is the date on which the order must be placed to receive the items on the date that you requested.</span></span> <span data-ttu-id="1a705-108">Затем дата, в которую товары будут в наличии для подбора, вычисляется и вводится в поле **Ожидаемая дата поставки**.</span><span class="sxs-lookup"><span data-stu-id="1a705-108">Then, the date on which the items are available for picking is calculated and entered in the **Expected Receipt Date** field.</span></span>  

<span data-ttu-id="1a705-109">Если требуемая дата приемки не указана, в качестве начальной точки расчета ожидаемой даты поставки товаров и даты, при наступлении которой товары станут доступны для подбора, используется дата заказа в строке документа.</span><span class="sxs-lookup"><span data-stu-id="1a705-109">If you do not specify a requested receipt date, then the order date on the line is used as the starting point for calculating the date on which you can expect to receive the items and the date on which the items are available for picking.</span></span>  

## <a name="calculating-with-a-requested-receipt-date"></a><span data-ttu-id="1a705-110">Вычисление с требуемой датой приемки</span><span class="sxs-lookup"><span data-stu-id="1a705-110">Calculating with a requested receipt date</span></span>

<span data-ttu-id="1a705-111">Если в строке заказа на покупку указана требуемая дата приемки, она будет использоваться как отправная точка для следующих расчетов.</span><span class="sxs-lookup"><span data-stu-id="1a705-111">If there is a requested receipt date on the purchase order line, then that date is used as the starting point for the following calculations.</span></span>  

- <span data-ttu-id="1a705-112">требуемая дата приемки - расчет времени упреждения = дата заказа</span><span class="sxs-lookup"><span data-stu-id="1a705-112">requested receipt date - lead time calculation = order date</span></span>  
- <span data-ttu-id="1a705-113">требуемая дата приемки + входящие - время обработки склада + страховой запас времени упреждения = Ожидаемая дата приемки</span><span class="sxs-lookup"><span data-stu-id="1a705-113">requested receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="1a705-114">Если в заголовок заказа на покупку введена требуемая дата приемки, то она будет скопирована в соответствующее поле всех строк заказа.</span><span class="sxs-lookup"><span data-stu-id="1a705-114">If you entered a requested receipt date on the purchase order header, then that date is copied to the corresponding field on all the lines.</span></span> <span data-ttu-id="1a705-115">Эту дату можно изменить или удалить в любой строке.</span><span class="sxs-lookup"><span data-stu-id="1a705-115">You can change this date on any of the lines, or you can remove the date on the line.</span></span>  

> [!NOTE]
> <span data-ttu-id="1a705-116">Если ваш процесс основан на обратном расчете, например, если вы используете запрошенную дату получения для получения даты заказа, мы рекомендуем использовать формулы дат с фиксированной длительностью, такие как "5D" для пяти дней или "1W" для одной недели.</span><span class="sxs-lookup"><span data-stu-id="1a705-116">If your process is based on backward calculation, for example, if you use the requested receipt date to get the order date, we recommend that you use date formulas that have fixed durations, such as "5D" for five days or "1W" for one week.</span></span> <span data-ttu-id="1a705-117">Формулы дат без фиксированной длительности, такие как "CW" для текущей недели или CM для текущего месяца, могут привести к неправильным вычислениям даты.</span><span class="sxs-lookup"><span data-stu-id="1a705-117">Date formulas without fixed durations, such as "CW" for current week or CM for current month, can result in incorrect date calculations.</span></span> <span data-ttu-id="1a705-118">Дополнительные сведения о формулах дат см. в разделе [Работа с календарными датами и значениями времени](ui-enter-date-ranges.md).</span><span class="sxs-lookup"><span data-stu-id="1a705-118">For more information about date formulas, see [Working with Calendar Dates and Times](ui-enter-date-ranges.md).</span></span>

## <a name="calculating-without-a-requested-delivery-date"></a><span data-ttu-id="1a705-119">Вычисление без требуемой даты доставки</span><span class="sxs-lookup"><span data-stu-id="1a705-119">Calculating without a requested delivery date</span></span>

<span data-ttu-id="1a705-120">При вводе строки заказа на покупку без требуемой даты доставки в поле **Дата заказа** в строке копируется дата из поля **Дата заказа** в заголовке заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="1a705-120">If you enter a purchase order line without a requested delivery date, then the **Order Date** field on the line is filled with the date in the **Order Date** field on the purchase order header.</span></span> <span data-ttu-id="1a705-121">Это может быть введенная вами дата или рабочая дата.</span><span class="sxs-lookup"><span data-stu-id="1a705-121">This is either the date that you entered or the work date.</span></span> <span data-ttu-id="1a705-122">Затем рассчитываются следующие даты для строки заказа на покупку с датой заказа в качестве начальной точки.</span><span class="sxs-lookup"><span data-stu-id="1a705-122">The following dates are then calculated for the purchase order line, with the order date as the starting point.</span></span>  

- <span data-ttu-id="1a705-123">дата заказа + расчет времени обработки заказа = плановая дата приемки.</span><span class="sxs-lookup"><span data-stu-id="1a705-123">order date + lead time calculation = planned receipt date</span></span>  
- <span data-ttu-id="1a705-124">требуемая дата поставки + вход. время обработки склада + страховой запас времени = ожидаемая дата приемки</span><span class="sxs-lookup"><span data-stu-id="1a705-124">planned receipt date + inbound whse. handling time + safety lead time = expected receipt date</span></span>  

<span data-ttu-id="1a705-125">В случае изменения даты заказа в строке, например из-за того, что товары недоступны у поставщика до более поздней даты, соответствующие даты в строке пересчитываются автоматически.</span><span class="sxs-lookup"><span data-stu-id="1a705-125">If you change the order date on the line, such as when items are not available at your vendor until a later date, then the relevant dates on the line are automatically recalculated.</span></span>  

<span data-ttu-id="1a705-126">В случае изменения даты заказа в заголовке документа, эта дата копируется в поле **Дата заказа** во всех строках, а все взаимосвязанные поля дат вычисляются заново.</span><span class="sxs-lookup"><span data-stu-id="1a705-126">If you change the order date on the header, then that date is copied to the **Order Date** field on all the lines, and all the related date fields are then recalculated.</span></span>  

## <a name="default-values-for-lead-time-calculation"></a><span data-ttu-id="1a705-127">Значения по умолчанию для расчета времени подготовки</span><span class="sxs-lookup"><span data-stu-id="1a705-127">Default values for lead time calculation</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="1a705-128">использует значение из поля **Рассчитанное время подготовки заказа** в строке заказа на покупку для расчета заказа и ожидаемых дат поступления.</span><span class="sxs-lookup"><span data-stu-id="1a705-128">uses the value from the **Lead Time Calculation** field on the purchase order line to calculate the order and the expected receipt dates.</span></span>  

<span data-ttu-id="1a705-129">Вы можете вручную указать значение в строке или позволить программе использовать значения, которые определены в карточке поставщика, карточке товара, карточке единицы складского учета или в каталоге поставщиков товаров.</span><span class="sxs-lookup"><span data-stu-id="1a705-129">You can manually specify the value on the line or let the program use values that are defined on the vendor card, item card, stockkeeping unit card, or the item vendor catalog.</span></span>
<span data-ttu-id="1a705-130">Однако значение времени выполнения заказа в карточке поставщика используется только в том случае, если время выполнения заказа не указано в карточке товара, карточке единицы складского учета или в каталоге поставщиков номенклатуры для номенклатуры.</span><span class="sxs-lookup"><span data-stu-id="1a705-130">However, the lead time value on the vendor card is used only if a lead time is not specified on the item card, stockkeeping unit card, or the item vendor catalog for the item.</span></span> <span data-ttu-id="1a705-131">Это также возрастающий порядок приоритета для этих значений.</span><span class="sxs-lookup"><span data-stu-id="1a705-131">This is also the escalating order of priority for these values.</span></span> <span data-ttu-id="1a705-132">Если все они предоставлены, время подготовки заказа из карточки поставщика имеет самый низкий приоритет, а время подготовки заказа из каталога поставщиков товаров имеет самый высокий приоритет.</span><span class="sxs-lookup"><span data-stu-id="1a705-132">If they are all provided, the lead time from the vendor card has the lowest priority, and the lead time from the item vendor catalog has the highest priority.</span></span>  

## <a name="see-also"></a><span data-ttu-id="1a705-133">См. также</span><span class="sxs-lookup"><span data-stu-id="1a705-133">See Also</span></span>

<span data-ttu-id="1a705-134">[Расчет даты для продаж](sales-date-calculation-for-sales.md) </span><span class="sxs-lookup"><span data-stu-id="1a705-134">[Date Calculation for Sales](sales-date-calculation-for-sales.md) </span></span>  
[<span data-ttu-id="1a705-135">Расчет сроков планирования заказов</span><span class="sxs-lookup"><span data-stu-id="1a705-135">Calculate Order Promising Dates</span></span>](sales-how-to-calculate-order-promising-dates.md)  
<span data-ttu-id="1a705-136">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1a705-136">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  
