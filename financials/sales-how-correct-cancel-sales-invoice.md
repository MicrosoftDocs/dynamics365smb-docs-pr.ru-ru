---
title: "Исправление или отмена учтенных счетов продажи | Документы Майкрософт"
description: "Описывается, как исправить или отменить учтенный счет продажи и применить кредит-ноту продажи."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: undo, credit memo, return
ms.date: 08/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: acef03f32124c5983846bc6ed0c4d332c9c8b347
ms.openlocfilehash: 558b01a2d7048b8a5817a61b26e3df61d007815d
ms.contentlocale: ru-ru
ms.lasthandoff: 04/16/2018

---
# <a name="correct-or-cancel-unpaid-sales-invoices"></a><span data-ttu-id="8d5d4-103">Исправление или отмена неоплаченных счетов продажи</span><span class="sxs-lookup"><span data-stu-id="8d5d4-103">Correct or Cancel Unpaid Sales Invoices</span></span>
<span data-ttu-id="8d5d4-104">Можно исправить или отменить учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-104">You can correct or cancel a posted sales invoice.</span></span> <span data-ttu-id="8d5d4-105">Это полезно, если сделана ошибка или клиент запрашивает изменение.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-105">This is useful if you make a mistake or if the customer requests a change.</span></span>

> [!NOTE]  
>   <span data-ttu-id="8d5d4-106">После полной или частичной оплаты учтенного счета продажи его нельзя изменить или отменить из учтенного счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-106">After a posted sales invoice has been partially or fully paid, you cannot correct or cancel it from the posted sales invoice itself.</span></span> <span data-ttu-id="8d5d4-107">Вместо этого следует вручную создать кредит-ноту продажи для аннулирования продажи и возмещения средств клиенту, при необходимости с управлением по заказу на возврат продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-107">Instead, you must manually create a sales credit memo to void the sale and reimburse the customer, optionally managed with a sales return order.</span></span> <span data-ttu-id="8d5d4-108">Дополнительные сведения см. в разделе [Обработка возвратов продажи или отмен](sales-how-process-sales-returns-cancellations.md)</span><span class="sxs-lookup"><span data-stu-id="8d5d4-108">For more information, see [Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).</span></span>

<span data-ttu-id="8d5d4-109">В окне **Учтенный счет продажи** можно выбрать действие **Исправить** или **Отмена** для выполнения действий, описанных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-109">In the **Posted Sales Invoice** window, you can choose the **Correct** action or the **Cancel** action to perform the actions that are described in the following table.</span></span>

| <span data-ttu-id="8d5d4-110">Действие</span><span class="sxs-lookup"><span data-stu-id="8d5d4-110">Action</span></span> | <span data-ttu-id="8d5d4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d5d4-111">Description</span></span> |
| --- | --- |
| <span data-ttu-id="8d5d4-112">**Исправить**</span><span class="sxs-lookup"><span data-stu-id="8d5d4-112">**Correct**</span></span> |<span data-ttu-id="8d5d4-113">Учтенный счет продажи отменяется.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-113">The posted sales invoice is canceled.</span></span> <span data-ttu-id="8d5d4-114">Создается новый счет продажи с теми же сведениями.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-114">A new sales invoice with the same information is created.</span></span> <span data-ttu-id="8d5d4-115">Можно сделать корректировку. а затем продолжить процесс продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-115">You can make the correction and then continue the sales process.</span></span> <span data-ttu-id="8d5d4-116">Новый счет продажи имеет номер, отличный от номера первоначального счета.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-116">The new sales invoice has a different number than the initial sales invoice.</span></span> <span data-ttu-id="8d5d4-117">Автоматически создается корректирующая кредит-нота продажи, которая учитывается для аннулирования исходного учтенного счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-117">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="8d5d4-118">В исходном учтенном счете продажи устанавливаются флажки "Отменено" и "Оплачено".</span><span class="sxs-lookup"><span data-stu-id="8d5d4-118">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |
| <span data-ttu-id="8d5d4-119">**Отмена**</span><span class="sxs-lookup"><span data-stu-id="8d5d4-119">**Cancel**</span></span> |<span data-ttu-id="8d5d4-120">Учтенный счет продажи отменяется.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-120">The posted sales invoice is canceled.</span></span> <span data-ttu-id="8d5d4-121">Автоматически создается корректирующая кредит-нота продажи, которая учитывается для аннулирования исходного учтенного счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-121">A corrective sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="8d5d4-122">В исходном учтенном счете продажи устанавливаются флажки "Отменено" и "Оплачено".</span><span class="sxs-lookup"><span data-stu-id="8d5d4-122">On the initial posted sales invoice, the Canceled and Paid check boxes are selected.</span></span> |

<span data-ttu-id="8d5d4-123">При корректировке или отмене учтенного счета продажи корректирующая кредит-нота продажи применяется ко всем операциям ГК и журнала товаров, созданным при учете первоначального счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-123">When you correct or cancel a posted sales invoice, the corrective sales credit memo is applied to all general ledger and inventory ledger entries that were created when the initial sales invoice was posted.</span></span> <span data-ttu-id="8d5d4-124">При этом сторнируется учтенный счет продажи в финансовых записях и оставляется корректирующая учтенная кредит-нота продажи для аудиторского следа.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-124">This reverses the posted sales invoice in your financial records and leaves the corrective posted sales credit memo for your audit trail.</span></span>

## <a name="to-correct-a-posted-sales-invoice"></a><span data-ttu-id="8d5d4-125">Коррекция учтенного счета продажи</span><span class="sxs-lookup"><span data-stu-id="8d5d4-125">To correct a posted sales invoice</span></span>
1. <span data-ttu-id="8d5d4-126">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учтенные счета продажи**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8d5d4-127">Выберите учтенный счет продажи, который требуется откорректировать.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-127">Select the posted sales invoice that you want to correct.</span></span>

    > [!NOTE]  
   >   <span data-ttu-id="8d5d4-128">Если установлен флажок **Отменено**, невозможно откорректировать учтенный счет продажи, поскольку он уже откорректирован или отменен.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-128">If the **Canceled** check box is selected, then you cannot correct the posted sales invoice because it has already been corrected or canceled.</span></span>
3. <span data-ttu-id="8d5d4-129">В окне **Учтенный счет продажи** выберите действие **Исправить**.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-129">In the **Posted Sales Invoice** window, choose the **Correct** action.</span></span>  
4. <span data-ttu-id="8d5d4-130">Создается новый счет продажи с теми же сведениями, в который можно внести изменения.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-130">A new sales invoice with the same information is created where you can make the correction.</span></span> <span data-ttu-id="8d5d4-131">Значение в поле **Отменено** в исходном учтенном счете продажи изменится на **Да**.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-131">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>

    <span data-ttu-id="8d5d4-132">Автоматически создается кредит-нота продажи, которая учитывается для аннулирования исходного учтенного счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-132">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span>
5. <span data-ttu-id="8d5d4-133">Выберите действие **Показать корректирующую кредит-ноту**, чтобы просмотреть учтенную кредит-ноту продажи, которая аннулирует исходный учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-133">Choose the **Show Corrective Credit Memo** action to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="to-cancel-a-posted-sales-invoice"></a><span data-ttu-id="8d5d4-134">Отмена учтенного счета продажи</span><span class="sxs-lookup"><span data-stu-id="8d5d4-134">To cancel a posted sales invoice</span></span>
1. <span data-ttu-id="8d5d4-135">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Учтенные счета продажи**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8d5d4-136">Выберите учтенный счет продажи, который требуется отменить.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-136">Select the posted sales invoice that you want to cancel.</span></span>

    > [!NOTE]  
   >   <span data-ttu-id="8d5d4-137">Если установлен флажок **Отменено**, невозможно отменить учтенный счет продажи, поскольку он уже отменена или откорректирован.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-137">If the **Canceled** check box is selected, then you cannot cancel the posted sales invoice because it has already been canceled or corrected.</span></span>
3. <span data-ttu-id="8d5d4-138">В окне **Учтенный счет продажи** выберите действие **Отмена**.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-138">In the **Posted Sales Invoice** window, choose the **Cancel** action.</span></span>

    <span data-ttu-id="8d5d4-139">Автоматически создается кредит-нота продажи, которая учитывается для аннулирования исходного учтенного счета продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-139">A sales credit memo is automatically created and posted to void the initial posted sales invoice.</span></span> <span data-ttu-id="8d5d4-140">Значение в поле **Отменено** в исходном учтенном счете продажи изменится на **Да**.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-140">The **Canceled** field on the initial posted sales invoice is changed to **Yes**.</span></span>
4. <span data-ttu-id="8d5d4-141">Выберите **Показать корректирующую кредит-ноту**, чтобы просмотреть учтенную кредит-ноту продажи, которая аннулирует исходный учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="8d5d4-141">Choose **Show Corrective Credit Memo** to view the posted sales credit memo that voids the initial posted sales invoice.</span></span>

## <a name="see-also"></a><span data-ttu-id="8d5d4-142">См. также</span><span class="sxs-lookup"><span data-stu-id="8d5d4-142">See Also</span></span>
[<span data-ttu-id="8d5d4-143">Продажи</span><span class="sxs-lookup"><span data-stu-id="8d5d4-143">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="8d5d4-144">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="8d5d4-144">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="8d5d4-145">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="8d5d4-145">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="8d5d4-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8d5d4-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

