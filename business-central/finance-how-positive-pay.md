---
title: Экспорт файлов Positive Pay | Документы Майкрософт
description: Вы можете гарантировать, чтобы банк выполнял клиринг только проверенных платежных документов и сумм путем экспорта файла Positive Pay, содержащего сведения о поставщике и платеже.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 61f3d3fcd093c9fca4e23481ff3b527714b85379
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804380"
---
# <a name="export-a-positive-pay-file"></a><span data-ttu-id="fc8cd-103">Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="fc8cd-103">Export a Positive Pay File</span></span>
<span data-ttu-id="fc8cd-104">Чтобы гарантировать, чтобы банк выполнял клиринг только по проверенным платежным документам и суммам, можно экспортировать файл Positive Pay, содержащий информацию о поставщике, номер платежного документа, сумму платежа, который можно затем переслать в банк для справки при обработке платежей.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-104">To make sure that your bank only clears validated checks and amounts, you can export a Positive Pay file that contains vendor information, check number, and payment amount, which you send to the bank for reference when you process payments.</span></span>

<span data-ttu-id="fc8cd-105">Программа [!INCLUDE[d365fin](includes/d365fin_md.md)] предварительно настроена для поддержки файлов Positive Pay оплаты для банков Bank of America и City Bank.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-105">[!INCLUDE[d365fin](includes/d365fin_md.md)] is preconfigured to support Positive Pay files for Bank of America and City Bank.</span></span>

## <a name="to-set-up-a-bank-account-for-positive-pay"></a><span data-ttu-id="fc8cd-106">Настройка банковского счета для Positive Pay</span><span class="sxs-lookup"><span data-stu-id="fc8cd-106">To set up a bank account for Positive Pay</span></span>
1. <span data-ttu-id="fc8cd-107">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-107">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc8cd-108">Откройте карточку банка, для которого требуется использовать Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-108">Open the card for the bank that you want to use Positive Pay for.</span></span>
3. <span data-ttu-id="fc8cd-109">В поле **Код экспорта Positive Pay** введите POSPAYBANK.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-109">In the **Positive Pay Export Code** field, enter POSPAYBANK.</span></span>
4. <span data-ttu-id="fc8cd-110">Закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-110">Close the page.</span></span>

## <a name="to-export-a-positive-pay-file"></a><span data-ttu-id="fc8cd-111">Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="fc8cd-111">To export a Positive Pay file</span></span>
1. <span data-ttu-id="fc8cd-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc8cd-113">Выберите банковский счет, для которого необходимо экспортировать файл Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-113">Select the bank account that you want to export a Positive Pay file for.</span></span>
3. <span data-ttu-id="fc8cd-114">Выберите действие **Экспорт Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-114">Choose **Positive Pay Export** action.</span></span>

    <span data-ttu-id="fc8cd-115">Откроется страница **Экспорт Positive Pay**, на которой отобразятся платежи, внесенные на банковский счет с даты последней отправки, как показано в полях **Дата последней отправки** и **Время последней отправки**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-115">The **Positive Pay Export** page opens displaying payments that have been made for the bank account since the last upload date, as shown in the **Last Upload Date** and **Last Upload Time** fields.</span></span>
4. <span data-ttu-id="fc8cd-116">В поле **Граничная дата отправки** укажите дату, до которой платежи не включаются в экспортированный файл.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-116">In the **Cutoff Upload Date** field, specify a date before which payments are not included in the exported file.</span></span>
5. <span data-ttu-id="fc8cd-117">Выберите действие **Экспорт**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-117">Choose the **Export** action.</span></span>
6. <span data-ttu-id="fc8cd-118">На странице **Экспорт файла** нажмите кнопку **Сохранить**, а затем сохраните файл в удобное расположение.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-118">On the **Export File** page, choose the **Save** button, and then save the file to a convenient location.</span></span>
7. <span data-ttu-id="fc8cd-119">Отправьте файл на сайт электронного банка.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-119">Upload the file to your electronic bank site.</span></span>
8. <span data-ttu-id="fc8cd-120">Запишите или скопируйте номер подтверждения, отображаемый после успешной отправки файла.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-120">Write down or copy the confirmation number that is displayed when the file upload is successful.</span></span>

<span data-ttu-id="fc8cd-121">Просмотр экспортированных записей Positive Pay</span><span class="sxs-lookup"><span data-stu-id="fc8cd-121">To view exported Positive Pay records</span></span>

1. <span data-ttu-id="fc8cd-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc8cd-123">Выберите банковский счет, для которого необходимо просмотреть записи экспорта Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-123">Select the bank account that you want to view Positive Pay export records for.</span></span>
3. <span data-ttu-id="fc8cd-124">Выберите действие **Записи Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-124">Choose the **Positive Pay Entries** action.</span></span>

    <span data-ttu-id="fc8cd-125">На странице **Записи Positive Pay** можно просмотреть все записи экспорта Positive Pay для банковского счета.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-125">On the **Positive Pay Entries** page, you can see all the Positive Pay export records for the bank account.</span></span>
4. <span data-ttu-id="fc8cd-126">В поле **Номер подтверждения** введите для каждой записи экспорта номер подтверждения, полученный после успешной отправки файла в банк.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-126">In the **Confirmation Number** field, enter, for each export record, the confirmation number that you receive when the file upload to the bank is successful.</span></span>
5. <span data-ttu-id="fc8cd-127">Для просмотра связанных строк платежей выберите действие **Сведения по операции Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-127">To view the related payment lines, choose the **Positive Pay Entry Details** action.</span></span>

<span data-ttu-id="fc8cd-128">Повторный экспорт файлов Positive Pay</span><span class="sxs-lookup"><span data-stu-id="fc8cd-128">To reexport Positive Pay files</span></span>

1. <span data-ttu-id="fc8cd-129">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Банковские счета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-129">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="fc8cd-130">Выберите банковский счет, для которого необходимо повторно экспортировать файлы Positive Pay.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-130">Select the bank account that you want to reexport Positive Pay files for.</span></span>
3. <span data-ttu-id="fc8cd-131">Выберите действие **Записи Positive Pay**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-131">Choose the **Positive Pay Entries** action.</span></span>
4. <span data-ttu-id="fc8cd-132">Выберите строку для файла Positive Pay, который необходимо повторно экспортировать.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-132">Select the line for the Positive Pay export file that you want to reexport.</span></span>
5. <span data-ttu-id="fc8cd-133">На странице **Записи Positive Pay** выберите действие **Повторный экспорт Positive Pay в файл**.</span><span class="sxs-lookup"><span data-stu-id="fc8cd-133">On the **Positive Pay Entries** page, choose the **Reexport Positive Pay to File** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="fc8cd-134">См. также</span><span class="sxs-lookup"><span data-stu-id="fc8cd-134">See Also</span></span>
[<span data-ttu-id="fc8cd-135">Финансы</span><span class="sxs-lookup"><span data-stu-id="fc8cd-135">Finance</span></span>](finance.md)  
[<span data-ttu-id="fc8cd-136">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="fc8cd-136">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="fc8cd-137">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="fc8cd-137">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="fc8cd-138">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fc8cd-138">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
