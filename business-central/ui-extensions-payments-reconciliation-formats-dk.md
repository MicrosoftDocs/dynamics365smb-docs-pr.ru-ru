---
title: Использование расширения "Платежи и выверки (DK)" | Документация Майкрософт
description: Это расширение облегчает экспорт файлов, форматированных в соответствии с банковскими требованиями к предоставляемым электронным документам.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, bank, formats
ms.date: 06/19/2020
ms.author: bholtorf
ms.openlocfilehash: 7e8a56492c1c848f4f3b371e1411c11f159c3cf3
ms.sourcegitcommit: 6200a08e91d507bab01d1d5b805fe8ea3f44a58a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2020
ms.locfileid: "3496754"
---
# <a name="the-payments-and-reconciliations-dk-extension"></a><span data-ttu-id="d4c35-103">Расширение платежей и выверки (DK)</span><span class="sxs-lookup"><span data-stu-id="d4c35-103">The Payments and Reconciliations (DK) Extension</span></span>

<span data-ttu-id="d4c35-104">Делайте быстрые платежи без ошибок, экспортируя файлы, форматированные специально для обмена документами с поставщиком или банком.</span><span class="sxs-lookup"><span data-stu-id="d4c35-104">Make fast, error-free payments by exporting files that are formatted specifically for exchanges with your vendor or bank.</span></span> <span data-ttu-id="d4c35-105">Эти файлы ускоряют процессы платежей и выверки, а также устраняют ошибки, которые возможны при вводе информации вручную на веб-сайте банка.</span><span class="sxs-lookup"><span data-stu-id="d4c35-105">These files speed up the payment and reconciliation processes, and eliminate errors that can happen when you manually enter the information on a bank website.</span></span>  

<span data-ttu-id="d4c35-106">Это расширение поддерживает форматы файлов для нескольких банках в Дании.</span><span class="sxs-lookup"><span data-stu-id="d4c35-106">This extension supports file formats for several Danish banks.</span></span> <span data-ttu-id="d4c35-107">При экспорте информации о платеже в файл расширение упаковывает данные в формат, требуемый банком.</span><span class="sxs-lookup"><span data-stu-id="d4c35-107">When you export payment information to a file, the extension packages the data into the format that your bank requires.</span></span> <span data-ttu-id="d4c35-108">Например, поддерживаются форматы Bankdata-V3, BEC, SDC и FIK, которые используются многими банками, а также некоторые более специализированные форматы для определенных банков, таких как Danske Bank и Nordea.</span><span class="sxs-lookup"><span data-stu-id="d4c35-108">For example, the formats include Bankdata-V3, BEC, SDC, and FIK, which many different banks use, and some that are more specialized for certain banks, for example, Danske Bank and Nordea.</span></span> <span data-ttu-id="d4c35-109">Расширение также включает некоторые форматы для импорта и выверки банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="d4c35-109">The extension also includes some formats for importing and reconciling bank statements.</span></span>  

> [!Note]
> <span data-ttu-id="d4c35-110">Для использования расширения необходимо знать, какой формат требуется для поставщика или банка.</span><span class="sxs-lookup"><span data-stu-id="d4c35-110">To use the extension, you must know the format that your bank or vendor requires.</span></span> <span data-ttu-id="d4c35-111">Некоторые банки или поставщики предоставляют эту информацию на своих веб-сайтах; однако может потребоваться связаться с их службой обслуживания клиентов для получения этой информации.</span><span class="sxs-lookup"><span data-stu-id="d4c35-111">Some banks or vendors provide this information on their websites; however, you might need to contact their customer service to get the information.</span></span>  

## <a name="supported-bank-formats"></a><span data-ttu-id="d4c35-112">Поддерживаемые банковские форматы</span><span class="sxs-lookup"><span data-stu-id="d4c35-112">Supported Bank Formats</span></span>
<span data-ttu-id="d4c35-113">Это расширение может применять следующие форматы файлов платежей:</span><span class="sxs-lookup"><span data-stu-id="d4c35-113">This extension can apply the following file formats for payment files:</span></span>  

* <span data-ttu-id="d4c35-114">BANKDATA-V3</span><span class="sxs-lookup"><span data-stu-id="d4c35-114">BANKDATA-V3</span></span>  
* <span data-ttu-id="d4c35-115">BEC-INDLAND</span><span class="sxs-lookup"><span data-stu-id="d4c35-115">BEC-INDLAND</span></span>  
* <span data-ttu-id="d4c35-116">BEC-CSV</span><span class="sxs-lookup"><span data-stu-id="d4c35-116">BEC-CSV</span></span>  
* <span data-ttu-id="d4c35-117">DANSKEBANK-CMKV</span><span class="sxs-lookup"><span data-stu-id="d4c35-117">DANSKEBANK-CMKV</span></span>  
* <span data-ttu-id="d4c35-118">DANSKEBANK-CMKXKSX</span><span class="sxs-lookup"><span data-stu-id="d4c35-118">DANSKEBANK-CMKXKSX</span></span>  
* <span data-ttu-id="d4c35-119">DANSKEBANK</span><span class="sxs-lookup"><span data-stu-id="d4c35-119">DANSKEBANK</span></span>  
* <span data-ttu-id="d4c35-120">FIK71</span><span class="sxs-lookup"><span data-stu-id="d4c35-120">FIK71</span></span>  
* <span data-ttu-id="d4c35-121">NORDEA-ERHVERV-CSV</span><span class="sxs-lookup"><span data-stu-id="d4c35-121">NORDEA-ERHVERV-CSV</span></span>  
* <span data-ttu-id="d4c35-122">NORDEA</span><span class="sxs-lookup"><span data-stu-id="d4c35-122">NORDEA</span></span>  
* <span data-ttu-id="d4c35-123">NORDEA-UNITEL-V3</span><span class="sxs-lookup"><span data-stu-id="d4c35-123">NORDEA-UNITEL-V3</span></span>  
* <span data-ttu-id="d4c35-124">SDC</span><span class="sxs-lookup"><span data-stu-id="d4c35-124">SDC</span></span>  
* <span data-ttu-id="d4c35-125">SDC-CSV</span><span class="sxs-lookup"><span data-stu-id="d4c35-125">SDC-CSV</span></span>  

## <a name="to-set-up-the-extension"></a><span data-ttu-id="d4c35-126">Настройка расширения</span><span class="sxs-lookup"><span data-stu-id="d4c35-126">To set up the extension</span></span>

<span data-ttu-id="d4c35-127">Для начала работы нужно выполнить несколько шагов.</span><span class="sxs-lookup"><span data-stu-id="d4c35-127">There are a few steps to get started.</span></span>  

* <span data-ttu-id="d4c35-128">Разрешите экспорт данных платежей.</span><span class="sxs-lookup"><span data-stu-id="d4c35-128">Allow payment data exports.</span></span> <span data-ttu-id="d4c35-129">Чтобы защитить ваши данные, это действие не доступно сразу.</span><span class="sxs-lookup"><span data-stu-id="d4c35-129">To help protect your data, this is not readily available.</span></span>  
* <span data-ttu-id="d4c35-130">Настройте покупки и расчеты с кредиторами таким образом, чтобы вам не требовались номера внешних документов в счетах.</span><span class="sxs-lookup"><span data-stu-id="d4c35-130">Set up purchase and payables so that you do not require external document numbers on invoices.</span></span> <span data-ttu-id="d4c35-131">При необходимости можно использовать ссылочный номер для ссылки на определенный счет.</span><span class="sxs-lookup"><span data-stu-id="d4c35-131">If needed, you can use the reference number to refer to a specific invoice.</span></span>  
* <span data-ttu-id="d4c35-132">Укажите способ оплаты для каждого поставщика.</span><span class="sxs-lookup"><span data-stu-id="d4c35-132">Specify the payment method for each vendor.</span></span> <span data-ttu-id="d4c35-133">Способы платежа определяют, как вы оплачивайте счета от поставщика.</span><span class="sxs-lookup"><span data-stu-id="d4c35-133">Payment methods define how you pay invoices from the vendor.</span></span> <span data-ttu-id="d4c35-134">Например, банк, наличные, чек или счет.</span><span class="sxs-lookup"><span data-stu-id="d4c35-134">For example, Bank, Cash, Check, or Account.</span></span>  
* <span data-ttu-id="d4c35-135">Укажите тип формата для использования для каждого из ваших банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="d4c35-135">Specify the type of format to use for each of your bank accounts.</span></span> <span data-ttu-id="d4c35-136">Например, NORDEA, DANSKEBANK, SDC и т. д.</span><span class="sxs-lookup"><span data-stu-id="d4c35-136">For example, NORDEA, DANSKEBANK, SDC, and so on.</span></span>  

<span data-ttu-id="d4c35-137">Кроме того, необходимо назначить поставщиков группам **Общая бизнес-группа** и **Учетная группа поставщика** внутри страны.</span><span class="sxs-lookup"><span data-stu-id="d4c35-137">Additionally, you must assign vendors to a domestic **Gen. Bus. Posting Group** and a **Vendor Posting Group**.</span></span> <span data-ttu-id="d4c35-138">Настройка страны/региона для поставщика должна быть Дания (DK).</span><span class="sxs-lookup"><span data-stu-id="d4c35-138">The Country/Region setting for the vendor must be Denmark (DK).</span></span> <span data-ttu-id="d4c35-139">Дополнительные сведения см. в разделе [Настройка учетных групп](finance-posting-groups.md).</span><span class="sxs-lookup"><span data-stu-id="d4c35-139">For more information, see [Setting Up Posting Groups](finance-posting-groups.md).</span></span>  

### <a name="to-allow-d365fin-to-export-payment-data"></a><span data-ttu-id="d4c35-140">Чтобы разрешить [!INCLUDE[d365fin](includes/d365fin_md.md)] экспортировать данные платежей</span><span class="sxs-lookup"><span data-stu-id="d4c35-140">To allow [!INCLUDE[d365fin](includes/d365fin_md.md)] to export payment data</span></span>

1. <span data-ttu-id="d4c35-141">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал платежей**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d4c35-141">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d4c35-142">На странице **Изменение журнала платежей** выберите пакет **Банк**.</span><span class="sxs-lookup"><span data-stu-id="d4c35-142">On the **Edit Payment Journal** page, choose the **Bank** batch.</span></span>  
3. <span data-ttu-id="d4c35-143">Установите флажок **Разрешить экспорт платежей**.</span><span class="sxs-lookup"><span data-stu-id="d4c35-143">Choose the **Allow Payment Export** check box.</span></span>  

### <a name="to-specify-a-payment-method-for-a-vendor"></a><span data-ttu-id="d4c35-144">Указание способ оплаты для поставщика</span><span class="sxs-lookup"><span data-stu-id="d4c35-144">To specify a payment method for a vendor</span></span>

<span data-ttu-id="d4c35-145">В следующей таблице перечислены сочетания способов оплаты FIK и GIRO, которые поддерживает [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d4c35-145">The following table shows the combinations of FIK and GIRO payment methods that [!INCLUDE[d365fin](includes/d365fin_md.md)] supports.</span></span>

|<span data-ttu-id="d4c35-146">Комбинация</span><span class="sxs-lookup"><span data-stu-id="d4c35-146">Combination</span></span>|<span data-ttu-id="d4c35-147">Тип 01</span><span class="sxs-lookup"><span data-stu-id="d4c35-147">Type 01</span></span> | <span data-ttu-id="d4c35-148">Тип 04</span><span class="sxs-lookup"><span data-stu-id="d4c35-148">Type 04</span></span> | <span data-ttu-id="d4c35-149">Тип 71</span><span class="sxs-lookup"><span data-stu-id="d4c35-149">Type 71</span></span> | <span data-ttu-id="d4c35-150">Тип 73</span><span class="sxs-lookup"><span data-stu-id="d4c35-150">Type 73</span></span> |
|----|--------|---------|---------|---------|
|<span data-ttu-id="d4c35-151">Номер жиросчета или номер кредитора FIK?</span><span class="sxs-lookup"><span data-stu-id="d4c35-151">Giro Account No. or FIK Creditor No.?</span></span> | <span data-ttu-id="d4c35-152">Номер жиросчета</span><span class="sxs-lookup"><span data-stu-id="d4c35-152">Giro Account No.</span></span> | <span data-ttu-id="d4c35-153">Номер жиросчета</span><span class="sxs-lookup"><span data-stu-id="d4c35-153">Giro Account No.</span></span> | <span data-ttu-id="d4c35-154">Номер кредитора FIK</span><span class="sxs-lookup"><span data-stu-id="d4c35-154">FIK Creditor No.</span></span> | <span data-ttu-id="d4c35-155">Номер кредитора FIK</span><span class="sxs-lookup"><span data-stu-id="d4c35-155">FIK Creditor No.</span></span>|
|<span data-ttu-id="d4c35-156">Допускает сообщение получателю?</span><span class="sxs-lookup"><span data-stu-id="d4c35-156">Allows Message to Recipient?</span></span> | <span data-ttu-id="d4c35-157">Да</span><span class="sxs-lookup"><span data-stu-id="d4c35-157">Yes</span></span> |<span data-ttu-id="d4c35-158">Нет</span><span class="sxs-lookup"><span data-stu-id="d4c35-158">No</span></span> |<span data-ttu-id="d4c35-159">Нет</span><span class="sxs-lookup"><span data-stu-id="d4c35-159">No</span></span> | <span data-ttu-id="d4c35-160">Да</span><span class="sxs-lookup"><span data-stu-id="d4c35-160">Yes</span></span> |
|<span data-ttu-id="d4c35-161">Содержит ссылочный номер платежа?</span><span class="sxs-lookup"><span data-stu-id="d4c35-161">Contains Payment Reference number?</span></span> | <span data-ttu-id="d4c35-162">Нет</span><span class="sxs-lookup"><span data-stu-id="d4c35-162">No</span></span> | <span data-ttu-id="d4c35-163">Да, 16 цифр.</span><span class="sxs-lookup"><span data-stu-id="d4c35-163">Yes, 16 digits.</span></span> | <span data-ttu-id="d4c35-164">Да, 15 цифр.</span><span class="sxs-lookup"><span data-stu-id="d4c35-164">Yes, 15 digits.</span></span> | <span data-ttu-id="d4c35-165">Нет</span><span class="sxs-lookup"><span data-stu-id="d4c35-165">No</span></span>|

1. <span data-ttu-id="d4c35-166">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Поставщики**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d4c35-166">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d4c35-167">Откройте карточку, разверните вкладку **Платежи**, в поле **Способ платежа** выберите способ платежа.</span><span class="sxs-lookup"><span data-stu-id="d4c35-167">Open the card, expand the **Payments** tab, in the **Payment Method** field choose the payment method.</span></span>  
3. <span data-ttu-id="d4c35-168">В зависимости от выбора следует заполнить другие поля.</span><span class="sxs-lookup"><span data-stu-id="d4c35-168">Depending on your selection, you must complete other fields.</span></span> <span data-ttu-id="d4c35-169">См. таблицу выше для описания комбинаций.</span><span class="sxs-lookup"><span data-stu-id="d4c35-169">See the table above for a description of the combinations.</span></span>  

### <a name="to-specify-the-format-to-use-for-a-bank-account"></a><span data-ttu-id="d4c35-170">Указание формата для использования для банковского счета</span><span class="sxs-lookup"><span data-stu-id="d4c35-170">To specify the format to use for a bank account</span></span>

1. <span data-ttu-id="d4c35-171">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d4c35-171">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d4c35-172">Откройте карточку для банковского счета.</span><span class="sxs-lookup"><span data-stu-id="d4c35-172">Open the card for the bank account.</span></span>  
3. <span data-ttu-id="d4c35-173">В поле **Формат экспорта платежей** выберите формат для экспорта файла.</span><span class="sxs-lookup"><span data-stu-id="d4c35-173">In the **Payment Export Format** field, choose the format for your export file.</span></span>  

## <a name="choosing-the-fik-or-giro-payment-information-for-vendor-invoices"></a><span data-ttu-id="d4c35-174">Выбор информации о платеже FIK или Жиро для счета поставщика</span><span class="sxs-lookup"><span data-stu-id="d4c35-174">Choosing the FIK or Giro payment information for vendor invoices</span></span>

1. <span data-ttu-id="d4c35-175">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d4c35-175">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="d4c35-176">Выберите поставщика,</span><span class="sxs-lookup"><span data-stu-id="d4c35-176">Choose the vendor.</span></span> <span data-ttu-id="d4c35-177">Не забудьте, это должен быть датский поставщик с адресом в Дании.</span><span class="sxs-lookup"><span data-stu-id="d4c35-177">Remember, this must be a Danish vendor with an address in Denmark.</span></span>
3. <span data-ttu-id="d4c35-178">Создайте счет.</span><span class="sxs-lookup"><span data-stu-id="d4c35-178">Create an invoice.</span></span> <span data-ttu-id="d4c35-179">Поля **Метод платежа** и **Код поставщика** будут заполнены на основе настроек в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="d4c35-179">The **Payment Method** and **Vendor Number** fields are filled in based on settings on the Vendor card.</span></span> <span data-ttu-id="d4c35-180">При необходимости их можно изменить.</span><span class="sxs-lookup"><span data-stu-id="d4c35-180">You can change them if you want.</span></span>
4. <span data-ttu-id="d4c35-181">В поле **Ссылка на оплату** введите 15-значный номер из счета поставщика.</span><span class="sxs-lookup"><span data-stu-id="d4c35-181">In the **Payment Reference** field, enter the 15-digit number from the vendor invoice.</span></span>  

    > [!Tip]
    > <span data-ttu-id="d4c35-182">Необходимо ввести только 11 последних цифр этого номера.</span><span class="sxs-lookup"><span data-stu-id="d4c35-182">You only have to add the last 11 digits of the number.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="d4c35-183">добавить четыре нуля в начало номера.</span><span class="sxs-lookup"><span data-stu-id="d4c35-183">will add four zeros to the beginning of the number.</span></span>  

5. <span data-ttu-id="d4c35-184">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="d4c35-184">Post the invoice.</span></span>

## <a name="to-use-the-extension-to-export-payment-data"></a><span data-ttu-id="d4c35-185">Использование расширения для экспорта данных платежа</span><span class="sxs-lookup"><span data-stu-id="d4c35-185">To use the extension to export payment data</span></span>

1. <span data-ttu-id="d4c35-186">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы платежей**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d4c35-186">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d4c35-187">Выберите действие **Журналы предлож. оплаты поставщикам**.</span><span class="sxs-lookup"><span data-stu-id="d4c35-187">Choose the **Suggest Vendor Payment Journals** action.</span></span>  

    > [!Tip]
    > <span data-ttu-id="d4c35-188">Если нужно экспортировать только определенные платежи, следует использовать параметры для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="d4c35-188">If you want to export only specific payments, use the options for filtering the data.</span></span>  

3. <span data-ttu-id="d4c35-189">При необходимости можно добавить фильтры, чтобы экспортировать только определенные платежи.</span><span class="sxs-lookup"><span data-stu-id="d4c35-189">If needed, you can add filters to export only specific payments.</span></span>  
4. <span data-ttu-id="d4c35-190">В поле **Тип банковского платежа** выберите **Электронные платежи**.</span><span class="sxs-lookup"><span data-stu-id="d4c35-190">In the **Bank Payment Type** field, choose **Electronic Payment**.</span></span>  
5. <span data-ttu-id="d4c35-191">Выберите действие **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="d4c35-191">Choose the **Export** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d4c35-192">См. также</span><span class="sxs-lookup"><span data-stu-id="d4c35-192">See also</span></span>

<span data-ttu-id="d4c35-193">[Настройка Business Central для [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="d4c35-193">[Customizing Business Central for [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="d4c35-194">Сбор платежей с прямым дебетом SEPA</span><span class="sxs-lookup"><span data-stu-id="d4c35-194">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)  
[<span data-ttu-id="d4c35-195">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="d4c35-195">Working with General Journals</span></span>](ui-work-general-journals.md)  
