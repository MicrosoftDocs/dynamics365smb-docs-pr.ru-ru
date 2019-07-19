---
title: Создание дополнительных листов в России
description: Российские усовершенствования включают дополнительные листы для книг НДС покупок и продаж.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 07/02/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 66062781d04dd5e9c7f3db027ecce5919d607e62
ms.sourcegitcommit: 8fe694b7bbe7fc0456ed5a9e42291218d2251b05
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2019
ms.locfileid: "1738218"
---
# <a name="how-to-create-additional-sheets"></a><span data-ttu-id="b9907-103">Практическое руководство. Создание дополнительных листов</span><span class="sxs-lookup"><span data-stu-id="b9907-103">How to: Create Additional Sheets</span></span>

<span data-ttu-id="b9907-104">В [!INCLUDE[prodshort](../../includes/prodshort.md)] можно создавать дополнительные листы на основе книг НДС покупок и книг НДС продаж.</span><span class="sxs-lookup"><span data-stu-id="b9907-104">In [!INCLUDE[prodshort](../../includes/prodshort.md)], you can create additional sheets based on VAT purchase ledgers and VAT sales ledgers.</span></span>

### <a name="to-create-entries-for-an-additional-sheet-for-a-vat-purchase-or-sales-ledger"></a><span data-ttu-id="b9907-105">Создание операций для дополнительного листа книги НДС покупок или продаж</span><span class="sxs-lookup"><span data-stu-id="b9907-105">To create entries for an additional sheet for a VAT purchase or sales ledger</span></span>

1. <span data-ttu-id="b9907-106">Выберите строку НДС покупки или продажи в окне **Список книг покупок и продаж** с требуемым учетным периодом.</span><span class="sxs-lookup"><span data-stu-id="b9907-106">Select the VAT purchase or sales line in the **VAT Ledger List** window with the required accounting period.</span></span>

2. <span data-ttu-id="b9907-107">На вкладке **Действия** выберите **Функции**, а затем выберите **Создать дополнительный лист**.</span><span class="sxs-lookup"><span data-stu-id="b9907-107">On the **Actions** tab, choose **Functions**, and then choose **Create Additional Sheet**.</span></span>

3. <span data-ttu-id="b9907-108">Заполните пакетное задание в соответствии с рекомендациями в "Создание доп. листа книги</span><span class="sxs-lookup"><span data-stu-id="b9907-108">Fill in the batch job according to the guidelines at Create VAT Sales Led.</span></span> <span data-ttu-id="b9907-109">НДС</span><span class="sxs-lookup"><span data-stu-id="b9907-109">Ad.</span></span> <span data-ttu-id="b9907-110">продаж".</span><span class="sxs-lookup"><span data-stu-id="b9907-110">Sh..</span></span>

   <span data-ttu-id="b9907-111">Параметры создания дополнительного листа книги НДС покупок и книги НДС продаж совпадают с параметрами создания формы "НДС Книга Покупок" и формы "НДС Книга Продаж".</span><span class="sxs-lookup"><span data-stu-id="b9907-111">The parameters for creating a VAT purchase ledger additional sheet and VAT sales ledger additional sheet are the same as the parameters for creating the VAT Purchase Ledger and the VAT Sales Ledger.</span></span>

### <a name="to-print-additional-sheets-on-a-vat-ledger"></a><span data-ttu-id="b9907-112">Печать дополнительных листов книги НДС</span><span class="sxs-lookup"><span data-stu-id="b9907-112">To print additional sheets on a VAT Ledger</span></span> 

1. <span data-ttu-id="b9907-113">В окне **Книга покупок** или **Книга продаж** на вкладке **Действия** выберите вкладку **Параметры**.</span><span class="sxs-lookup"><span data-stu-id="b9907-113">In the **VAT Purch. Ledger** or **VAT Sales Ledger**, on the **Actions** tab, choose **Options** tab.</span></span>

2. <span data-ttu-id="b9907-114">Выберите **Дополнительный лист**.</span><span class="sxs-lookup"><span data-stu-id="b9907-114">Choose **Additional sheet**.</span></span>

3. <span data-ttu-id="b9907-115">В поле **Тип периода** выберите один из вариантов:</span><span class="sxs-lookup"><span data-stu-id="b9907-115">In the **Period Type** field, select one of the following options:</span></span>

   - <span data-ttu-id="b9907-116">**День**</span><span class="sxs-lookup"><span data-stu-id="b9907-116">**Day**</span></span>
   - <span data-ttu-id="b9907-117">**Месяц**</span><span class="sxs-lookup"><span data-stu-id="b9907-117">**Month**</span></span>
   - <span data-ttu-id="b9907-118">**Квартал**</span><span class="sxs-lookup"><span data-stu-id="b9907-118">**Quarter**</span></span>

   > :speech_balloon: <span data-ttu-id="b9907-119">Примечание</span><span class="sxs-lookup"><span data-stu-id="b9907-119">Note</span></span>
   >
   > <span data-ttu-id="b9907-120">На вкладке **Книга НДС** автоматически создаются поля **Тип** и **Код**.</span><span class="sxs-lookup"><span data-stu-id="b9907-120">In the **VAT Ledger** tab, the **Type** field and the **Code** field are automatically created.</span></span>

4. <span data-ttu-id="b9907-121">Выберите **Просмотр** или **Печать**.</span><span class="sxs-lookup"><span data-stu-id="b9907-121">Choose **Preview** or choose **Print**.</span></span>

## <a name="creating-corrective-documents-to-include-in-additional-sheets"></a><span data-ttu-id="b9907-122">Создание корректирующих документов для включения в дополнительные листы</span><span class="sxs-lookup"><span data-stu-id="b9907-122">Creating Corrective Documents to Include in Additional Sheets</span></span>

<span data-ttu-id="b9907-123">Изменения информации, указанной в счете-фактуре, который был зарегистрирован в предыдущей книге покупок, необходимо отразить в дополнительном листе предыдущей книги (исправленная книга).</span><span class="sxs-lookup"><span data-stu-id="b9907-123">The information changed in the tax invoice after the invoice is registered in the previous purchase book must be reflected in the additional sheet of the previous book (corrected book).</span></span> <span data-ttu-id="b9907-124">Этот дополнительный лист является частью книги покупок.</span><span class="sxs-lookup"><span data-stu-id="b9907-124">The additional sheet is part of the purchase book.</span></span>

<span data-ttu-id="b9907-125">В первой строке содержатся итоговые значения книги покупок на конец периода, в котором был зарегистрирован этот счет-фактура.</span><span class="sxs-lookup"><span data-stu-id="b9907-125">The first line contains the totals of the purchase book at the end of the period when the tax invoice is registered.</span></span> <span data-ttu-id="b9907-126">Следующие строки являются аннулированными счетами-фактурами.</span><span class="sxs-lookup"><span data-stu-id="b9907-126">The next lines are the annulled tax invoices.</span></span> <span data-ttu-id="b9907-127">Аннулированные счета-фактуры имеют отрицательный знак, если исправленная сумма счета-фактуры меньше первоначальной суммы, и положительный знак, если исправленная сумма счета-фактуры больше первоначальной суммы.</span><span class="sxs-lookup"><span data-stu-id="b9907-127">The annulled tax invoices have a negative sign if the corrected invoice amount is lesser than the initial amount, and a positive sign if the corrected invoice amount is greater than the initial amount.</span></span> <span data-ttu-id="b9907-128">Последняя строка вычисляется как итоговая сумма первой итоговой строки и аннулированных счетов-фактур.</span><span class="sxs-lookup"><span data-stu-id="b9907-128">The last line is calculated as the sum of the amounts of the first total line and the annulled tax invoices.</span></span>

<span data-ttu-id="b9907-129">Изменения информации, указанной в счете-фактуре, который был зарегистрирован в предыдущей книге продаж, необходимо отразить в дополнительном листе предыдущей книги (исправленная книга).</span><span class="sxs-lookup"><span data-stu-id="b9907-129">The information changed in the tax invoice after the invoice is registered in the previous sales book must be reflected in the additional sheet of the previous book (corrected book).</span></span> <span data-ttu-id="b9907-130">Этот дополнительный лист является частью книги продаж.</span><span class="sxs-lookup"><span data-stu-id="b9907-130">The additional sheet is part of the sales book.</span></span>

<span data-ttu-id="b9907-131">В первой строке содержатся итоговые значения книги продаж для конца периода, в котором был зарегистрирован этот счет-фактура.</span><span class="sxs-lookup"><span data-stu-id="b9907-131">The first line contains totals of the sales book at the end of the period when the tax invoice is registered.</span></span> <span data-ttu-id="b9907-132">Следующие строки являются аннулированными счетами-фактурами с отрицательными суммами.</span><span class="sxs-lookup"><span data-stu-id="b9907-132">The next lines are the annulled tax invoices with a negative sign.</span></span> <span data-ttu-id="b9907-133">Исправленные счета-фактуры с положительными суммами относятся к предыдущему периоду.</span><span class="sxs-lookup"><span data-stu-id="b9907-133">The corrected invoices with positive amounts belong to the previous period.</span></span> <span data-ttu-id="b9907-134">Последняя строка вычисляется как итоговая сумма первой итоговой строки, аннулированных счетов-фактур и исправленных счетов.</span><span class="sxs-lookup"><span data-stu-id="b9907-134">The last line is calculated as the sum of the amounts of the first total line, annulled tax invoices, and the corrected invoices.</span></span>

<span data-ttu-id="b9907-135">Обработка корректирующих документов для книги продаж аналогична обработке корректирующих документов для книги покупок.</span><span class="sxs-lookup"><span data-stu-id="b9907-135">Processing of corrective documents for sales book is similar to processing for purchases book with one difference.</span></span> <span data-ttu-id="b9907-136">Единственное различие заключается в том, что в дополнительных листах необходимо отражать номер и дату исходного счета-фактуры.</span><span class="sxs-lookup"><span data-stu-id="b9907-136">In additional sheets, the number and the date of initial factura must be reflected.</span></span>

#### <a name="to-create-a-correction-entry-for-posted-purchase-credit-memos"></a><span data-ttu-id="b9907-137">Создание корректирующей операции для учтенных кредит-нот покупки</span><span class="sxs-lookup"><span data-stu-id="b9907-137">To create a correction entry for posted purchase credit memos</span></span>

1. <span data-ttu-id="b9907-138">Создайте и учтите кредит-ноту покупки.</span><span class="sxs-lookup"><span data-stu-id="b9907-138">Create and post a purchase credit memo.</span></span>
2. <span data-ttu-id="b9907-139">Выберите вкладку **НДС**.</span><span class="sxs-lookup"><span data-stu-id="b9907-139">Choose the **VAT** tab.</span></span>
3. <span data-ttu-id="b9907-140">Выберите поле **Дополнительный лист книги НДС**.</span><span class="sxs-lookup"><span data-stu-id="b9907-140">Select the **Additional VAT Ledger Sheet** field.</span></span>
4. <span data-ttu-id="b9907-141">Заполните следующие поля.</span><span class="sxs-lookup"><span data-stu-id="b9907-141">Enter information in the following fields:</span></span>
   - <span data-ttu-id="b9907-142">**Дата скорректированного документа**</span><span class="sxs-lookup"><span data-stu-id="b9907-142">**Corrected Document Date**</span></span>
   - <span data-ttu-id="b9907-143">**Дата счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="b9907-143">**Vendor VAT Invoice Date**</span></span>
   - <span data-ttu-id="b9907-144">**Дата получения счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="b9907-144">**Vendor VAT Invoice Rcvd Date**</span></span>
   - <span data-ttu-id="b9907-145">**Счет-Фактура Но.**</span><span class="sxs-lookup"><span data-stu-id="b9907-145">**Vendor VAT Invoice No.**</span></span>

#### <a name="to-create-a-correction-entry-for-a-posted-purchase-invoice"></a><span data-ttu-id="b9907-146">Создание корректирующей операции для учтенного счета покупки</span><span class="sxs-lookup"><span data-stu-id="b9907-146">To create a correction entry for a posted purchase invoice</span></span>

1. <span data-ttu-id="b9907-147">Создайте и учтите счет покупки.</span><span class="sxs-lookup"><span data-stu-id="b9907-147">Create and post a purchase invoice.</span></span>

2. <span data-ttu-id="b9907-148">Выберите вкладку **НДС**.</span><span class="sxs-lookup"><span data-stu-id="b9907-148">Choose the **VAT** tab.</span></span>

3. <span data-ttu-id="b9907-149">Выберите поле **Дата скорректированного документа**.</span><span class="sxs-lookup"><span data-stu-id="b9907-149">Select the **Corrected Document Date** field.</span></span>

4. <span data-ttu-id="b9907-150">Заполните следующие поля.</span><span class="sxs-lookup"><span data-stu-id="b9907-150">Enter information in the following fields:</span></span>

   - <span data-ttu-id="b9907-151">**Дата счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="b9907-151">**Vendor VAT Invoice Date**</span></span>
   - <span data-ttu-id="b9907-152">**Дата получения счета-фактуры поставщика**</span><span class="sxs-lookup"><span data-stu-id="b9907-152">**Vendor VAT Invoice Rcvd. Date**</span></span>
   - <span data-ttu-id="b9907-153">**Счет-Фактура Но.**</span><span class="sxs-lookup"><span data-stu-id="b9907-153">**Vendor VAT Invoice No.**</span></span>

   > :speech_balloon: <span data-ttu-id="b9907-154">Примечание</span><span class="sxs-lookup"><span data-stu-id="b9907-154">Note</span></span>
   >
   > <span data-ttu-id="b9907-155">Также можно создать корректирующие документы в финансовом журнале.</span><span class="sxs-lookup"><span data-stu-id="b9907-155">You can also create corrective documents in the general journal.</span></span> <span data-ttu-id="b9907-156">Строки финансового журнала содержат все перечисленные выше поля.</span><span class="sxs-lookup"><span data-stu-id="b9907-156">General journal lines contain all the fields mentioned above.</span></span>

#### <a name="to-post-additional-vat"></a><span data-ttu-id="b9907-157">Учет дополнительного НДС</span><span class="sxs-lookup"><span data-stu-id="b9907-157">To post additional VAT</span></span>

1. <span data-ttu-id="b9907-158">В окне **Счет продажи** или **Кредит-нота** откройте вкладку **НДС**.</span><span class="sxs-lookup"><span data-stu-id="b9907-158">In the **Sales Invoice** window or the **Credit Memo** window, choose the **VAT** tab.</span></span>

2. <span data-ttu-id="b9907-159">Заполните поле **Учетный номер**.</span><span class="sxs-lookup"><span data-stu-id="b9907-159">Enter the **Posting No.**</span></span> <span data-ttu-id="b9907-160">.</span><span class="sxs-lookup"><span data-stu-id="b9907-160">field.</span></span>

   > :speech_balloon: <span data-ttu-id="b9907-161">Примечание</span><span class="sxs-lookup"><span data-stu-id="b9907-161">Note</span></span>
   >
   > <span data-ttu-id="b9907-162">Нельзя учесть счет с тем же номером, что и у исходного счета.</span><span class="sxs-lookup"><span data-stu-id="b9907-162">You cannot post an invoice with the same number as the initial invoice.</span></span> <span data-ttu-id="b9907-163">Необходимо добавить к исходному номеру еще один дополнительный символ.</span><span class="sxs-lookup"><span data-stu-id="b9907-163">You must use an extra symbol in addition to the initial number.</span></span>

3. <span data-ttu-id="b9907-164">Выберите поле **Дополнительный лист книги НДС**.</span><span class="sxs-lookup"><span data-stu-id="b9907-164">Select the **Additional VAT Ledger Sheet** field.</span></span>

4. <span data-ttu-id="b9907-165">Заполните поле **Дата скорректированного документа**.</span><span class="sxs-lookup"><span data-stu-id="b9907-165">Enter information in the **Corrected Document Date** field.</span></span>

5. <span data-ttu-id="b9907-166">В дополнительном листе поле **Дата Счета-Фактуры** отражает дату корректируемого документа.</span><span class="sxs-lookup"><span data-stu-id="b9907-166">In the additional sheet, the **Date of Facture** field reflects the corrected document date.</span></span>

## <a name="see-also"></a><span data-ttu-id="b9907-167">См. также</span><span class="sxs-lookup"><span data-stu-id="b9907-167">See Also</span></span>

[<span data-ttu-id="b9907-168">Книги НДС</span><span class="sxs-lookup"><span data-stu-id="b9907-168">VAT Ledgers</span></span>](VAT-Ledgers.md)
