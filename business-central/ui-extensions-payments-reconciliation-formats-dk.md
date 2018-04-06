---
title: "Использование расширения \"Платежи и выверки (DK)\" | Microsoft Docs"
description: "Это расширение облегчает экспорт файлов, форматированных в соответствии с банковскими требованиями к предоставляемым электронным документам."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, bank, formats
ms.date: 09/15/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: b345100f2ec89685855bfd8e630e3ef44506e86d
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---

# <a name="the-payments-and-reconciliations-dk-extension-for-microsoft-dynamics-for-business-central"></a><span data-ttu-id="e7ce1-103">Расширение платежей и выверки (DK) для Microsoft Dynamics for Business Central</span><span class="sxs-lookup"><span data-stu-id="e7ce1-103">The Payments and Reconciliations (DK) Extension for Microsoft Dynamics for Business Central</span></span>
<span data-ttu-id="e7ce1-104">Делайте быстрые платежи без ошибок, экспортируя файлы, форматированные специально для обмена документами с поставщиком или банком.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-104">Make fast, error-free payments by exporting files that are formatted specifically for exchanges with your vendor or bank.</span></span> <span data-ttu-id="e7ce1-105">Эти файлы ускоряют процессы платежей и выверки, а также устраняют ошибки, которые возможны при вводе информации вручную на веб-сайте банка.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-105">These files speed up the payment and reconciliation processes, and eliminate errors that can happen when you manually enter the information on a bank website.</span></span>  
  
<span data-ttu-id="e7ce1-106">Это расширение поддерживает форматы файлов для нескольких банках в Дании.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-106">This extension supports file formats for several Danish banks.</span></span> <span data-ttu-id="e7ce1-107">При экспорте информации о платеже в файл расширение упаковывает данные в формат, требуемый банком.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-107">When you export payment information to a file, the extension packages the data into the format that your bank requires.</span></span> <span data-ttu-id="e7ce1-108">Например, поддерживаются форматы Bankdata-V3, BEC, SDC и FIK, которые используются многими банками, а также некоторые более специализированные форматы для определенных банков, таких как Danske Bank и Nordea.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-108">For example, the formats include Bankdata-V3, BEC, SDC, and FIK, which many different banks use, and some that are more specialized for certain banks, for example, Danske Bank and Nordea.</span></span> <span data-ttu-id="e7ce1-109">Расширение также включает некоторые форматы для импорта и выверки банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-109">The extension also includes some formats for importing and reconciling bank statements.</span></span>  
  
> [!Note]
> <span data-ttu-id="e7ce1-110">Для использования расширения необходимо знать, какой формат требуется для поставщика или банка.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-110">To use the extension, you must know the format that your bank or vendor requires.</span></span> <span data-ttu-id="e7ce1-111">Некоторые банки или поставщики предоставляют эту информацию на своих веб-сайтах; однако может потребоваться связаться с их службой обслуживания клиентов для получения этой информации.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-111">Some banks or vendors provide this information on their websites; however, you might need to contact their customer service to get the information.</span></span>  
  
## <a name="supported-bank-formats"></a><span data-ttu-id="e7ce1-112">Поддерживаемые банковские форматы</span><span class="sxs-lookup"><span data-stu-id="e7ce1-112">Supported Bank Formats</span></span>
<span data-ttu-id="e7ce1-113">Это расширение может применять следующие форматы файлов платежей:</span><span class="sxs-lookup"><span data-stu-id="e7ce1-113">This extension can apply the following file formats for payment files:</span></span>  
  
* <span data-ttu-id="e7ce1-114">BANKDATA-V3</span><span class="sxs-lookup"><span data-stu-id="e7ce1-114">BANKDATA-V3</span></span>  
* <span data-ttu-id="e7ce1-115">BEC-INDLAND</span><span class="sxs-lookup"><span data-stu-id="e7ce1-115">BEC-INDLAND</span></span>  
* <span data-ttu-id="e7ce1-116">BEC-CSV</span><span class="sxs-lookup"><span data-stu-id="e7ce1-116">BEC-CSV</span></span>  
* <span data-ttu-id="e7ce1-117">DANSKEBANK-CMKV</span><span class="sxs-lookup"><span data-stu-id="e7ce1-117">DANSKEBANK-CMKV</span></span>  
* <span data-ttu-id="e7ce1-118">DANSKEBANK-CMKXKSX</span><span class="sxs-lookup"><span data-stu-id="e7ce1-118">DANSKEBANK-CMKXKSX</span></span>  
* <span data-ttu-id="e7ce1-119">DANSKEBANK</span><span class="sxs-lookup"><span data-stu-id="e7ce1-119">DANSKEBANK</span></span>  
* <span data-ttu-id="e7ce1-120">FIK71</span><span class="sxs-lookup"><span data-stu-id="e7ce1-120">FIK71</span></span>  
* <span data-ttu-id="e7ce1-121">NORDEA-ERHVERV-CSV</span><span class="sxs-lookup"><span data-stu-id="e7ce1-121">NORDEA-ERHVERV-CSV</span></span>  
* <span data-ttu-id="e7ce1-122">NORDEA</span><span class="sxs-lookup"><span data-stu-id="e7ce1-122">NORDEA</span></span>  
* <span data-ttu-id="e7ce1-123">NORDEA-UNITEL-V3</span><span class="sxs-lookup"><span data-stu-id="e7ce1-123">NORDEA-UNITEL-V3</span></span>  
* <span data-ttu-id="e7ce1-124">SDC</span><span class="sxs-lookup"><span data-stu-id="e7ce1-124">SDC</span></span>  
* <span data-ttu-id="e7ce1-125">SDC-CSV</span><span class="sxs-lookup"><span data-stu-id="e7ce1-125">SDC-CSV</span></span>  

## <a name="to-set-up-the-extension"></a><span data-ttu-id="e7ce1-126">Настройка расширения</span><span class="sxs-lookup"><span data-stu-id="e7ce1-126">To set up the extension</span></span>
<span data-ttu-id="e7ce1-127">Для начала работы нужно выполнить несколько шагов.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-127">There are a few steps to get started.</span></span>  
  
* <span data-ttu-id="e7ce1-128">Разрешите экспорт данных платежей.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-128">Allow payment data exports.</span></span> <span data-ttu-id="e7ce1-129">Чтобы защитить ваши данные, это действие не доступно сразу.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-129">To help protect your data, this is not readily available.</span></span>  
* <span data-ttu-id="e7ce1-130">Настройте покупки и расчеты с кредиторами таким образом, чтобы вам не требовались номера внешних документов в счетах.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-130">Set up purchase and payables so that you do not require external document numbers on invoices.</span></span> <span data-ttu-id="e7ce1-131">При необходимости можно использовать ссылочный номер для ссылки на определенный счет.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-131">If needed, you can use the reference number to refer to a specific invoice.</span></span>  
* <span data-ttu-id="e7ce1-132">Укажите способ оплаты для каждого поставщика.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-132">Specify the payment method for each vendor.</span></span> <span data-ttu-id="e7ce1-133">Способы платежа определяют, как вы оплачивайте счета от поставщика.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-133">Payment methods define how you pay invoices from the vendor.</span></span> <span data-ttu-id="e7ce1-134">Например, банк, наличные, чек или счет.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-134">For example, Bank, Cash, Check, or Account.</span></span>  
* <span data-ttu-id="e7ce1-135">Укажите тип формата для использования для каждого из ваших банковских счетов.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-135">Specify the type of format to use for each of your bank accounts.</span></span> <span data-ttu-id="e7ce1-136">Например, NORDEA, DANSKEBANK, SDC и т. д.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-136">For example, NORDEA, DANSKEBANK, SDC, and so on.</span></span>  
  
<span data-ttu-id="e7ce1-137">Кроме того, необходимо назначить поставщиков группам **Общая бизнес-группа** и **Учетная группа поставщика** внутри страны.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-137">Additionally, you must assign vendors to a domestic **Gen. Bus. Posting Group** and a **Vendor Posting Group**.</span></span> <span data-ttu-id="e7ce1-138">Настройка страны/региона для поставщика должна быть Дания (DK).</span><span class="sxs-lookup"><span data-stu-id="e7ce1-138">The Country/Region setting for the vendor must be Denmark (DK).</span></span> <span data-ttu-id="e7ce1-139">Дополнительные сведения см. в разделе [Настройка учетных групп](finance-posting-groups.md).</span><span class="sxs-lookup"><span data-stu-id="e7ce1-139">For more information, see [Setting Up Posting Groups](finance-posting-groups.md).</span></span>  
  
### <a name="to-allow-included365finincludesd365finmdmd-to-export-payment-data"></a><span data-ttu-id="e7ce1-140">Чтобы разрешить [!INCLUDE[d365fin](includes/d365fin_md.md)] экспортировать данные платежей</span><span class="sxs-lookup"><span data-stu-id="e7ce1-140">To allow [!INCLUDE[d365fin](includes/d365fin_md.md)] to export payment data</span></span>
1. <span data-ttu-id="e7ce1-141">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал платежей**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7ce1-142">В окне **Изменение журнала платежей** выберите пакет **Банк**.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-142">In the **Edit Payment Journal** window, choose the **Bank** batch.</span></span>  
3. <span data-ttu-id="e7ce1-143">Установите флажок **Разрешить экспорт платежей**.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-143">Choose the **Allow Payment Export** check box.</span></span>  

### <a name="to-specify-a-payment-method-for-a-vendor"></a><span data-ttu-id="e7ce1-144">Указание способ оплаты для поставщика</span><span class="sxs-lookup"><span data-stu-id="e7ce1-144">To specify a payment method for a vendor</span></span>
<span data-ttu-id="e7ce1-145">В следующей таблице перечислены сочетания способов оплаты FIK и GIRO, которые поддерживает [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e7ce1-145">The following table shows the combinations of FIK and GIRO payment methods that [!INCLUDE[d365fin](includes/d365fin_md.md)] supports.</span></span>

||<span data-ttu-id="e7ce1-146">Тип 01</span><span class="sxs-lookup"><span data-stu-id="e7ce1-146">Type 01</span></span> | <span data-ttu-id="e7ce1-147">Тип 04</span><span class="sxs-lookup"><span data-stu-id="e7ce1-147">Type 04</span></span> | <span data-ttu-id="e7ce1-148">Тип 71</span><span class="sxs-lookup"><span data-stu-id="e7ce1-148">Type 71</span></span> | <span data-ttu-id="e7ce1-149">Тип 73</span><span class="sxs-lookup"><span data-stu-id="e7ce1-149">Type 73</span></span> |
|----|---|---|---|---|
|<span data-ttu-id="e7ce1-150">Номер жиросчета или номер кредитора FIK?</span><span class="sxs-lookup"><span data-stu-id="e7ce1-150">Giro Account No. or FIK Creditor No.?</span></span> | <span data-ttu-id="e7ce1-151">Номер жиросчета</span><span class="sxs-lookup"><span data-stu-id="e7ce1-151">Giro Account No.</span></span> | <span data-ttu-id="e7ce1-152">Номер жиросчета</span><span class="sxs-lookup"><span data-stu-id="e7ce1-152">Giro Account No.</span></span> | <span data-ttu-id="e7ce1-153">Номер кредитора FIK</span><span class="sxs-lookup"><span data-stu-id="e7ce1-153">FIK Creditor No.</span></span> | <span data-ttu-id="e7ce1-154">Номер кредитора FIK</span><span class="sxs-lookup"><span data-stu-id="e7ce1-154">FIK Creditor No.</span></span>|
|<span data-ttu-id="e7ce1-155">Допускает сообщение получателю?</span><span class="sxs-lookup"><span data-stu-id="e7ce1-155">Allows Message to Recipient?</span></span> | <span data-ttu-id="e7ce1-156">Да</span><span class="sxs-lookup"><span data-stu-id="e7ce1-156">Yes</span></span> |<span data-ttu-id="e7ce1-157">Нет</span><span class="sxs-lookup"><span data-stu-id="e7ce1-157">No</span></span> |<span data-ttu-id="e7ce1-158">Нет</span><span class="sxs-lookup"><span data-stu-id="e7ce1-158">No</span></span> | <span data-ttu-id="e7ce1-159">Да</span><span class="sxs-lookup"><span data-stu-id="e7ce1-159">Yes</span></span> |
|<span data-ttu-id="e7ce1-160">Содержит ссылочный номер платежа?</span><span class="sxs-lookup"><span data-stu-id="e7ce1-160">Contains Payment Reference number?</span></span> | <span data-ttu-id="e7ce1-161">Нет</span><span class="sxs-lookup"><span data-stu-id="e7ce1-161">No</span></span> | <span data-ttu-id="e7ce1-162">Да, 16 цифр.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-162">Yes, 16 digits.</span></span> | <span data-ttu-id="e7ce1-163">Да, 15 цифр.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-163">Yes, 15 digits.</span></span> | <span data-ttu-id="e7ce1-164">Нет</span><span class="sxs-lookup"><span data-stu-id="e7ce1-164">No</span></span>|

1. <span data-ttu-id="e7ce1-165">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Поставщики**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-165">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7ce1-166">Откройте карточку, разверните вкладку **Платежи**, в поле **Способ платежа** выберите способ платежа.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-166">Open the card, expand the **Payments** tab, in the **Payment Method** field choose the payment method.</span></span>  
3. <span data-ttu-id="e7ce1-167">В зависимости от выбора следует заполнить другие поля.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-167">Depending on your selection, you must complete other fields.</span></span> <span data-ttu-id="e7ce1-168">См. таблицу выше для описания комбинаций.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-168">See the table above for a description of the combinations.</span></span>  

### <a name="to-specify-the-format-to-use-for-a-bank-account"></a><span data-ttu-id="e7ce1-169">Указание формата для использования для банковского счета</span><span class="sxs-lookup"><span data-stu-id="e7ce1-169">To specify the format to use for a bank account</span></span>
1. <span data-ttu-id="e7ce1-170">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Банковские счета**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-170">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7ce1-171">Откройте карточку для банковского счета.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-171">Open the card for the bank account.</span></span>  
3. <span data-ttu-id="e7ce1-172">В поле **Формат экспорта платежей** выберите формат для экспорта файла.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-172">In the **Payment Export Format** field, choose the format for your export file.</span></span>  

## <a name="choosing-the-fik-or-giro-payment-information-for-vendor-invoices"></a><span data-ttu-id="e7ce1-173">Выбор информации о платеже FIK или Жиро для счета поставщика</span><span class="sxs-lookup"><span data-stu-id="e7ce1-173">Choosing the FIK or Giro payment information for vendor invoices</span></span>
1. <span data-ttu-id="e7ce1-174">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета покупки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-174">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7ce1-175">Выберите поставщика,</span><span class="sxs-lookup"><span data-stu-id="e7ce1-175">Choose the vendor.</span></span> <span data-ttu-id="e7ce1-176">Не забудьте, это должен быть датский поставщик с адресом в Дании.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-176">Remember, this must be a Danish vendor with an address in Denmark.</span></span>
3. <span data-ttu-id="e7ce1-177">Создайте счет.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-177">Create an invoice.</span></span> <span data-ttu-id="e7ce1-178">Поля **Метод платежа** и **Код поставщика** будут заполнены на основе настроек в карточке поставщика.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-178">The **Payment Method** and **Vendor Number** fields are filled in based on settings on the Vendor card.</span></span> <span data-ttu-id="e7ce1-179">При необходимости их можно изменить.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-179">You can change them if you want.</span></span>
4. <span data-ttu-id="e7ce1-180">В поле **Ссылка на оплату** введите 15-значный номер из счета поставщика.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-180">In the **Payment Reference** field, enter the 15-digit number from the vendor invoice.</span></span>  
  
    > [!Tip]
    > <span data-ttu-id="e7ce1-181">Необходимо ввести только 11 последних цифр этого номера.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-181">You only have to add the last 11 digits of the number.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="e7ce1-182"> добавить четыре нуля в начало номера.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-182"> will add four zeros to the beginning of the number.</span></span>  
  
5. <span data-ttu-id="e7ce1-183">Учет счета.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-183">Post the invoice.</span></span>

## <a name="to-use-the-extension-to-export-payment-data"></a><span data-ttu-id="e7ce1-184">Использование расширения для экспорта данных платежа</span><span class="sxs-lookup"><span data-stu-id="e7ce1-184">To use the extension to export payment data</span></span>
1. <span data-ttu-id="e7ce1-185">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы платежей**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-185">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7ce1-186">Выберите действие **Журналы предлож. оплаты поставщикам**.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-186">Choose the **Suggest Vendor Payment Journals** action.</span></span>  
  
    > [!Tip]
    > <span data-ttu-id="e7ce1-187">Если нужно экспортировать только определенные платежи, следует использовать параметры для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-187">If you want to export only specific payments, use the options for filtering the data.</span></span>  
  
3. <span data-ttu-id="e7ce1-188">При необходимости можно добавить фильтры, чтобы экспортировать только определенные платежи.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-188">If needed, you can add filters to export only specific payments.</span></span>  
4. <span data-ttu-id="e7ce1-189">В поле **Тип банковского платежа** выберите **Электронные платежи**.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-189">In the **Bank Payment Type** field, choose **Electronic Payment**.</span></span>  
5. <span data-ttu-id="e7ce1-190">Выберите действие **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="e7ce1-190">Choose the **Export** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e7ce1-191">См. также</span><span class="sxs-lookup"><span data-stu-id="e7ce1-191">See also</span></span>
<span data-ttu-id="e7ce1-192">[Настройка Business Central для [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="e7ce1-192">[Customizing Business Central for [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="e7ce1-193">Создание операций погашения прямого дебета SEPA и их экспорт в файл банка</span><span class="sxs-lookup"><span data-stu-id="e7ce1-193">Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)  
[<span data-ttu-id="e7ce1-194">Настройка прямого дебетования SEPA</span><span class="sxs-lookup"><span data-stu-id="e7ce1-194">Set Up SEPA Direct Debit</span></span>](finance-how-to-set-up-sepa-direct-debit.md)  
[<span data-ttu-id="e7ce1-195">Учет платежной квитанции по прямому дебету SEPA</span><span class="sxs-lookup"><span data-stu-id="e7ce1-195">Post SEPA Direct Debit Payment Receipts</span></span>](finance-how-to-post-sepa-direct-debit-payment-receipts.md)  
[<span data-ttu-id="e7ce1-196">Сбор платежей с прямым дебетом SEPA</span><span class="sxs-lookup"><span data-stu-id="e7ce1-196">Collecting Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)  
[<span data-ttu-id="e7ce1-197">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="e7ce1-197">Working with General Journals</span></span>](ui-work-general-journals.md)  





