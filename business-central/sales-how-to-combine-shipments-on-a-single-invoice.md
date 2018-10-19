---
title: "Практическое руководство. Объединение поставок в один счет | Документы Майкрософт"
description: "Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 429002d1eb6bfa487e5a21e54964ce33de175441
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="combine-shipments-on-a-single-invoice"></a><span data-ttu-id="fa24d-103">Объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="fa24d-103">Combine Shipments on a Single Invoice</span></span>
<span data-ttu-id="fa24d-104">Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок.</span><span class="sxs-lookup"><span data-stu-id="fa24d-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span></span>  

 <span data-ttu-id="fa24d-105">Чтобы создать объединенную расходную накладную, необходимо сначала учесть несколько расходных накладных для одного и того же клиента в одной и той же валюте.</span><span class="sxs-lookup"><span data-stu-id="fa24d-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span></span> <span data-ttu-id="fa24d-106">Иными словами, следует заполнить два или более заказа на продажу и учесть их как отгруженные, но без выставления счета.</span><span class="sxs-lookup"><span data-stu-id="fa24d-106">In other words, you must have filled in two or more sales orders and posted them as shipped, but not invoiced.</span></span> <span data-ttu-id="fa24d-107">Чтобы объединить расходные накладные возврата, необходимо флажок в поле **Объединение поставок** на экспресс-вкладке **Отгрузка** карточки **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-107">To combine shipments, the **Combine Shipments** check box must be selected on the **Shipping** FastTab of the **Customer** card.</span></span>  

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="fa24d-108">Объединение поставок в один счет вручную</span><span class="sxs-lookup"><span data-stu-id="fa24d-108">To manually combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="fa24d-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fa24d-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="fa24d-110">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-110">Choose the **New** action.</span></span> <span data-ttu-id="fa24d-111">Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="fa24d-111">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>
3. <span data-ttu-id="fa24d-112">В поле **Код клиента (покупателя)**</span><span class="sxs-lookup"><span data-stu-id="fa24d-112">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="fa24d-113">укажите клиента, который получит счет за отгруженные товары.</span><span class="sxs-lookup"><span data-stu-id="fa24d-113">field, enter the customer who will receive the invoice for the shipped items.</span></span>  
4. <span data-ttu-id="fa24d-114">На экспресс-вкладке **Строки** выберите действие **Получение строк отгрузки**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-114">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span></span>  
5. <span data-ttu-id="fa24d-115">Выберите строку расходной накладной, которую необходимо включить в этот счет.</span><span class="sxs-lookup"><span data-stu-id="fa24d-115">Select the shipment line that you want to include in the invoice:</span></span>  

    - <span data-ttu-id="fa24d-116">Чтобы вставить все строки, выделите все строки и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-116">To insert all lines, select all lines and choose the **OK** button.</span></span>  
    - <span data-ttu-id="fa24d-117">Чтобы вставить определенные строки, выделите эти строки и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-117">To insert specific lines, select the lines and choose the **OK** button.</span></span> <span data-ttu-id="fa24d-118">Для выбора нескольких непоследовательных строк можно использовать клавишу Ctrl.</span><span class="sxs-lookup"><span data-stu-id="fa24d-118">You can use the Ctrl key to select multiple nonsequential lines.</span></span>  

    <span data-ttu-id="fa24d-119">Если строка расходной накладной была выделена ошибочно или необходимо начать сначала, то можно просто удалить строки счета и запустить функцию **Получить строки расх. накл.** повторно.</span><span class="sxs-lookup"><span data-stu-id="fa24d-119">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span></span>  
7. <span data-ttu-id="fa24d-120">Чтобы учесть счет, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-120">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="fa24d-121">Автоматическое объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="fa24d-121">To automatically combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="fa24d-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Объединение поставок**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fa24d-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Combine Shipments**, and then choose the related link.</span></span> <span data-ttu-id="fa24d-123">Откроется окно запроса пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="fa24d-123">The batch job request window opens.</span></span>  
2. <span data-ttu-id="fa24d-124">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="fa24d-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="fa24d-125">Установите флажок **Учет счетов**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-125">Select the **Post Invoices** check box.</span></span>  
4.  <span data-ttu-id="fa24d-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-126">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fa24d-127">В том случае, когда флажок **Учет счетов** в пакетном задании не установлен, потребуется выполнить учет счетов вручную.</span><span class="sxs-lookup"><span data-stu-id="fa24d-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span></span>  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a><span data-ttu-id="fa24d-128">Удаление открытых заказов на продажу после совмещенного учета расходных накладных</span><span class="sxs-lookup"><span data-stu-id="fa24d-128">To remove open sales orders after combined shipment posting</span></span> 
<span data-ttu-id="fa24d-129">Когда расходные накладные объединяются в счете и учитываются, для строк, включенных в счет, создается учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="fa24d-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span></span> <span data-ttu-id="fa24d-130">Поле **Кол-во по выст. счетам** в исходном общем заказе на продажу или заказе на продажу обновляется на основе количества в выставленных счетах.</span><span class="sxs-lookup"><span data-stu-id="fa24d-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span></span>  

<span data-ttu-id="fa24d-131">При таком способе выставления счетов по отгрузкам заказы, из которых были учтены эти отгрузки, продолжают существовать, даже если они были полностью отгружены и включены в счета.</span><span class="sxs-lookup"><span data-stu-id="fa24d-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span></span>   

1. <span data-ttu-id="fa24d-132">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fa24d-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span></span>  
2. <span data-ttu-id="fa24d-133">Укажите в поле фильтра **Номер**,</span><span class="sxs-lookup"><span data-stu-id="fa24d-133">Specify in the **No.**</span></span> <span data-ttu-id="fa24d-134">какие заказы на продажу следует удалить.</span><span class="sxs-lookup"><span data-stu-id="fa24d-134">filter field which sales orders to delete.</span></span>  
3. <span data-ttu-id="fa24d-135">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fa24d-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="fa24d-136">В качестве альтернативы удалите отдельные заказы на продажу вручную.</span><span class="sxs-lookup"><span data-stu-id="fa24d-136">Alternatively, delete individual sales orders manually.</span></span>  

<span data-ttu-id="fa24d-137">Повторите шаги с 1 по 3 для всех остальных затронутых документов, таких как общие заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="fa24d-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="fa24d-138">См. также</span><span class="sxs-lookup"><span data-stu-id="fa24d-138">See Also</span></span>  
[<span data-ttu-id="fa24d-139">Продажи</span><span class="sxs-lookup"><span data-stu-id="fa24d-139">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="fa24d-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fa24d-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

