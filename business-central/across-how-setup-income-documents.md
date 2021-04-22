---
title: Настройка входящих документов| Документация Майкрософт
description: Используйте функцию входящих документов для создания документов, управления задачами OCR, импорта счетов преобразования файлов изображений.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fd35c0af4d2b66f99c0a4a3a65f77826cd9af806
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775926"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="2ebb5-103">Настройка входящих документов</span><span class="sxs-lookup"><span data-stu-id="2ebb5-103">Set Up Incoming Documents</span></span>

<span data-ttu-id="2ebb5-104">При создании строк финансового журнала на основании записей входящих документов необходимо выбрать на странице **Настройка входящих документов** шаблон и раздел журнала.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="2ebb5-105">Если пользователи не должны создавать счета или строки общего журнала по записям входящих документов до их утверждения, необходимо настроить утверждающих рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span></span>

<span data-ttu-id="2ebb5-106">Чтобы преобразовать PDF-файлы и файлы изображений в электронные документы, которые можно будет преобразовывать, например, счета покупки в [!INCLUDE[prod_short](includes/prod_short.md)], следует сначала настроить функцию OCR и включить этот сервис.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[prod_short](includes/prod_short.md)], you must first set up the OCR feature and enable the service.</span></span> <span data-ttu-id="2ebb5-107">Выберите пакет услуг, подходящий для вашей организации и/или страны/региона.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-107">Choose a service package that is appropriate for your organization and/or country/region.</span></span> <span data-ttu-id="2ebb5-108">Кроме того, вы можете создавать записи вручную для представления внешних документов.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-108">Alternatively, you can create entries manually to represent the external documents.</span></span>  

<span data-ttu-id="2ebb5-109">Если функция входящих документов настроена, можно использовать различные функции для просмотра квитанций по расходам, управления задачами OCR, а также преобразования входящих файлов документов, вручную и автоматически, в соответствующие документы либо строки журналов.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-109">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="2ebb5-110">Внешние файлы можно прикреплять на любом этапе обработки, в том числе к учтенным документам и к полученным записям поставщика, клиента и главной книги.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-110">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="2ebb5-111">Дополнительные сведения см. в разделе [Обработка входящих документов](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="2ebb5-111">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="2ebb5-112">Настройка возможности входящих документов</span><span class="sxs-lookup"><span data-stu-id="2ebb5-112">To set up the Incoming Documents feature</span></span>

1. <span data-ttu-id="2ebb5-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка входящих документов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="2ebb5-114">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-114">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="2ebb5-115">В рамках настройки вы должны решить, хотите ли вы требовать утверждения входящих документов.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-115">As part of the setup, you must decide if you want to require approval of incoming documents.</span></span> <span data-ttu-id="2ebb5-116">Чтобы требовать утверждения, вы должны настроить утверждающих и рабочие процессы утверждения.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-116">To require approval, you must set up approvers and approval workflows.</span></span> <span data-ttu-id="2ebb5-117">Если ваша организация не намерена требовать утверждения, вы можете пропустить следующий раздел.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-117">If your organization does not intend to require approval, you can skip the next section.</span></span>  

<span data-ttu-id="2ebb5-118">Наконец, если вы используете службу для преобразования файлов PDF или изображений, представляющих входящие документы, вы должны ее настроить.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-118">Finally, you if you use a service to convert PDF or image files representing incoming documents, you must it set up.</span></span> <span data-ttu-id="2ebb5-119">В противном случае вы также можете пропустить этот раздел.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-119">Otherwise, you can also skip that section.</span></span>  

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="2ebb5-120">Настройка утверждающих для записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="2ebb5-120">To set up approvers of incoming document records</span></span>

<span data-ttu-id="2ebb5-121">При желании настройте процесс утверждения для входящих документов.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-121">Optionally, set up an approval process for the incoming documents.</span></span> <span data-ttu-id="2ebb5-122">Утверждающие входящих документов должны быть настроены в качестве пользователей рабочего процесса утверждения.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-122">Approvers of incoming documents must be set up as approval workflow users.</span></span>

<span data-ttu-id="2ebb5-123">Прежде чем можно будет создавать рабочие процессы, которые включают шаги утверждения, необходимо настроить пользователей рабочих процессов, участвующих в процессах утверждения.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-123">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span></span> <span data-ttu-id="2ebb5-124">На странице **Настройка пользователя для утверждений** также можно задавать лимиты по суммам для отдельных типов запросов и определять заместителей утверждающих лиц, которым делегируются запросы на утверждение в случае отсутствия исходного утверждающего лица.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-124">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span></span> <span data-ttu-id="2ebb5-125">Дополнительные сведения см. в разделе [Настройка утверждающих пользователей](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="2ebb5-125">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="2ebb5-126">Настройка службы распознавания</span><span class="sxs-lookup"><span data-stu-id="2ebb5-126">To set up an OCR service</span></span>

1. <span data-ttu-id="2ebb5-127">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка OCR**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="2ebb5-128">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-128">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="2ebb5-129">Ваши учетные данные автоматически шифруются.</span><span class="sxs-lookup"><span data-stu-id="2ebb5-129">You login data is automatically encrypted.</span></span>

<span data-ttu-id="2ebb5-130">Дополнительные сведения см. в разделе [Использование OCR для преобразования PDF-файлов и графических файлов в электронные документы](across-how-use-ocr-pdf-images-files.md).</span><span class="sxs-lookup"><span data-stu-id="2ebb5-130">For more information, see [Use OCR to Turn PDF and Image Files into Electronic Documents](across-how-use-ocr-pdf-images-files.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="2ebb5-131">См. также</span><span class="sxs-lookup"><span data-stu-id="2ebb5-131">See Also</span></span>

[<span data-ttu-id="2ebb5-132">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="2ebb5-132">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="2ebb5-133">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="2ebb5-133">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="2ebb5-134">Покупки</span><span class="sxs-lookup"><span data-stu-id="2ebb5-134">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="2ebb5-135">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2ebb5-135">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]