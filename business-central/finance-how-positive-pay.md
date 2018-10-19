---
title: "Экспорт файлов Positive Pay | Документы Майкрософт"
description: "Вы можете гарантировать, чтобы банк выполнял клиринг только проверенных платежных документов и сумм путем экспорта файла Positive Pay, содержащего сведения о поставщике и платеже."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: dc63da7f3363ef45028a0b185c27aa468e02db6d
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="export-a-positive-pay-file"></a><span data-ttu-id="d983f-103">Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="d983f-103">Export a Positive Pay File</span></span>
<span data-ttu-id="d983f-104">Чтобы гарантировать, чтобы банк выполнял клиринг только по проверенным платежным документам и суммам, можно экспортировать файл Positive Pay, содержащий информацию о поставщике, номер платежного документа, сумму платежа, который можно затем переслать в банк для справки при обработке платежей.</span><span class="sxs-lookup"><span data-stu-id="d983f-104">To make sure that your bank only clears validated checks and amounts, you can export a Positive Pay file that contains vendor information, check number, and payment amount, which you send to the bank for reference when you process payments.</span></span>

<span data-ttu-id="d983f-105">Программа [!INCLUDE[d365fin](includes/d365fin_md.md)] предварительно настроена для поддержки файлов Positive Pay оплаты для банков Bank of America и City Bank.</span><span class="sxs-lookup"><span data-stu-id="d983f-105">[!INCLUDE[d365fin](includes/d365fin_md.md)] is preconfigured to support Positive Pay files for Bank of America and City Bank.</span></span>

## <a name="to-set-up-a-bank-account-for-positive-pay"></a><span data-ttu-id="d983f-106">Настройка банковского счета для Positive Pay</span><span class="sxs-lookup"><span data-stu-id="d983f-106">To set up a bank account for Positive Pay</span></span>
1. <span data-ttu-id="d983f-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d983f-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="d983f-108">Откройте карточку банка, для которого требуется использовать Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="d983f-108">Open the card for the bank that you want to use Positive Pay for.</span></span>
3. <span data-ttu-id="d983f-109">В поле **Код экспорта Positive Pay** введите POSPAYBANK.</span><span class="sxs-lookup"><span data-stu-id="d983f-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span></span>
4. <span data-ttu-id="d983f-110">Закройте данное окно.</span><span class="sxs-lookup"><span data-stu-id="d983f-110">Close the window.</span></span>

## <a name="to-export-a-positive-pay-file"></a><span data-ttu-id="d983f-111">Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="d983f-111">To export a Positive Pay file</span></span>
1. <span data-ttu-id="d983f-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d983f-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="d983f-113">Выберите банковский счет, для которого необходимо экспортировать файл Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="d983f-113">Select the bank account that you want to export a Positive Pay file for.</span></span>
3. <span data-ttu-id="d983f-114">Выберите действие **Экспорт Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="d983f-114">Choose **Positive Pay Export** action.</span></span>

    <span data-ttu-id="d983f-115">Откроется окно **Экспорт Positive Pay**, в котором отобразятся платежи, внесенные на банковский счет с даты последней отправки, как показано в полях **Дата последней отправки** и **Время последней отправки**.</span><span class="sxs-lookup"><span data-stu-id="d983f-115">The **Positive Pay Export** window opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span></span>
4. <span data-ttu-id="d983f-116">В поле **Граничная дата отправки** укажите дату, до которой платежи не включаются в экспортированный файл.</span><span class="sxs-lookup"><span data-stu-id="d983f-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span></span>
5. <span data-ttu-id="d983f-117">Выберите действие **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="d983f-117">Choose the **Export** action.</span></span>
6. <span data-ttu-id="d983f-118">В окне **Экспорт файла** нажмите кнопку **Сохранить**, а затем сохраните файл в удобное расположение.</span><span class="sxs-lookup"><span data-stu-id="d983f-118">In the **Export File** window, choose the **Save** button, and then save the file to a convenient location.</span></span>
7. <span data-ttu-id="d983f-119">Отправьте файл на сайт электронного банка.</span><span class="sxs-lookup"><span data-stu-id="d983f-119">Upload the file to your electronic bank site.</span></span>
8. <span data-ttu-id="d983f-120">Запишите или скопируйте номер подтверждения, отображаемый после успешной отправки файла.</span><span class="sxs-lookup"><span data-stu-id="d983f-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span></span>

<span data-ttu-id="d983f-121">Просмотр экспортированных записей Positive Pay</span><span class="sxs-lookup"><span data-stu-id="d983f-121">To view exported Positive Pay records</span></span>

1. <span data-ttu-id="d983f-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d983f-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="d983f-123">Выберите банковский счет, для которого необходимо просмотреть записи экспорта Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="d983f-123">Select the bank account that you want to view Positive Pay export records for.</span></span>
3. <span data-ttu-id="d983f-124">Выберите действие **Записи Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="d983f-124">Choose the **Positive Pay Entries** action.</span></span>

    <span data-ttu-id="d983f-125">В окне **Записи Positive Pay** можно просмотреть все записи экспорта Positive Pay для банковского счета.</span><span class="sxs-lookup"><span data-stu-id="d983f-125">In the **Positive Pay Entries** window, you can see all the Positive Pay export records for the bank account.</span></span>
4. <span data-ttu-id="d983f-126">В поле **Номер подтверждения** введите для каждой записи экспорта номер подтверждения, полученный после успешной отправки файла в банк.</span><span class="sxs-lookup"><span data-stu-id="d983f-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span></span>
5. <span data-ttu-id="d983f-127">Для просмотра связанных строк платежей выберите действие **Сведения по операции Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="d983f-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span></span>

<span data-ttu-id="d983f-128">Повторный экспорт файлов Positive Pay</span><span class="sxs-lookup"><span data-stu-id="d983f-128">To reexport Positive Pay files</span></span>

1. <span data-ttu-id="d983f-129">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="d983f-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="d983f-130">Выберите банковский счет, для которого необходимо повторно экспортировать файлы Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="d983f-130">Select the bank account that you want to reexport Positive Pay files for.</span></span>
3. <span data-ttu-id="d983f-131">Выберите действие **Записи Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="d983f-131">Choose the **Positive Pay Entries** action.</span></span>
4. <span data-ttu-id="d983f-132">Выберите строку для файла Positive Pay, который необходимо повторно экспортировать.</span><span class="sxs-lookup"><span data-stu-id="d983f-132">Select the line for the Positive Pay export file that you want to reexport.</span></span>
5. <span data-ttu-id="d983f-133">В окне **Записи Positive Pay** выберите действие **Повторный экспорт Positive Pay в файл**.</span><span class="sxs-lookup"><span data-stu-id="d983f-133">In the **Positive Pay Entries** window, choose the **Reexport Positive Pay to File** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="d983f-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d983f-134">See Also</span></span>
[<span data-ttu-id="d983f-135">Финансы</span><span class="sxs-lookup"><span data-stu-id="d983f-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="d983f-136">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="d983f-136">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="d983f-137">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="d983f-137">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="d983f-138">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d983f-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

