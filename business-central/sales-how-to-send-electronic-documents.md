---
title: Отправка электронных документов
description: Узнайте, как отправлять счета в электронном виде.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 43f61682a1068a8e1652fd28421f83d5291c8fe8
ms.sourcegitcommit: fe6943d410f5dca4e8b2986f95501009ae982d98
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "4827072"
---
# <a name="send-electronic-documents"></a><span data-ttu-id="d7e9f-103">Отправка электронных документов</span><span class="sxs-lookup"><span data-stu-id="d7e9f-103">Send Electronic Documents</span></span>

<span data-ttu-id="d7e9f-104">Универсальная версия [!INCLUDE[prod_short](includes/prod_short.md)] поддерживает отправку электронных счетов и кредит-нот в формате PEPPOL, который поддерживается крупнейшими поставщиками служб обмена документами.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-104">The generic version of [!INCLUDE[prod_short](includes/prod_short.md)] supports sending electronic invoices and credit memos in the PEPPOL format, a format that the largest document exchange service providers support.</span></span> <span data-ttu-id="d7e9f-105">Поставщик службы обмена документами обеспечивает перемещение электронных документов между торговыми партнерами.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="d7e9f-106">Чтобы обеспечить поддержку других форматов электронных документов, следует использовать платформу обмена данными.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="d7e9f-107">В универсальной версии [!INCLUDE[prod_short](includes/prod_short.md)] служба обмена документами предварительно сконфигурирована и готова для настройки в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-107">In the generic version of [!INCLUDE[prod_short](includes/prod_short.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="d7e9f-108">Дополнительные сведения см. в разделе [Настройка службы обмена документами](across-how-to-set-up-a-document-exchange-service.md).</span><span class="sxs-lookup"><span data-stu-id="d7e9f-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span> <span data-ttu-id="d7e9f-109">Однако в некоторых случаях необходимо установить приложение.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-109">However, in some cases, you must install an app.</span></span> <span data-ttu-id="d7e9f-110">Дополнительные сведения см. в разделе [Вопросы и ответы по электронному выставлению счетов](faq-electronic-invoicing.yml).</span><span class="sxs-lookup"><span data-stu-id="d7e9f-110">For more information, see [Electronic Invoicing FAQ](faq-electronic-invoicing.yml).</span></span>  

 <span data-ttu-id="d7e9f-111">Чтобы отправить счет продажи как электронный документ PEPPOL, следует выбрать параметр **Электронный документ** в диалоговом окне **Учет и отправка**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-111">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box.</span></span> <span data-ttu-id="d7e9f-112">Также можно настроить профиль отправки документов клиента по умолчанию из этого диалогового окна.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-112">You can also set up the customer's default document sending profile from that dialog box.</span></span> <span data-ttu-id="d7e9f-113">Прежде всего, необходимо настроить различные основные данные – такие как информацию об организации, клиентах, товарах и единицах измерения.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-113">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="d7e9f-114">Они используются для определения бизнес-партнеров и товаров при преобразовании данных в полях в разделе [Настройка отправки и получения электронных документов](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="d7e9f-114">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="d7e9f-115">Отправка электронного счета продажи</span><span class="sxs-lookup"><span data-stu-id="d7e9f-115">To send an electronic sales invoice</span></span>

1. <span data-ttu-id="d7e9f-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2. <span data-ttu-id="d7e9f-117">Создайте новый счет продажи.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-117">Create a new sales invoice.</span></span>  

3. <span data-ttu-id="d7e9f-118">Когда строки счета продажи готовы к выставлению счета, выберите действие **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-118">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span></span>  

     <span data-ttu-id="d7e9f-119">Если профиль отправки по умолчанию клиента — **Электронный документ**, то он будет показан в диалоговом окне **Подтверждение учета и отправки**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-119">If the customer's default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box.</span></span> <span data-ttu-id="d7e9f-120">Таким образом, вам просто нужно выбрать кнопку **Да**, чтобы учесть и отправить счет в электронном виде в выбранном формате.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-120">This way, you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4. <span data-ttu-id="d7e9f-121">В диалоговом окне **Подтверждение учета и отправки** нажмите кнопку AssistEdit справа от поля **Кому отправить документ**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-121">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5. <span data-ttu-id="d7e9f-122">В диалоговом окне **Кому отправить документ** в поле **Электронный документ** выберите **Через службу обмена документами**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-122">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6. <span data-ttu-id="d7e9f-123">В поле **Формат** выберите **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-123">In the **Format** field, choose **PEPPOL**.</span></span>  

7. <span data-ttu-id="d7e9f-124">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-124">Choose the **OK** button.</span></span> <span data-ttu-id="d7e9f-125">Откроется диалоговое окно **Подтверждение учета и отправки**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-125">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="d7e9f-126">**Электронный документ (PEPPOL)** будет добавлен в поле **Кому отправить документ**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-126">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8. <span data-ttu-id="d7e9f-127">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-127">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="d7e9f-128">Счет продажи учтен и отправлен клиенту в формате PEPPOL.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-128">The sales invoice is posted and sent to the customer in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="d7e9f-129">Можно также отправить учтенный счет на продажу в виде электронного документа.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-129">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="d7e9f-130">Процедура аналогична описанной в этом разделе для документов неучтенных продаж.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-130">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="d7e9f-131">На странице **Учтенный счет продажи** выберите действие **Журнал действий** для просмотра статуса электронного документа.</span><span class="sxs-lookup"><span data-stu-id="d7e9f-131">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="d7e9f-132">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="d7e9f-132">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="d7e9f-133">См. также</span><span class="sxs-lookup"><span data-stu-id="d7e9f-133">See Also</span></span>

[<span data-ttu-id="d7e9f-134">Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="d7e9f-134">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="d7e9f-135">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="d7e9f-135">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="d7e9f-136">Настройка отправки и получения электронных документов</span><span class="sxs-lookup"><span data-stu-id="d7e9f-136">Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="d7e9f-137">Настройка службы обмена документами</span><span class="sxs-lookup"><span data-stu-id="d7e9f-137">Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="d7e9f-138">Настройка определений обмена данными</span><span class="sxs-lookup"><span data-stu-id="d7e9f-138">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="d7e9f-139">Электронный обмен данными</span><span class="sxs-lookup"><span data-stu-id="d7e9f-139">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="d7e9f-140">Вопросы и ответы по электронным счетам</span><span class="sxs-lookup"><span data-stu-id="d7e9f-140">Electronic Invoicing FAQ</span></span>](faq-electronic-invoicing.yml)  
[<span data-ttu-id="d7e9f-141">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="d7e9f-141">General Business Functionality</span></span>](ui-across-business-areas.md)  
