---
title: Практическое руководство. Объединение поставок в один счет | Документация Майкрософт
description: Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: f6ce4c0c304fc8255789ec91fb3a00ba78170d6d
ms.sourcegitcommit: 6078bc9b2b571248d779722ce4125f250e7a3922
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/07/2020
ms.locfileid: "3666926"
---
# <a name="combine-shipments-on-a-single-invoice"></a><span data-ttu-id="ba58e-103">Объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="ba58e-103">Combine Shipments on a Single Invoice</span></span>
<span data-ttu-id="ba58e-104">Если требуется выставить счет сразу по нескольким отгрузкам, можно использовать функцию объединения поставок.</span><span class="sxs-lookup"><span data-stu-id="ba58e-104">If you want to invoice more than one shipment at a time, you can use the combined shipments feature.</span></span>  

<span data-ttu-id="ba58e-105">Чтобы создать объединенную расходную накладную, необходимо сначала учесть несколько расходных накладных для одного и того же клиента в одной и той же валюте.</span><span class="sxs-lookup"><span data-stu-id="ba58e-105">Before you can create a combined shipment, more than one sales shipment for the same customer in the same currency must be posted.</span></span> <span data-ttu-id="ba58e-106">Иными словами, следует создать два или более заказа на продажу и учесть их как отгруженные, но без выставления счета.</span><span class="sxs-lookup"><span data-stu-id="ba58e-106">In other words, you must have create two or more sales orders and post them as shipped, but not invoiced.</span></span> 

## <a name="to-manually-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="ba58e-107">Объединение поставок в один счет вручную</span><span class="sxs-lookup"><span data-stu-id="ba58e-107">To manually combine shipments on a single invoice</span></span>  
1. <span data-ttu-id="ba58e-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ba58e-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="ba58e-109">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-109">Choose the **New** action.</span></span> <span data-ttu-id="ba58e-110">Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="ba58e-110">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>
3. <span data-ttu-id="ba58e-111">В поле **Код клиента (покупателя)**</span><span class="sxs-lookup"><span data-stu-id="ba58e-111">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="ba58e-112">укажите клиента, который получит счет за отгруженные товары.</span><span class="sxs-lookup"><span data-stu-id="ba58e-112">field, enter the customer who will receive the invoice for the shipped items.</span></span>  
4. <span data-ttu-id="ba58e-113">На экспресс-вкладке **Строки** выберите действие **Получение строк отгрузки**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-113">On the **Lines** FastTab, choose the **Get Shipment Lines** action.</span></span>  
5. <span data-ttu-id="ba58e-114">Выберите строку расходной накладной, которую необходимо включить в этот счет.</span><span class="sxs-lookup"><span data-stu-id="ba58e-114">Select the shipment line that you want to include in the invoice:</span></span>  

    - <span data-ttu-id="ba58e-115">Чтобы вставить все строки, выделите все строки и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-115">To insert all lines, select all lines and choose the **OK** button.</span></span>  
    - <span data-ttu-id="ba58e-116">Чтобы вставить определенные строки, выделите эти строки и нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-116">To insert specific lines, select the lines and choose the **OK** button.</span></span> <span data-ttu-id="ba58e-117">Для выбора нескольких непоследовательных строк можно использовать клавишу Ctrl.</span><span class="sxs-lookup"><span data-stu-id="ba58e-117">You can use the Ctrl key to select multiple nonsequential lines.</span></span>  

    <span data-ttu-id="ba58e-118">Если строка расходной накладной была выделена ошибочно или необходимо начать сначала, то можно просто удалить строки счета и запустить функцию **Получить строки расх. накл.** повторно.</span><span class="sxs-lookup"><span data-stu-id="ba58e-118">If an incorrect shipment line was selected or you want to start over, you can simply delete the lines on the invoice and re-run the **Get Shipment Lines** function.</span></span>  
7. <span data-ttu-id="ba58e-119">Чтобы учесть счет, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-119">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-automatically-combine-shipments-on-a-single-invoice"></a><span data-ttu-id="ba58e-120">Автоматическое объединение поставок в один счет</span><span class="sxs-lookup"><span data-stu-id="ba58e-120">To automatically combine shipments on a single invoice</span></span>  
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="ba58e-121">выберет только заказы на продажу, в которых выбран вариант **Объединение поставок**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-121">will select only sales orders where **Combine Shipments** is chosen.</span></span> 

1. <span data-ttu-id="ba58e-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Объединение поставок**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ba58e-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Combine Shipments**, and then choose the related link.</span></span> <span data-ttu-id="ba58e-123">Откроется страница запроса пакетного задания.</span><span class="sxs-lookup"><span data-stu-id="ba58e-123">The batch job request page opens.</span></span>  
2. <span data-ttu-id="ba58e-124">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="ba58e-124">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="ba58e-125">Установите флажок **Учет счетов**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-125">Choose the **Post Invoices** check box.</span></span>  
4. <span data-ttu-id="ba58e-126">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-126">Choose the **OK** button.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="ba58e-127">В том случае, когда флажок **Учет счетов** в пакетном задании не установлен, потребуется выполнить учет счетов вручную.</span><span class="sxs-lookup"><span data-stu-id="ba58e-127">You will need to manually post the invoices if the **Post Invoices** check box was not selected on the batch job.</span></span>  

## <a name="to-remove-open-sales-orders-after-combined-shipment-posting"></a><span data-ttu-id="ba58e-128">Удаление открытых заказов на продажу после совмещенного учета расходных накладных</span><span class="sxs-lookup"><span data-stu-id="ba58e-128">To remove open sales orders after combined shipment posting</span></span> 
<span data-ttu-id="ba58e-129">Когда расходные накладные объединяются в счете и учитываются, для строк, включенных в счет, создается учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="ba58e-129">When shipments are combined on an invoice and posted, a posted sales invoice is created for the invoiced lines.</span></span> <span data-ttu-id="ba58e-130">Поле **Кол-во по выст. счетам** в исходном общем заказе на продажу или заказе на продажу обновляется на основе количества в выставленных счетах.</span><span class="sxs-lookup"><span data-stu-id="ba58e-130">The **Quantity Invoiced** field on the originating blanket sales order or sales order is updated based on the invoiced quantity.</span></span>  

<span data-ttu-id="ba58e-131">При таком способе выставления счетов по отгрузкам заказы, из которых были учтены эти отгрузки, продолжают существовать, даже если они были полностью отгружены и включены в счета.</span><span class="sxs-lookup"><span data-stu-id="ba58e-131">When you invoice shipments in this way, the orders from which the shipments were posted still exist, even if they have been fully shipped and invoiced.</span></span>   

1. <span data-ttu-id="ba58e-132">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удаление заказов на продажу, по которым выставлены счета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ba58e-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Sales Orders**, and then select the link.</span></span>  
2. <span data-ttu-id="ba58e-133">Укажите в поле фильтра **Номер**,</span><span class="sxs-lookup"><span data-stu-id="ba58e-133">Specify in the **No.**</span></span> <span data-ttu-id="ba58e-134">какие заказы на продажу следует удалить.</span><span class="sxs-lookup"><span data-stu-id="ba58e-134">filter field which sales orders to delete.</span></span>  
3. <span data-ttu-id="ba58e-135">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ba58e-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="ba58e-136">В качестве альтернативы удалите отдельные заказы на продажу вручную.</span><span class="sxs-lookup"><span data-stu-id="ba58e-136">Alternatively, delete individual sales orders manually.</span></span>  

<span data-ttu-id="ba58e-137">Повторите шаги с 1 по 3 для всех остальных затронутых документов, таких как общие заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="ba58e-137">Repeat steps 1 through 3 for any other affected documents, such as blanket sales orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="ba58e-138">См. также</span><span class="sxs-lookup"><span data-stu-id="ba58e-138">See Also</span></span>  
[<span data-ttu-id="ba58e-139">Продажи</span><span class="sxs-lookup"><span data-stu-id="ba58e-139">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="ba58e-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ba58e-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
