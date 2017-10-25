---
title: "Практическое руководство. Объединение поставок в один счет | Документы Майкрософт"
description: "Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: e6be50119da5c617ce6dbf603903266f9ced821e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="9ade8-103">Практическое руководство. Объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="9ade8-103">How to: Combine Shipments on a Single Invoice</span></span>
<span data-ttu-id="9ade8-104">Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок.</span><span class="sxs-lookup"><span data-stu-id="9ade8-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span></span>  

 <span data-ttu-id="9ade8-105">Чтобы создать объединенную расходную накладную, необходимо сначала учесть несколько расходных накладных для одного и того же клиента в одной и той же валюте.</span><span class="sxs-lookup"><span data-stu-id="9ade8-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span></span> <span data-ttu-id="9ade8-106">Иными словами, следует заполнить два или более заказа на продажу и учесть их как отгруженные, но без выставления счета.</span><span class="sxs-lookup"><span data-stu-id="9ade8-106">In other words, you must have filled in two or more sales orders and posted them as shipped, but not invoiced.</span></span> <span data-ttu-id="9ade8-107">Чтобы объединить расходные накладные возврата, необходимо флажок в поле **Объединение поставок** на экспресс-вкладке **Отгрузка** карточки **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-107">To combine shipments, the **Combine Shipments** check box must be selected on the **Shipping** FastTab of the **Customer** card.</span></span>  

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="9ade8-108">Объединение поставок в один счет вручную</span><span class="sxs-lookup"><span data-stu-id="9ade8-108">To manually combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="9ade8-109">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета продажи**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="9ade8-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9ade8-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-110">Choose the **New** action.</span></span> <span data-ttu-id="9ade8-111">Дополнительные сведения см. в разделе [Практическое руководство. Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="9ade8-111">For more information, see [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span>
3. <span data-ttu-id="9ade8-112">В поле **Код клиента (покупателя)**</span><span class="sxs-lookup"><span data-stu-id="9ade8-112">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="9ade8-113">укажите клиента, который получит счет за отгруженные товары.</span><span class="sxs-lookup"><span data-stu-id="9ade8-113">field, enter the customer who will receive the invoice for the shipped items.</span></span>  
4. <span data-ttu-id="9ade8-114">На экспресс-вкладке **Строки** выберите действие **Получение строк отгрузки**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-114">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span></span>  
5. <span data-ttu-id="9ade8-115">Выберите строку расходной накладной, которую необходимо включить в этот счет.</span><span class="sxs-lookup"><span data-stu-id="9ade8-115">Select the shipment line that you want to include in the invoice:</span></span>  

    - <span data-ttu-id="9ade8-116">Чтобы вставить все строки, выделите все строки и нажмите кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-116">To insert all lines, select all lines and choose the **OK** button.</span></span>  
    - <span data-ttu-id="9ade8-117">Чтобы вставить определенные строки, выделите эти строки и нажмите кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-117">To insert specific lines, select the lines and choose the **OK** button.</span></span> <span data-ttu-id="9ade8-118">Для выбора нескольких непоследовательных строк можно использовать клавишу Ctrl.</span><span class="sxs-lookup"><span data-stu-id="9ade8-118">You can use the Ctrl key to select multiple nonsequential lines.</span></span>  

    <span data-ttu-id="9ade8-119">Если строка расходной накладной была выделена ошибочно или необходимо начать сначала, то можно просто удалить строки счета и запустить функцию **Получить строки расх. накл.** повторно.</span><span class="sxs-lookup"><span data-stu-id="9ade8-119">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span></span>  
7. <span data-ttu-id="9ade8-120">Чтобы учесть счет, выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-120">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="9ade8-121">Автоматическое объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="9ade8-121">To automatically combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="9ade8-122">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Объединение поставок**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="9ade8-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Combine Shipments**, and then choose the related link.</span></span> <span data-ttu-id="9ade8-123">Откроется окно запроса пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="9ade8-123">The batch job request window opens.</span></span>  
2. <span data-ttu-id="9ade8-124">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="9ade8-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="9ade8-125">Установите флажок **Учет счетов**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-125">Select the **Post Invoices** check box.</span></span>  
4.  <span data-ttu-id="9ade8-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-126">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9ade8-127">В том случае, когда флажок **Учет счетов** в пакетном задании не установлен, потребуется выполнить учет счетов вручную.</span><span class="sxs-lookup"><span data-stu-id="9ade8-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span></span>  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a><span data-ttu-id="9ade8-128">Удаление открытых заказов на продажу после совмещенного учета расходных накладных</span><span class="sxs-lookup"><span data-stu-id="9ade8-128">To remove open sales orders after combined shipment posting</span></span> 
<span data-ttu-id="9ade8-129">Когда расходные накладные объединяются в счете и учитываются, для строк, включенных в счет, создается учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="9ade8-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span></span> <span data-ttu-id="9ade8-130">Поле **Кол-во по выст. счетам** в исходном общем заказе на продажу или заказе на продажу обновляется на основе количества в выставленных счетах.</span><span class="sxs-lookup"><span data-stu-id="9ade8-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span></span>  

<span data-ttu-id="9ade8-131">При таком способе выставления счетов по отгрузкам заказы, из которых были учтены эти отгрузки, продолжают существовать, даже если они были полностью отгружены и включены в счета.</span><span class="sxs-lookup"><span data-stu-id="9ade8-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span></span>   

1. <span data-ttu-id="9ade8-132">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Удаление заказов на продажу, по которым выставлены счета**, затем выберите ссылку.</span><span class="sxs-lookup"><span data-stu-id="9ade8-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span></span>  
2. <span data-ttu-id="9ade8-133">Укажите в поле фильтра **Номер**,</span><span class="sxs-lookup"><span data-stu-id="9ade8-133">Specify in the **No.**</span></span> <span data-ttu-id="9ade8-134">какие заказы на продажу следует удалить.</span><span class="sxs-lookup"><span data-stu-id="9ade8-134">filter field which sales orders to delete.</span></span>  
3. <span data-ttu-id="9ade8-135">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9ade8-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="9ade8-136">В качестве альтернативы удалите отдельные заказы на продажу вручную.</span><span class="sxs-lookup"><span data-stu-id="9ade8-136">Alternatively, delete individual sales orders manually.</span></span>  

<span data-ttu-id="9ade8-137">Повторите шаги с 1 по 3 для всех остальных затронутых документов, таких как общие заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="9ade8-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="9ade8-138">См. также</span><span class="sxs-lookup"><span data-stu-id="9ade8-138">See Also</span></span>  
[<span data-ttu-id="9ade8-139">Продажи</span><span class="sxs-lookup"><span data-stu-id="9ade8-139">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="9ade8-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9ade8-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

