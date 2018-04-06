---
title: "Создание записей входящих документов | Microsoft Docs"
description: "Вы можете создавать записи входящих документах, например для счетов, и управлять задачами OCR, eCommerce и обмена документами."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f80438923773822eba0abc7dfa7dae45b0e87637
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="create-incoming-document-records"></a><span data-ttu-id="f3fc7-103">Создание записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="f3fc7-103">Create Incoming Document Records</span></span>
<span data-ttu-id="f3fc7-104">В окне **Входящие документы** можно использовать различные функции для просмотра квитанций по расходам, управления задачами OCR, а также преобразования входящих файлов документов, вручную и автоматически, в соответствующие документы либо строки журналов.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-104">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="f3fc7-105">Внешние файлы можно прикреплять на любом этапе обработки, в том числе к учтенным документам и к полученным записям поставщика, клиента и главной книги.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-105">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="f3fc7-106">Чтобы зарегистрировать внешний документ в [!INCLUDE[d365fin](includes/d365fin_md.md)], сначала необходимо создать или завершить запись входящего документа.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-106">To record an external document in [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first create or complete an incoming document record.</span></span> <span data-ttu-id="f3fc7-107">Это можно сделать вручную или можно сфотографировать внешний документ, а затем создать запись входящего документа с вложенным файлом изображения.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-107">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="f3fc7-108">Перед использованием функции входящих документов необходимо выполнить обязательную настройку.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-108">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="f3fc7-109">Дополнительные сведения см. в разделе [Настройка входящих документов](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="f3fc7-109">For more information, see [Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="f3fc7-110">Утверждение или отклонение входящего документа</span><span class="sxs-lookup"><span data-stu-id="f3fc7-110">To approve or reject an incoming document</span></span>
<span data-ttu-id="f3fc7-111">Если необходимо разрешить пользователям создавать счета или строки общего журнала на основе записей входящего документа до их утверждения, можно настроить утверждающих, которые будут утверждать записи перед их обработкой.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-111">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="f3fc7-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Входящие документы**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="f3fc7-113">Выберите строку с документом, который необходимо утвердить или отклонить, а затем выберите действие **Утвердить** или **Отклонить**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-113">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="f3fc7-114">При утверждении записи входящего документа в строке этого документа устанавливается флажок **Выпущено**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-114">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="f3fc7-115">Например, пользователь, который отвечает за создание счетов на покупку, может перейти к обработке записи.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-115">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="f3fc7-116">Создание записи входящего документа по фотографии</span><span class="sxs-lookup"><span data-stu-id="f3fc7-116">To create an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="f3fc7-117">Следующая процедура применяется только к клиентам [!INCLUDE[d365fin](includes/d365fin_md.md)] для планшетов и телефонов.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-117">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="f3fc7-118">В строке приложения выберите плитку **Создать входящий документ по данным камеры**, а затем перейдите к шагу 4.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-118">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="f3fc7-119">Или же в строке приложения нажмите кнопку приложения, выберите **Входящие документы**, а затем выберите **Все**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-119">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="f3fc7-120">В окне **Входящие документы** нажмите кнопку с многоточием, а затем выберите **Создать из камеры**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-120">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="f3fc7-121">Камера планшета или телефона включится.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-121">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="f3fc7-122">Сделайте фотографию документа, например приходной накладной, которую требуется обработать как входящий документ, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-122">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="f3fc7-123">Создается новая запись входящего документа с прикрепленным изображением.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-123">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="f3fc7-124">Прикрепление изображения к записи входящего документа по фотографии</span><span class="sxs-lookup"><span data-stu-id="f3fc7-124">To attach an image to an incoming document record by taking a photo</span></span>
> [!NOTE]  
>   <span data-ttu-id="f3fc7-125">Следующая процедура применяется только к клиентам [!INCLUDE[d365fin](includes/d365fin_md.md)] для планшетов и телефонов.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-125">The following procedure only applies to the [!INCLUDE[d365fin](includes/d365fin_md.md)] Tablet and Phone clients.</span></span>

1. <span data-ttu-id="f3fc7-126">В строке приложения нажмите кнопку приложения, выберите **Входящие документы**, а затем выберите **Все**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-126">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="f3fc7-127">Откройте карточку для существующей записи входящего документа.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-127">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="f3fc7-128">В окне **Входящий документ** нажмите кнопку с многоточием, а затем выберите **Прикрепить изображение с камеры**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-128">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="f3fc7-129">Камера планшета или телефона включится.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-129">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="f3fc7-130">Сделайте фотографию документа, например приходной накладной, которую требуется обработать как входящий документ, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-130">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

    <span data-ttu-id="f3fc7-131">Изображение прикрепляется к записи входящего документа.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-131">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="f3fc7-132">Создание записи входящего документа вручную</span><span class="sxs-lookup"><span data-stu-id="f3fc7-132">To create an incoming document record manually</span></span>
1. <span data-ttu-id="f3fc7-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Входящие документы**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="f3fc7-134">Выберите действие **Создать из файла**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-134">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="f3fc7-135">В окне **Вставка файла** выделите файл, а затем выберите **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-135">In the **Insert File** window, select a file, and then choose **Open**.</span></span> <span data-ttu-id="f3fc7-136">Файл будет прикреплен автоматически.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-136">The file is automatically attached.</span></span>
4. <span data-ttu-id="f3fc7-137">Кроме того, выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-137">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="f3fc7-138">Чтобы вложить файл, выберите действие **Прикрепить файл**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-138">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="f3fc7-139">В окне **Вставка файла** выберите файл, представляющий соответствующий входящий документ, а затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-139">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="f3fc7-140">В окне **Входящий документ** заполните поля по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="f3fc7-140">In the **Incoming Document** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a><span data-ttu-id="f3fc7-141">См. также</span><span class="sxs-lookup"><span data-stu-id="f3fc7-141">See Also</span></span>
[<span data-ttu-id="f3fc7-142">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="f3fc7-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="f3fc7-143">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="f3fc7-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="f3fc7-144">Покупки</span><span class="sxs-lookup"><span data-stu-id="f3fc7-144">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="f3fc7-145">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f3fc7-145">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

