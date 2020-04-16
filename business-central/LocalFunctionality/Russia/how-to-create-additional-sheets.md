---
title: Создание дополнительных листов в России
description: Российские усовершенствования включают дополнительные листы для книг НДС покупок и продаж.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: d73c13b9b27f11184e80dac6bdc83aaed8e6cfd7
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180966"
---
# <a name="create-additional-sheets"></a><span data-ttu-id="4c91e-103">Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="4c91e-103">Create Additional Sheets</span></span>

<span data-ttu-id="4c91e-104">В [!INCLUDE[prodshort](../../includes/prodshort.md)] можно создавать дополнительные листы на основе книг НДС покупок и книг НДС продаж.</span><span class="sxs-lookup"><span data-stu-id="4c91e-104">In [!INCLUDE[prodshort](../../includes/prodshort.md)], you can create additional sheets based on VAT purchase ledgers and VAT sales ledgers.</span></span>

## <a name="to-create-entries-for-an-additional-sheet-for-a-vat-purchase-or-sales-ledger"></a><span data-ttu-id="4c91e-105">Создание операций для дополнительного листа книги НДС покупок или продаж</span><span class="sxs-lookup"><span data-stu-id="4c91e-105">To create entries for an additional sheet for a VAT purchase or sales ledger</span></span>

1. <span data-ttu-id="4c91e-106">Выберите строку НДС покупки или продажи в окне **Список книг покупок и продаж** с требуемым учетным периодом.</span><span class="sxs-lookup"><span data-stu-id="4c91e-106">Select the VAT purchase or sales line in the **VAT Ledger List** window with the required accounting period.</span></span>

2. <span data-ttu-id="4c91e-107">Выберите действие **Создать дополнительный лист**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-107">Choose the **Create Additional Sheet** action.</span></span>

3. <span data-ttu-id="4c91e-108">Заполните пакетное задание в соответствии с рекомендациями в "Создание доп. листа книги</span><span class="sxs-lookup"><span data-stu-id="4c91e-108">Fill in the batch job according to the guidelines at Create VAT Sales Led.</span></span> <span data-ttu-id="4c91e-109">НДС</span><span class="sxs-lookup"><span data-stu-id="4c91e-109">Ad.</span></span> <span data-ttu-id="4c91e-110">продаж".</span><span class="sxs-lookup"><span data-stu-id="4c91e-110">Sh..</span></span>

   <span data-ttu-id="4c91e-111">Параметры создания дополнительного листа книги НДС покупок и книги НДС продаж совпадают с параметрами создания формы "НДС Книга Покупок" и формы "НДС Книга Продаж".</span><span class="sxs-lookup"><span data-stu-id="4c91e-111">The parameters for creating a VAT purchase ledger additional sheet and VAT sales ledger additional sheet are the same as the parameters for creating the VAT Purchase Ledger and the VAT Sales Ledger.</span></span>

## <a name="to-print-additional-sheets-on-a-vat-ledger"></a><span data-ttu-id="4c91e-112">Печать дополнительных листов книги НДС</span><span class="sxs-lookup"><span data-stu-id="4c91e-112">To print additional sheets on a VAT Ledger</span></span>

1. <span data-ttu-id="4c91e-113">На странице **НДС книги покупок** или **НДС книги продаж** выберите действие **Дополнительный лист**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-113">On the **VAT Purch. Ledger** or **VAT Sales Ledger** page, choose the **Additional Sheet** action.</span></span>
2. <span data-ttu-id="4c91e-114">В поле **Тип периода** выберите один из вариантов:</span><span class="sxs-lookup"><span data-stu-id="4c91e-114">In the **Period Type** field, select one of the following options:</span></span>

   - <span data-ttu-id="4c91e-115">**День**</span><span class="sxs-lookup"><span data-stu-id="4c91e-115">**Day**</span></span>
   - <span data-ttu-id="4c91e-116">**Месяц**</span><span class="sxs-lookup"><span data-stu-id="4c91e-116">**Month**</span></span>
   - <span data-ttu-id="4c91e-117">**Квартал**</span><span class="sxs-lookup"><span data-stu-id="4c91e-117">**Quarter**</span></span>

   > [!NOTE]
   > <span data-ttu-id="4c91e-118">На вкладке **Книга НДС** автоматически создаются поля **Тип** и **Код**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-118">In the **VAT Ledger** tab, the **Type** field and the **Code** field are automatically created.</span></span>

4. <span data-ttu-id="4c91e-119">Выберите действие **Просмотр** или **Печать**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-119">Choose the **Preview** or **Print** action.</span></span>

## <a name="creating-corrective-documents-to-include-in-additional-sheets"></a><span data-ttu-id="4c91e-120">Создание корректирующих документов для включения в дополнительные листы</span><span class="sxs-lookup"><span data-stu-id="4c91e-120">Creating Corrective Documents to Include in Additional Sheets</span></span>

<span data-ttu-id="4c91e-121">Изменения информации, указанной в счете-фактуре, который был зарегистрирован в предыдущей книге покупок, необходимо отразить в дополнительном листе предыдущей книги (исправленная книга).</span><span class="sxs-lookup"><span data-stu-id="4c91e-121">The information changed in the tax invoice after the invoice is registered in the previous purchase book must be reflected in the additional sheet of the previous book (corrected book).</span></span> <span data-ttu-id="4c91e-122">Этот дополнительный лист является частью книги покупок.</span><span class="sxs-lookup"><span data-stu-id="4c91e-122">The additional sheet is part of the purchase book.</span></span>

<span data-ttu-id="4c91e-123">В первой строке содержатся итоговые значения книги покупок на конец периода, в котором был зарегистрирован этот счет-фактура.</span><span class="sxs-lookup"><span data-stu-id="4c91e-123">The first line contains the totals of the purchase book at the end of the period when the tax invoice is registered.</span></span> <span data-ttu-id="4c91e-124">Следующие строки являются аннулированными счетами-фактурами.</span><span class="sxs-lookup"><span data-stu-id="4c91e-124">The next lines are the annulled tax invoices.</span></span> <span data-ttu-id="4c91e-125">Аннулированные счета-фактуры имеют отрицательный знак, если исправленная сумма счета-фактуры меньше первоначальной суммы, и положительный знак, если исправленная сумма счета-фактуры больше первоначальной суммы.</span><span class="sxs-lookup"><span data-stu-id="4c91e-125">The annulled tax invoices have a negative sign if the corrected invoice amount is lesser than the initial amount, and a positive sign if the corrected invoice amount is greater than the initial amount.</span></span> <span data-ttu-id="4c91e-126">Последняя строка вычисляется как итоговая сумма первой итоговой строки и аннулированных счетов-фактур.</span><span class="sxs-lookup"><span data-stu-id="4c91e-126">The last line is calculated as the sum of the amounts of the first total line and the annulled tax invoices.</span></span>

<span data-ttu-id="4c91e-127">Изменения информации, указанной в счете-фактуре, который был зарегистрирован в предыдущей книге продаж, необходимо отразить в дополнительном листе предыдущей книги (исправленная книга).</span><span class="sxs-lookup"><span data-stu-id="4c91e-127">The information changed in the tax invoice after the invoice is registered in the previous sales book must be reflected in the additional sheet of the previous book (corrected book).</span></span> <span data-ttu-id="4c91e-128">Этот дополнительный лист является частью книги продаж.</span><span class="sxs-lookup"><span data-stu-id="4c91e-128">The additional sheet is part of the sales book.</span></span>

<span data-ttu-id="4c91e-129">В первой строке содержатся итоговые значения книги продаж для конца периода, в котором был зарегистрирован этот счет-фактура.</span><span class="sxs-lookup"><span data-stu-id="4c91e-129">The first line contains totals of the sales book at the end of the period when the tax invoice is registered.</span></span> <span data-ttu-id="4c91e-130">Следующие строки являются аннулированными счетами-фактурами с отрицательными суммами.</span><span class="sxs-lookup"><span data-stu-id="4c91e-130">The next lines are the annulled tax invoices with a negative sign.</span></span> <span data-ttu-id="4c91e-131">Исправленные счета-фактуры с положительными суммами относятся к предыдущему периоду.</span><span class="sxs-lookup"><span data-stu-id="4c91e-131">The corrected invoices with positive amounts belong to the previous period.</span></span> <span data-ttu-id="4c91e-132">Последняя строка вычисляется как итоговая сумма первой итоговой строки, аннулированных счетов-фактур и исправленных счетов.</span><span class="sxs-lookup"><span data-stu-id="4c91e-132">The last line is calculated as the sum of the amounts of the first total line, annulled tax invoices, and the corrected invoices.</span></span>

<span data-ttu-id="4c91e-133">Обработка корректирующих документов для книги продаж аналогична обработке корректирующих документов для книги покупок.</span><span class="sxs-lookup"><span data-stu-id="4c91e-133">Processing of corrective documents for sales book is similar to processing for purchases book with one difference.</span></span> <span data-ttu-id="4c91e-134">Единственное различие заключается в том, что в дополнительных листах необходимо отражать номер и дату исходного счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="4c91e-134">In additional sheets, the number and the date of initial factura must be reflected.</span></span>

### <a name="to-create-a-correction-entry-for-posted-purchase-credit-memos"></a><span data-ttu-id="4c91e-135">Создание корректирующей операции для учтенных кредит-нот покупки</span><span class="sxs-lookup"><span data-stu-id="4c91e-135">To create a correction entry for posted purchase credit memos</span></span>

1. <span data-ttu-id="4c91e-136">Создайте и учтите кредит-ноту покупки.</span><span class="sxs-lookup"><span data-stu-id="4c91e-136">Create and post a purchase credit memo.</span></span>
2. <span data-ttu-id="4c91e-137">Выберите поле **Дополнительный лист книги НДС**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-137">Choose **Additional VAT Ledger Sheet** field.</span></span>
3. <span data-ttu-id="4c91e-138">Заполните следующие поля.</span><span class="sxs-lookup"><span data-stu-id="4c91e-138">Enter information in the following fields:</span></span>
   - <span data-ttu-id="4c91e-139">**Дата скорректированного документа**</span><span class="sxs-lookup"><span data-stu-id="4c91e-139">**Corrected Document Date**</span></span>
   - <span data-ttu-id="4c91e-140">**Дата счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="4c91e-140">**Vendor VAT Invoice Date**</span></span>
   - <span data-ttu-id="4c91e-141">**Дата получения счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="4c91e-141">**Vendor VAT Invoice Rcvd Date**</span></span>
   - <span data-ttu-id="4c91e-142">**Счет-Фактура Но.**</span><span class="sxs-lookup"><span data-stu-id="4c91e-142">**Vendor VAT Invoice No.**</span></span>

### <a name="to-create-a-correction-entry-for-a-posted-purchase-invoice"></a><span data-ttu-id="4c91e-143">Создание корректирующей операции для учтенного счета покупки</span><span class="sxs-lookup"><span data-stu-id="4c91e-143">To create a correction entry for a posted purchase invoice</span></span>

1. <span data-ttu-id="4c91e-144">Создайте и учтите счет покупки.</span><span class="sxs-lookup"><span data-stu-id="4c91e-144">Create and post a purchase invoice.</span></span>
2. <span data-ttu-id="4c91e-145">Выберите поле **Дата скорректированного документа**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-145">Choose the **Corrected Document Date** field.</span></span>
3. <span data-ttu-id="4c91e-146">Заполните следующие поля.</span><span class="sxs-lookup"><span data-stu-id="4c91e-146">Enter information in the following fields:</span></span>

   - <span data-ttu-id="4c91e-147">**Дата счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="4c91e-147">**Vendor VAT Invoice Date**</span></span>
   - <span data-ttu-id="4c91e-148">**Дата получения счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="4c91e-148">**Vendor VAT Invoice Rcvd. Date**</span></span>
   - <span data-ttu-id="4c91e-149">**Счет-Фактура Но.**</span><span class="sxs-lookup"><span data-stu-id="4c91e-149">**Vendor VAT Invoice No.**</span></span>

   > [!NOTE]
   > <span data-ttu-id="4c91e-150">Также можно создать корректирующие документы в финансовом журнале.</span><span class="sxs-lookup"><span data-stu-id="4c91e-150">You can also create corrective documents in the general journal.</span></span> <span data-ttu-id="4c91e-151">Строки финансового журнала содержат все перечисленные выше поля.</span><span class="sxs-lookup"><span data-stu-id="4c91e-151">General journal lines contain all the fields mentioned above.</span></span>

### <a name="to-post-additional-vat"></a><span data-ttu-id="4c91e-152">Учет дополнительного НДС</span><span class="sxs-lookup"><span data-stu-id="4c91e-152">To post additional VAT</span></span>

1. <span data-ttu-id="4c91e-153">В окне **Счет продажи** или **Кредит-нота** откройте вкладку **НДС**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-153">In the **Sales Invoice** window or the **Credit Memo** window, choose the **VAT** tab.</span></span>

2. <span data-ttu-id="4c91e-154">Заполните поле **Учетный номер**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-154">Enter the **Posting No.**</span></span> <span data-ttu-id="4c91e-155">.</span><span class="sxs-lookup"><span data-stu-id="4c91e-155">field.</span></span>

   > [!NOTE]
   > <span data-ttu-id="4c91e-156">Нельзя учесть счет с тем же номером, что и у исходного счета.</span><span class="sxs-lookup"><span data-stu-id="4c91e-156">You cannot post an invoice with the same number as the initial invoice.</span></span> <span data-ttu-id="4c91e-157">Необходимо добавить к исходному номеру еще один дополнительный символ.</span><span class="sxs-lookup"><span data-stu-id="4c91e-157">You must use an extra symbol in addition to the initial number.</span></span>

3. <span data-ttu-id="4c91e-158">Выберите поле **Дополнительный лист книги НДС**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-158">Select the **Additional VAT Ledger Sheet** field.</span></span>

4. <span data-ttu-id="4c91e-159">Заполните поле **Дата скорректированного документа**.</span><span class="sxs-lookup"><span data-stu-id="4c91e-159">Enter information in the **Corrected Document Date** field.</span></span>

5. <span data-ttu-id="4c91e-160">В дополнительном листе поле **Дата Счета-Фактуры** отражает дату корректируемого документа.</span><span class="sxs-lookup"><span data-stu-id="4c91e-160">In the additional sheet, the **Date of Facture** field reflects the corrected document date.</span></span>

## <a name="see-also"></a><span data-ttu-id="4c91e-161">См. также</span><span class="sxs-lookup"><span data-stu-id="4c91e-161">See Also</span></span>

[<span data-ttu-id="4c91e-162">Книги НДС</span><span class="sxs-lookup"><span data-stu-id="4c91e-162">VAT Ledgers</span></span>](VAT-Ledgers.md)
