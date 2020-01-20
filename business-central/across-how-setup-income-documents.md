---
title: Настройка входящих документов| Документация Майкрософт
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
ms.date: 12/09/2019
ms.author: sgroespe
ms.openlocfilehash: e67ca1c0b26d7e4a81e53854ca31efc64a366c3f
ms.sourcegitcommit: 3d128a00358668b3fdd105ebf4604ca4e2b6743c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2019
ms.locfileid: "2910496"
---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="8f0b6-103">Настройка входящих документов</span><span class="sxs-lookup"><span data-stu-id="8f0b6-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="8f0b6-104">При создании строк финансового журнала на основании записей входящих документов необходимо выбрать на странице **Настройка входящих документов** шаблон и раздел журнала.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-104">If you create general journal lines from incoming document records, you must specify on the **Incoming Documents Setup** page which journal template and batch to use.</span></span>

<span data-ttu-id="8f0b6-105">Если пользователи не должны создавать счета или строки общего журнала по записям входящих документов до их утверждения, необходимо настроить утверждающих рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up workflow approvers.</span></span>

<span data-ttu-id="8f0b6-106">Чтобы преобразовать PDF-файлы и файлы изображений в электронные документы, которые можно будет преобразовывать, например, счета покупки в [!INCLUDE[d365fin](includes/d365fin_md.md)], следует сначала настроить функцию OCR и включить этот сервис.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="8f0b6-107">Если функция входящих документов настроена, можно использовать различные функции для просмотра квитанций по расходам, управления задачами OCR, а также преобразования входящих файлов документов, вручную и автоматически, в соответствующие документы либо строки журналов.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="8f0b6-108">Внешние файлы можно прикреплять на любом этапе обработки, в том числе к учтенным документам и к полученным записям поставщика, клиента и главной книги.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="8f0b6-109">Дополнительные сведения см. в разделе [Обработка входящих документов](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="8f0b6-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="8f0b6-110">Настройка возможности входящих документов</span><span class="sxs-lookup"><span data-stu-id="8f0b6-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="8f0b6-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка входящих документов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="8f0b6-112">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="8f0b6-113">Настройка утверждающих для записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="8f0b6-113">To set up approvers of incoming document records</span></span>
<span data-ttu-id="8f0b6-114">Утверждающие входящих документов должны быть настроены в качестве пользователей рабочего процесса утверждения.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-114">Approvers of incoming documents must be set up as approval workflow users.</span></span>

<span data-ttu-id="8f0b6-115">Прежде чем можно будет создавать рабочие процессы, которые включают шаги утверждения, необходимо настроить пользователей рабочих процессов, участвующих в процессах утверждения.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-115">Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes.</span></span> <span data-ttu-id="8f0b6-116">На странице **Настройка пользователя для утверждений** также можно задавать лимиты по суммам для отдельных типов запросов и определять заместителей утверждающих лиц, которым делегируются запросы на утверждение в случае отсутствия исходного утверждающего лица.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-116">On the **Approval User Setup** page, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.</span></span> <span data-ttu-id="8f0b6-117">Дополнительные сведения см. в разделе [Настройка утверждающих пользователей](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="8f0b6-117">For more information, see [Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="8f0b6-118">Настройка службы распознавания</span><span class="sxs-lookup"><span data-stu-id="8f0b6-118">To set up an OCR service</span></span>
1. <span data-ttu-id="8f0b6-119">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка OCR**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="8f0b6-120">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-120">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> <span data-ttu-id="8f0b6-121">Ваши учетные данные автоматически шифруются.</span><span class="sxs-lookup"><span data-stu-id="8f0b6-121">You login data is automatically encrypted.</span></span>

## <a name="see-also"></a><span data-ttu-id="8f0b6-122">См. также</span><span class="sxs-lookup"><span data-stu-id="8f0b6-122">See Also</span></span>
[<span data-ttu-id="8f0b6-123">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="8f0b6-123">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="8f0b6-124">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="8f0b6-124">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="8f0b6-125">Покупки</span><span class="sxs-lookup"><span data-stu-id="8f0b6-125">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="8f0b6-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8f0b6-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
