---
title: Настройка входящих документов| Microsoft Docs
description: Используйте функцию входящих документов для создания документов, управления задачами OCR, импорта счетов преобразования файлов изображений.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7e99f4b33767a1bdea7b942d1b183edbacc829ac
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241512"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="9d18e-103">Настройка входящих документов</span><span class="sxs-lookup"><span data-stu-id="9d18e-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="9d18e-104">При создании строк финансового журнала на основании записей входящих документов необходимо выбрать на странице **Настройка входящих документов** шаблон и раздел журнала.</span><span class="sxs-lookup"><span data-stu-id="9d18e-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="9d18e-105">Если пользователи не должны создавать счета или строки финансового журнала на основании записей входящих документов до утверждения документов, необходимо настроить утверждающих на странице **Утверждающие для входящего документа**.</span><span class="sxs-lookup"><span data-stu-id="9d18e-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers on the **Incoming Document Approvers** page.</span></span>

<span data-ttu-id="9d18e-106">Чтобы преобразовать PDF-файлы и файлы изображений в электронные документы, которые можно будет преобразовывать, например, счета покупки в [!INCLUDE[d365fin](includes/d365fin_md.md)], следует сначала настроить функцию OCR и включить этот сервис.</span><span class="sxs-lookup"><span data-stu-id="9d18e-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="9d18e-107">Если функция входящих документов настроена, можно использовать различные функции для просмотра квитанций по расходам, управления задачами OCR, а также преобразования входящих файлов документов, вручную и автоматически, в соответствующие документы либо строки журналов.</span><span class="sxs-lookup"><span data-stu-id="9d18e-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="9d18e-108">Внешние файлы можно прикреплять на любом этапе обработки, в том числе к учтенным документам и к полученным записям поставщика, клиента и главной книги.</span><span class="sxs-lookup"><span data-stu-id="9d18e-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="9d18e-109">Дополнительные сведения см. в разделе [Обработка входящих документов](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="9d18e-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="9d18e-110">Настройка возможности входящих документов</span><span class="sxs-lookup"><span data-stu-id="9d18e-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="9d18e-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка входящих документов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="9d18e-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="9d18e-112">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="9d18e-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="9d18e-113">Настройка утверждающих для записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="9d18e-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="9d18e-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка входящих документов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="9d18e-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="9d18e-115">На странице **Настройка входящих документов** выберите действие **Утверждающие**.</span><span class="sxs-lookup"><span data-stu-id="9d18e-115">On the **Incoming Documents Setup** page, choose the **Approvers** action.</span></span>

    <span data-ttu-id="9d18e-116">На странице **Утверждающие для входящего документа** будут показаны все пользователи, настроенные в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="9d18e-116">The **Incoming Document Approvers** page shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="9d18e-117">Выберите одного или нескольких пользователей, которые могут утвердить входящий документ до создания соответствующей строки в документе или журнале.</span><span class="sxs-lookup"><span data-stu-id="9d18e-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="9d18e-118">После настройки утверждающих на странице **Утверждание для входящего документа** только такие пользователи смогут утверждать входящий документ, если установлен флажок **Требовать утверждение для создания** на странице **Настройка входящих документов**.</span><span class="sxs-lookup"><span data-stu-id="9d18e-118">When approvers have been set up on the **Incoming Document Approvers** page, only those users can approve an incoming document if the **Require Approval To Create** check box on the **Incoming Documents Setup** page is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="9d18e-119">Эта настройка утверждения не связана с рабочими процессами утверждения.</span><span class="sxs-lookup"><span data-stu-id="9d18e-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="9d18e-120">Дополнительные сведения см. в разделе [Использование рабочих процессов утверждения](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="9d18e-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="9d18e-121">Настройка службы распознавания</span><span class="sxs-lookup"><span data-stu-id="9d18e-121">To set up an OCR service</span></span>
1. <span data-ttu-id="9d18e-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка OCR**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="9d18e-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="9d18e-123">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="9d18e-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="9d18e-124">Ваши учетные данные автоматически шифруются.</span><span class="sxs-lookup"><span data-stu-id="9d18e-124">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="9d18e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="9d18e-125">See Also</span></span>
[<span data-ttu-id="9d18e-126">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="9d18e-126">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="9d18e-127">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="9d18e-127">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="9d18e-128">Покупки</span><span class="sxs-lookup"><span data-stu-id="9d18e-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="9d18e-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9d18e-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
