---
title: Как объединить приходные накладные | Документы Майкрософт
description: Если необходимо выставить счет по нескольким приходным накладным покупки одновременно, можно использовать функцию Объединить приемки.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 07/02/2020
ms.author: edupont
ms.openlocfilehash: 70433ce496c79edcd053ae345b3b0559cf60b744
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3782903"
---
# <a name="combine-receipts-on-a-single-invoice"></a><span data-ttu-id="5495f-103">Объединение приходных накладных в один счет</span><span class="sxs-lookup"><span data-stu-id="5495f-103">Combine Receipts on a Single Invoice</span></span>

<span data-ttu-id="5495f-104">Если необходимо выставить счет по нескольким приходным накладным покупки одновременно, можно использовать функцию **Объединить приемки**.</span><span class="sxs-lookup"><span data-stu-id="5495f-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span></span>  

<span data-ttu-id="5495f-105">Перед созданием объединенной приходной накладной необходимо учесть более одной приходной накладной для одного и того же поставщика в одной и той же валюте.</span><span class="sxs-lookup"><span data-stu-id="5495f-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span></span> <span data-ttu-id="5495f-106">Другими словами, должны быть заполнены два или более заказов на покупку, и они должны быть учтены как полученные, но без выставленного счета.</span><span class="sxs-lookup"><span data-stu-id="5495f-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span></span>  

<span data-ttu-id="5495f-107">Когда приходные накладные покупки объединяются в счет и учитываются, для строк с выставленным счетом создается учтенный счет покупки.</span><span class="sxs-lookup"><span data-stu-id="5495f-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span></span> <span data-ttu-id="5495f-108">Поле **Кол-во по выст. счетам** в исходном заказе на покупку или в общем заказе на покупку обновляется на основании количества, выставленного по счету.</span><span class="sxs-lookup"><span data-stu-id="5495f-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span></span> <span data-ttu-id="5495f-109">Исходный документ покупки не удаляется, даже если он полностью получен и для него выставлен счет, поэтому документ покупки следует удалить.</span><span class="sxs-lookup"><span data-stu-id="5495f-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span></span>  

> [!NOTE]
> <span data-ttu-id="5495f-110">Полученный счет покупки не может быть впоследствии исправлен или отменен.</span><span class="sxs-lookup"><span data-stu-id="5495f-110">The resulting purchase invoice cannot later be corrected or canceled.</span></span> <span data-ttu-id="5495f-111">Если вы хотите изменить созданный таким образом счет покупки, вы должны использовать кредит-ноты покупки.</span><span class="sxs-lookup"><span data-stu-id="5495f-111">If you want to modify a purchase invoice that is created in this way, you must use purchase credit memos.</span></span> <span data-ttu-id="5495f-112">Дополнительные сведения см. в разделе [Исправление или отмена неоплаченных счетов покупки](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="5495f-112">For more information, see [Correct or Cancel Unpaid Purchase Invoices](purchasing-how-correct-cancel-unpaid-purchase-invoices.md).</span></span>

## <a name="to-combine-receipts"></a><span data-ttu-id="5495f-113">Объединение приемок</span><span class="sxs-lookup"><span data-stu-id="5495f-113">To combine receipts</span></span>

1. <span data-ttu-id="5495f-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5495f-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5495f-115">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="5495f-115">Choose the **New** action.</span></span> <span data-ttu-id="5495f-116">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="5495f-116">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>  
3. <span data-ttu-id="5495f-117">На экспресс-вкладке **Строки** выберите действие **Получить строки приемки**.</span><span class="sxs-lookup"><span data-stu-id="5495f-117">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span></span>  
4. <span data-ttu-id="5495f-118">Выберите несколько строк приемки, которые должны быть включены в счет.</span><span class="sxs-lookup"><span data-stu-id="5495f-118">Select multiple receipt lines that you want to include in the invoice.</span></span>  

    <span data-ttu-id="5495f-119">Если выбраны неправильные строки или если необходимо начать сначала, можно просто удалить строки из счета на покупку и использовать функцию **Получить строки прих. накладной** еще раз.</span><span class="sxs-lookup"><span data-stu-id="5495f-119">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span></span>  
5. <span data-ttu-id="5495f-120">Чтобы учесть счет, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="5495f-120">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a><span data-ttu-id="5495f-121">Удаление открытых заказов на покупку после совмещенного учета приходных накладных</span><span class="sxs-lookup"><span data-stu-id="5495f-121">To remove open purchase orders after combined receipt posting</span></span>

1. <span data-ttu-id="5495f-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удаление заказов на покупку, по которым выставлены счета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5495f-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span></span>  
2. <span data-ttu-id="5495f-123">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="5495f-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="5495f-124">.</span><span class="sxs-lookup"><span data-stu-id="5495f-124">.</span></span>
3. <span data-ttu-id="5495f-125">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="5495f-125">Choose the **OK** button.</span></span>  

<span data-ttu-id="5495f-126">В качестве альтернативы удалите отдельные заказы вручную.</span><span class="sxs-lookup"><span data-stu-id="5495f-126">Alternatively, delete the individual orders manually.</span></span>

<span data-ttu-id="5495f-127">Повторите шаги с 1 по 3 для всех остальных затронутых документов, таких как общие заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="5495f-127">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="5495f-128">См. также</span><span class="sxs-lookup"><span data-stu-id="5495f-128">See Also</span></span>

[<span data-ttu-id="5495f-129">Покупки</span><span class="sxs-lookup"><span data-stu-id="5495f-129">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="5495f-130">Исправление или отмена неоплаченных счетов покупки</span><span class="sxs-lookup"><span data-stu-id="5495f-130">Correct or Cancel Unpaid Purchase Invoices</span></span>](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
<span data-ttu-id="5495f-131">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5495f-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
