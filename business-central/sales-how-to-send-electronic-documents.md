---
title: Отправка электронных документов | Документация Майкрософт
description: Узнайте, как отправлять счета в электронном виде.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 110c81bdf6de02e16a1e1185028f6b803290f3d7
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3192667"
---
# <a name="send-electronic-documents"></a><span data-ttu-id="c19f1-103">Отправка электронных документов</span><span class="sxs-lookup"><span data-stu-id="c19f1-103">Send Electronic Documents</span></span>
<span data-ttu-id="c19f1-104">Универсальная версия [!INCLUDE[d365fin](includes/d365fin_md.md)] поддерживает отправку электронных счетов и кредит-нот в формате PEPPOL, поддерживаемом крупнейшими поставщиками служб обмена документами.</span><span class="sxs-lookup"><span data-stu-id="c19f1-104">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports sending electronic invoices and credit memos in the PEPPOL format, which is supported by the largest document exchange service providers.</span></span> <span data-ttu-id="c19f1-105">Поставщик службы обмена документами обеспечивает перемещение электронных документов между торговыми партнерами.</span><span class="sxs-lookup"><span data-stu-id="c19f1-105">A document exchange service provider dispatches electronic documents between trading partners.</span></span> <span data-ttu-id="c19f1-106">Чтобы обеспечить поддержку других форматов электронных документов, следует использовать платформу обмена данными.</span><span class="sxs-lookup"><span data-stu-id="c19f1-106">To provide support for other electronic document formats, you use the data exchange framework.</span></span>  

 <span data-ttu-id="c19f1-107">В универсальной версии [!INCLUDE[d365fin](includes/d365fin_md.md)] служба обмена документами предварительно сконфигурирована и готова для настройки в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="c19f1-107">In the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)], a document exchange service is preconfigured and ready to be set up for your company.</span></span> <span data-ttu-id="c19f1-108">Дополнительные сведения см. в разделе [Настройка службы обмена документами](across-how-to-set-up-a-document-exchange-service.md).</span><span class="sxs-lookup"><span data-stu-id="c19f1-108">For more information, see [Set Up a Document Exchange Service](across-how-to-set-up-a-document-exchange-service.md).</span></span>  

 <span data-ttu-id="c19f1-109">Для отправки счета продажи в виде электронного документа PEPPOL следует выбрать вариант **Электронный документ** в диалоговом окне **Учет и отправка**, в котором также можно задать его в качестве профиля отправки документов клиенту по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c19f1-109">To send a sales invoice as an electronic PEPPOL document, you select the **Electronic Document** option in the **Post and Send** dialog box from where you can also set up the customer’s default document sending profile.</span></span> <span data-ttu-id="c19f1-110">Прежде всего, необходимо настроить различные основные данные – такие как информацию об организации, клиентах, товарах и единицах измерения.</span><span class="sxs-lookup"><span data-stu-id="c19f1-110">First, you must set up various master data, such as company information, customers, items, and units of measure.</span></span> <span data-ttu-id="c19f1-111">Они используются для определения бизнес-партнеров и товаров при преобразовании данных в полях в разделе [Настройка отправки и получения электронных документов](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span><span class="sxs-lookup"><span data-stu-id="c19f1-111">These are used to identify the business partners and items when converting data in fields in [Set Up Electronic Document Sending and Receiving](across-how-to-set-up-electronic-document-sending-and-receiving.md).</span></span>  

### <a name="to-send-an-electronic-sales-invoice"></a><span data-ttu-id="c19f1-112">Отправка электронного счета продажи</span><span class="sxs-lookup"><span data-stu-id="c19f1-112">To send an electronic sales invoice</span></span>  

1.  <span data-ttu-id="c19f1-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c19f1-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Invoices**, and then choose the related link.</span></span>  

2.  <span data-ttu-id="c19f1-114">Создайте новый счет продажи.</span><span class="sxs-lookup"><span data-stu-id="c19f1-114">Create a new sales invoice.</span></span>  

3.  <span data-ttu-id="c19f1-115">Когда строки счета продажи готовы к выставлению счета, выберите действие **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-115">When the sales invoice is ready to be invoiced, choose the **Post and Send** action.</span></span>  

     <span data-ttu-id="c19f1-116">Если в профиле клиент по умолчанию указано **Электронный документ**, он также будет указан в диалоговом окне **Подтверждение учета и отправки**; необходимо только нажать кнопку **Да** для отправки счета по электронной почте в выбранном в формате.</span><span class="sxs-lookup"><span data-stu-id="c19f1-116">If the customer’s default sending profile is **Electronic Document**, then it will be shown in the **Post and Send Confirmation** dialog box and you just have to choose the **Yes** button to post and send the invoice electronically in the selected format.</span></span>  

4.  <span data-ttu-id="c19f1-117">В диалоговом окне **Подтверждение учета и отправки** нажмите кнопку AssistEdit справа от поля **Кому отправить документ**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-117">In the **Post and Send Confirmation** dialog box, choose the AssistEdit button to the right of the **Send Document to** field.</span></span>  

5.  <span data-ttu-id="c19f1-118">В диалоговом окне **Кому отправить документ** в поле **Электронный документ** выберите **Через службу обмена документами**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-118">In the **Send Document to** dialog box, in the **Electronic Document** field, choose **Through Document Exchange Service**.</span></span>  

6.  <span data-ttu-id="c19f1-119">В поле **Формат** выберите **PEPPOL**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-119">In the **Format** field, choose **PEPPOL**.</span></span>  

7.  <span data-ttu-id="c19f1-120">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-120">Choose the **OK** button.</span></span> <span data-ttu-id="c19f1-121">Откроется диалоговое окно **Подтверждение учета и отправки**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-121">The **Post and Send Confirmation** dialog box appears.</span></span> <span data-ttu-id="c19f1-122">**Электронный документ (PEPPOL)** будет добавлен в поле **Кому отправить документ**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-122">**Electronic Document (PEPPOL)** is added to the **Send Document to** field.</span></span>  

8.  <span data-ttu-id="c19f1-123">Нажмите кнопку **Да**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-123">Choose the **Yes** button.</span></span>  

     <span data-ttu-id="c19f1-124">Счет продажи учтен и отправлен клиенту в виде электронного документа в формате PEPPOL.</span><span class="sxs-lookup"><span data-stu-id="c19f1-124">The sales invoice is posted and sent to the customer as an electronic document in the PEPPOL format.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c19f1-125">Можно также отправить учтенный счет на продажу в виде электронного документа.</span><span class="sxs-lookup"><span data-stu-id="c19f1-125">You can also send a posted sales invoice as an electronic document.</span></span> <span data-ttu-id="c19f1-126">Процедура аналогична описанной в этом разделе для документов неучтенных продаж.</span><span class="sxs-lookup"><span data-stu-id="c19f1-126">The procedure is the same as described in this topic for non-posted sales documents.</span></span> <span data-ttu-id="c19f1-127">На странице **Учтенный счет продажи** выберите действие **Журнал действий** для просмотра статуса электронного документа.</span><span class="sxs-lookup"><span data-stu-id="c19f1-127">On the **Posted Sales Invoice** page, choose the **Activity Log** action to view the status of the electronic document.</span></span> <span data-ttu-id="c19f1-128">Для получения дополнительных сведений см раздел **Журнал действий**.</span><span class="sxs-lookup"><span data-stu-id="c19f1-128">For more information, see **Activity Log**.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="c19f1-129">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="c19f1-129">See Related Training at [Microsoft Learn](/learn/modules/electronic-documents-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="c19f1-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c19f1-130">See Also</span></span>  
[<span data-ttu-id="c19f1-131">Выставление счетов продажи</span><span class="sxs-lookup"><span data-stu-id="c19f1-131">Invoice Sales</span></span>](sales-how-invoice-sales.md)  
[<span data-ttu-id="c19f1-132">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="c19f1-132">Set Up Document Sending Profiles</span></span>](sales-how-setup-document-send-profiles.md)  
[<span data-ttu-id="c19f1-133">Настройка отправки и получения электронных документов</span><span class="sxs-lookup"><span data-stu-id="c19f1-133">Set Up Electronic Document Sending and Receiving</span></span>](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[<span data-ttu-id="c19f1-134">Настройка службы обмена документами</span><span class="sxs-lookup"><span data-stu-id="c19f1-134">Set Up a Document Exchange Service</span></span>](across-how-to-set-up-a-document-exchange-service.md)  
[<span data-ttu-id="c19f1-135">Настройка определений обмена данными</span><span class="sxs-lookup"><span data-stu-id="c19f1-135">Set Up Data Exchange Definitions</span></span>](across-how-to-set-up-data-exchange-definitions.md)  
[<span data-ttu-id="c19f1-136">Электронный обмен данными</span><span class="sxs-lookup"><span data-stu-id="c19f1-136">Exchanging Data Electronically</span></span>](across-data-exchange.md)  
[<span data-ttu-id="c19f1-137">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="c19f1-137">General Business Functionality</span></span>](ui-across-business-areas.md)  
