---
title: "Как объединить приходные накладные | Документы Майкрософт"
description: "Если необходимо выставить счет по нескольким приходным накладным покупки одновременно, можно использовать функцию Объединить приемки."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 2176baf2947a08785fdf6327b2ebebf35686d04a
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="combine-receipts-on-a-single-invoice"></a><span data-ttu-id="f7498-103">Объединение приходных накладных в один счет</span><span class="sxs-lookup"><span data-stu-id="f7498-103">Combine Receipts on a Single Invoice</span></span>
<span data-ttu-id="f7498-104">Если необходимо выставить счет по нескольким приходным накладным покупки одновременно, можно использовать функцию **Объединить приемки**.</span><span class="sxs-lookup"><span data-stu-id="f7498-104">If you want to invoice more than one purchase receipt at a time, you can use the **Combine Receipts** function.</span></span>  

<span data-ttu-id="f7498-105">Перед созданием объединенной приходной накладной необходимо учесть более одной приходной накладной для одного и того же поставщика в одной и той же валюте.</span><span class="sxs-lookup"><span data-stu-id="f7498-105">Before you can create a combined purchase receipt, more than one receipt from the same vendor in the same currency must be posted.</span></span> <span data-ttu-id="f7498-106">Другими словами, должны быть заполнены два или более заказов на покупку, и они должны быть учтены как полученные, но без выставленного счета.</span><span class="sxs-lookup"><span data-stu-id="f7498-106">In other words, you must have filled in two or more purchase orders and posted them as received, but not invoiced.</span></span>  

<span data-ttu-id="f7498-107">Когда приходные накладные покупки объединяются в счет и учитываются, для строк с выставленным счетом создается учтенный счет покупки.</span><span class="sxs-lookup"><span data-stu-id="f7498-107">When purchase receipts are combined on an invoice and posted, then a posted purchase invoice is created for the invoiced lines.</span></span> <span data-ttu-id="f7498-108">Поле **Кол-во по выст. счетам** в исходном заказе на покупку или в общем заказе на покупку обновляется на основании количества, выставленного по счету.</span><span class="sxs-lookup"><span data-stu-id="f7498-108">The **Quantity Invoiced** field on the originating purchase order, or blanket purchase order, is updated based on the invoiced quantity.</span></span> <span data-ttu-id="f7498-109">Исходный документ покупки не удаляется, даже если он полностью получен и для него выставлен счет, поэтому документ покупки следует удалить.</span><span class="sxs-lookup"><span data-stu-id="f7498-109">However, this original purchase document is not deleted, even if it has been fully received and invoiced, and you must therefore delete the purchase document.</span></span>  

## <a name="to-combine-receipts"></a><span data-ttu-id="f7498-110">Объединение приемок</span><span class="sxs-lookup"><span data-stu-id="f7498-110">To combine receipts</span></span>  
1. <span data-ttu-id="f7498-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета покупки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7498-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f7498-112">Выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="f7498-112">Choose the **New** action.</span></span> <span data-ttu-id="f7498-113">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="f7498-113">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>  
3. <span data-ttu-id="f7498-114">На экспресс-вкладке **Строки** выберите действие **Получить строки приемки**.</span><span class="sxs-lookup"><span data-stu-id="f7498-114">On the **Lines** FastTab, choose the **Get Receipt Lines** action.</span></span>  
4. <span data-ttu-id="f7498-115">Выберите несколько строк приемки, которые должны быть включены в счет.</span><span class="sxs-lookup"><span data-stu-id="f7498-115">Select multiple receipt lines that you want to include in the invoice.</span></span>  

    <span data-ttu-id="f7498-116">Если выбраны неправильные строки или если необходимо начать сначала, можно просто удалить строки из счета на покупку и использовать функцию **Получить строки прих. накладной** еще раз.</span><span class="sxs-lookup"><span data-stu-id="f7498-116">If an incorrect receipt line was selected or you want to start over, you can just delete the lines on the purchase invoice and then use the **Get Receipt Lines** function again.</span></span>  
5. <span data-ttu-id="f7498-117">Чтобы учесть счет, выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="f7498-117">To post the invoice, choose the **Post** action.</span></span>  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a><span data-ttu-id="f7498-118">Удаление открытых заказов на покупку после совмещенного учета приходных накладных</span><span class="sxs-lookup"><span data-stu-id="f7498-118">To remove open purchase orders after combined receipt posting</span></span>  
1. <span data-ttu-id="f7498-119">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Удалить заказы на покупку, по которым выставлены счета**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7498-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Invoiced Purchase Orders**, and select the related link.</span></span>  
2. <span data-ttu-id="f7498-120">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="f7498-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="f7498-121">.</span><span class="sxs-lookup"><span data-stu-id="f7498-121">.</span></span>
3. <span data-ttu-id="f7498-122">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f7498-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="f7498-123">В качестве альтернативы удалите отдельные заказы вручную.</span><span class="sxs-lookup"><span data-stu-id="f7498-123">Alternatively, delete the individual orders manually.</span></span>

<span data-ttu-id="f7498-124">Повторите шаги с 1 по 3 для всех остальных затронутых документов, таких как общие заказы на покупку.</span><span class="sxs-lookup"><span data-stu-id="f7498-124">Repeat steps 1 through 3 for any other affected documents, such as blanket purchase orders.</span></span>

## <a name="see-also"></a><span data-ttu-id="f7498-125">См. также</span><span class="sxs-lookup"><span data-stu-id="f7498-125">See Also</span></span>  
[<span data-ttu-id="f7498-126">Покупки</span><span class="sxs-lookup"><span data-stu-id="f7498-126">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="f7498-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f7498-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

