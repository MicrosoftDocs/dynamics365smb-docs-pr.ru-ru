---
title: "Отмена учета путем учета сторнирующей операции | Документы Майкрософт"
description: "Если выполнен ошибочный учет в финансовом журнале, можно воспользоваться функцией сторнирования транзакции, чтобы отменить учет, сохранив корректный след аудита."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: cc624d52ce61cea4a8e92bb7d37e07ad8c769393
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="reverse-postings"></a><span data-ttu-id="01dfe-103">Сторнирование учета</span><span class="sxs-lookup"><span data-stu-id="01dfe-103">Reverse Postings</span></span>
<span data-ttu-id="01dfe-104">Что отменить ошибочную проводку в журнале, выберите операцию и создайте сторнирующую операцию (операции, идентичные исходным, но с противоположным знаком в поле суммы) с таким же номером документа и датой учета, что и у исходной операции.</span><span class="sxs-lookup"><span data-stu-id="01dfe-104">To undo an erroneous journal posting, you select the entry and create a reverse entry (entries identical to the original entry but with opposite sign in the amount field) with the same document number and posting date as the original entry.</span></span> <span data-ttu-id="01dfe-105">После сторнирования операции необходимо создать корректирующую запись.</span><span class="sxs-lookup"><span data-stu-id="01dfe-105">After reversing an entry, you must make the correct entry.</span></span>

<span data-ttu-id="01dfe-106">Можно сторнировать только те операции, которые были учтены из строки финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="01dfe-106">You can only reverse entries that are posted from a general journal line.</span></span> <span data-ttu-id="01dfe-107">Операцию можно сторнировать только один раз.</span><span class="sxs-lookup"><span data-stu-id="01dfe-107">An entry can only be reversed once.</span></span>

<span data-ttu-id="01dfe-108">Дополнительные сведения об учете из финансового журнала, см. в разделе [Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="01dfe-108">For more information about posting from a general journal, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>

<span data-ttu-id="01dfe-109">В случае учета неправильного отрицательного количества, например если сделан заказ покупки с неправильным числом товаров, и принят к учету как полученный (но без выставления счета), то эту операцию можно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-109">If you have made an incorrect negative quantity posting, such as a purchase order with the wrong number of items and posted it as received but not invoiced, then you can undo the posting.</span></span>

<span data-ttu-id="01dfe-110">В случае учета неправильного положительного количества, например если сделан заказ возврата покупки с неправильным числом товаров, и принят к учету как отгруженный (но без выставления счета), то эту операцию можно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-110">If you have made an incorrect positive quantity posting, such as a purchase return order with the wrong number of items and posted it as shipped but not invoiced, then you can undo the posting.</span></span>   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a><span data-ttu-id="01dfe-111">Сторнирование учета в журнале для операции главной книги</span><span class="sxs-lookup"><span data-stu-id="01dfe-111">To reverse the journal posting of a general ledger entry</span></span>
<span data-ttu-id="01dfe-112">Операции можно сторнировать со всех страниц **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-112">You can reverse entries from all **Ledger Entries** pages.</span></span> <span data-ttu-id="01dfe-113">Следующая процедура основана на странице **Операции главной книги**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-113">The following procedure is based on the **General Ledger Entries** page.</span></span>
1. <span data-ttu-id="01dfe-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Операции главной книги**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="01dfe-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="01dfe-115">Выберите операцию, которую требуется сторнировать, а затем выберите **Сторнировать транзакцию**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-115">Select the entry that you want to reverse, and then choose the **Reverse Transaction** action.</span></span> <span data-ttu-id="01dfe-116">Следует отметить, что операцию нужно выполнять из учтенной операции в журнале.</span><span class="sxs-lookup"><span data-stu-id="01dfe-116">Note that is must originate from a journal posting.</span></span>
3. <span data-ttu-id="01dfe-117">На странице **Сторнировать операции транзакции** выберите соответствующую операцию, а затем выберите действие **Сторнировать**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-117">On the **Reverse Transaction Entries** page, select the relevant entry, and then choose the **Reverse** action.</span></span>
4. <span data-ttu-id="01dfe-118">Нажмите кнопку **Да** в сообщении подтверждения.</span><span class="sxs-lookup"><span data-stu-id="01dfe-118">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a><span data-ttu-id="01dfe-119">Отмена учета количества в учтенной приходной накладной покупки</span><span class="sxs-lookup"><span data-stu-id="01dfe-119">To undo a quantity posting on a posted purchase receipt</span></span>  

1.  <span data-ttu-id="01dfe-120">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные приходные накладные покупки**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="01dfe-120">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Purchase Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="01dfe-121">Откройте учтенную приемку, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-121">Open the posted receipt that you want to undo.</span></span>  
3.  <span data-ttu-id="01dfe-122">Выберите строку или строки, которые нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-122">Select the line or lines that you want to undo.</span></span>  
4.  <span data-ttu-id="01dfe-123">Выберите действие **Отменить прих. накладную**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-123">Choose **Undo Receipt** action.</span></span>

    <span data-ttu-id="01dfe-124">Корректирующая строка вставляется под выбранной строкой приходной накладной.</span><span class="sxs-lookup"><span data-stu-id="01dfe-124">A corrective line is inserted under the selected receipt line.</span></span>  

    <span data-ttu-id="01dfe-125">Если количество получено в складской приемке, то в учтенную складскую приемку вставлена корректирующая строка.</span><span class="sxs-lookup"><span data-stu-id="01dfe-125">If the quantity was received in a warehouse receipt, then a corrective line is inserted in the posted warehouse receipt.</span></span>  

    <span data-ttu-id="01dfe-126">Значения в полях **Полученное кол-во** и **Получ. кол-во без выст. счета** в соответствующем заказе на покупку сводятся к нулю.</span><span class="sxs-lookup"><span data-stu-id="01dfe-126">The **Quantity Received** and **Qty. Rcd. Not Invoiced** fields on the related purchase order are set to zero.</span></span>

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a><span data-ttu-id="01dfe-127">Отмена учета и последующий повторный учет количества в учтенной расходной накладной по возврату</span><span class="sxs-lookup"><span data-stu-id="01dfe-127">To undo and then redo a quantity posting on a posted return shipment</span></span>

1.  <span data-ttu-id="01dfe-128">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные возвр. расх. накладные**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="01dfe-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Return Shipments**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="01dfe-129">Откройте учтенную возвратную расходную накладную, которую нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-129">Open the posted return shipment that you want to undo.</span></span>
3. <span data-ttu-id="01dfe-130">Выберите строку или строки, которые нужно отменить.</span><span class="sxs-lookup"><span data-stu-id="01dfe-130">Select the line or lines you want to undo.</span></span>  

4.  <span data-ttu-id="01dfe-131">Выберите действие **Отменить возвр. расх. накладную**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-131">Choose the **Undo Return Shipment** action.</span></span>  

    <span data-ttu-id="01dfe-132">В учтенный документ вставляется корректирующая строка, а поля **Отгруженное кол-во возвр.** и **Возврат, отгруженный без выст. счета** в заказе на возврат устанавливаются равными нулю.</span><span class="sxs-lookup"><span data-stu-id="01dfe-132">A corrective line is inserted in the posted document, and the **Return Qty. Shipped** and **Return Shpd. Not Invd.** fields on the return order are set to zero.</span></span>  

    <span data-ttu-id="01dfe-133">Теперь вернитесь в окно возврата покупки, чтобы переделать учет.</span><span class="sxs-lookup"><span data-stu-id="01dfe-133">Now go back to the purchase return order to redo the posting.</span></span>  

5.  <span data-ttu-id="01dfe-134">На странице **Учтенная возвр. расх. накладная** запомните номер в поле **Номер возврата**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-134">On the **Posted Return Shipment** page, take a note of the number in the **Return Order No.**</span></span> <span data-ttu-id="01dfe-135">.</span><span class="sxs-lookup"><span data-stu-id="01dfe-135">field.</span></span>  
6.  <span data-ttu-id="01dfe-136">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Возвраты покупок**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="01dfe-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Return Orders**, and then select the related link.</span></span>  
7.  <span data-ttu-id="01dfe-137">Откройте требуемый заказ на возврат, затем выберите действие **Открыть повторно**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-137">Open the return order in question, and then choose the **Reopen** action.</span></span>  
8.  <span data-ttu-id="01dfe-138">Исправьте запись в поле **Кол-во** и снова выполните учет возврата покупки.</span><span class="sxs-lookup"><span data-stu-id="01dfe-138">Correct the entry in the **Quantity** field and post the purchase return order again.</span></span>  

## <a name="to-post-a-negative-entry"></a><span data-ttu-id="01dfe-139">Учет расхода</span><span class="sxs-lookup"><span data-stu-id="01dfe-139">To post a negative entry</span></span>  
<span data-ttu-id="01dfe-140">Можно использовать поле **Коррекция** для учета отрицательного дебета вместо кредита или учета отрицательного кредита вместо дебета по счету.</span><span class="sxs-lookup"><span data-stu-id="01dfe-140">You can use the **Correction** field to post a negative debit instead of a credit, or to post a negative credit instead of a debit on an account.</span></span> <span data-ttu-id="01dfe-141">Для выполнения юридических требований это поле по умолчанию видно во всех журналах.</span><span class="sxs-lookup"><span data-stu-id="01dfe-141">To meet legal requirements, this field is visible by default in all journals.</span></span> <span data-ttu-id="01dfe-142">Поля **Сумма по дебету** и **Сумма по кредиту** включают как исходную операцию, так и скорректированную операцию.</span><span class="sxs-lookup"><span data-stu-id="01dfe-142">The **Debit Amount** and **Credit Amount** fields include both the original entry, and the corrected entry.</span></span> <span data-ttu-id="01dfe-143">Эти поля не оказывают влияния на сальдо счета.</span><span class="sxs-lookup"><span data-stu-id="01dfe-143">These fields have no effect on the account balance.</span></span>  

1.  <span data-ttu-id="01dfe-144">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые журналы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="01dfe-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link</span></span>  
2.  <span data-ttu-id="01dfe-145">В поле **Код раздела** выберите требуемое название раздела.</span><span class="sxs-lookup"><span data-stu-id="01dfe-145">In the **Batch Name** field, select the required batch name.</span></span>  
3.  <span data-ttu-id="01dfe-146">Заполните соответствующие поля.</span><span class="sxs-lookup"><span data-stu-id="01dfe-146">Enter information into the relevant fields.</span></span>  
4.  <span data-ttu-id="01dfe-147">В строке журнала. которую необходимо активизировать для отрицательных операций, установите флажок **Коррекция**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-147">In the journal line that you want to activate for negative entries, select the **Correction** check box.</span></span>  
5.  <span data-ttu-id="01dfe-148">Для учета журнала выберите действие **Учет**, затем выберите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="01dfe-148">To post the journal, choose the **Post** action, and then choose the **Yes** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="01dfe-149">См. также</span><span class="sxs-lookup"><span data-stu-id="01dfe-149">See Also</span></span>
<span data-ttu-id="01dfe-150">[Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="01dfe-150">[Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md)</span></span>  
[<span data-ttu-id="01dfe-151">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="01dfe-151">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="01dfe-152">Финансы</span><span class="sxs-lookup"><span data-stu-id="01dfe-152">Finance</span></span>](finance.md)  
<span data-ttu-id="01dfe-153">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="01dfe-153">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

