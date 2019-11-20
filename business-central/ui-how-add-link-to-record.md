---
title: Добавление вложений, ссылок и заметок в записи | Документация Майкрософт
description: Присоединение гиперссылок к документам или веб-сайтам на конкретную запись, например, на клиента или документ.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/21/2019
ms.author: sgroespe
ms.openlocfilehash: 88e6a04a8e4a992b6a5df3fee87104eba7b5510e
ms.sourcegitcommit: be1e2c49a8434d3f440d5a201508af9c3c8cc87f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "2649792"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="4d46a-103">Управление вложениями, ссылками и заметками в карточках и документах</span><span class="sxs-lookup"><span data-stu-id="4d46a-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="4d46a-104">В информационных панелях в большинстве карточек и документов можно вкладывать файлы, добавлять ссылки и писать заметки.</span><span class="sxs-lookup"><span data-stu-id="4d46a-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="4d46a-105">В случае ссылок и заметок это также можно делать на странице списка, предварительно выбрав соответствующую строку.</span><span class="sxs-lookup"><span data-stu-id="4d46a-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="4d46a-106">Чтобы просмотреть или изменить какой-либо из этих прикрепленных типов информации, необходимо сначала открыть вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="4d46a-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="4d46a-107">Цифра в заголовке вкладки показывает, сколько вложенных файлов, ссылок или заметок существует для карточки или документа.</span><span class="sxs-lookup"><span data-stu-id="4d46a-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="4d46a-108">Вложения, ссылки и заметки остаются прикрепленными, когда в результате обработки карточка или документ переходят в другое состояние, например когда текущий заказ на продажу превращается в учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="4d46a-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="4d46a-109">Однако обратите внимание, что ни один из типов вложений не выводится из системы, например при печати или при сохранении в файл.</span><span class="sxs-lookup"><span data-stu-id="4d46a-109">Note, however, that none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="4d46a-110">Прикрепление файла к счету покупки</span><span class="sxs-lookup"><span data-stu-id="4d46a-110">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="4d46a-111">К карточке или документу можно прикрепить файл любого типа, содержащий текст, изображение или видео.</span><span class="sxs-lookup"><span data-stu-id="4d46a-111">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="4d46a-112">Это удобно делать, например, когда вы хотите сохранить счет поставщика в виде файла PDF в соответствующем счете покупки в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="4d46a-112">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="4d46a-113">Файлы, прикрепленные с помощью функции "Входящие документы", на вкладке **Вложения** не отображаются. Дополнительные сведения см. в разделе [Входящие документы](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="4d46a-113">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="4d46a-114">Следующая процедура основана на заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="4d46a-114">The following procedure is based on a sales order.</span></span> <span data-ttu-id="4d46a-115">Действия для всех остальных поддерживаемых документов и карточек аналогичны.</span><span class="sxs-lookup"><span data-stu-id="4d46a-115">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="4d46a-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4d46a-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d46a-117">Откройте заказ на продажу, к которому требуется прикрепить файл.</span><span class="sxs-lookup"><span data-stu-id="4d46a-117">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="4d46a-118">В информационной панели откройте вкладку **Вложения**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-118">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="4d46a-119">Выберите значение за полем **Документы**, например "0".</span><span class="sxs-lookup"><span data-stu-id="4d46a-119">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="4d46a-120">На странице **Вложенные документы** в поле **Вложение** нажмите кнопку **Выберите файл**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-120">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** button.</span></span>
5. <span data-ttu-id="4d46a-121">Выберите файл из любого расположения, затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-121">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="4d46a-122">Файл прикреплен к счету покупки.</span><span class="sxs-lookup"><span data-stu-id="4d46a-122">The file is now attached to the purchase invoice.</span></span>

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="4d46a-123">Добавление ссылки из карточки товара</span><span class="sxs-lookup"><span data-stu-id="4d46a-123">To add a link from an item card</span></span>
<span data-ttu-id="4d46a-124">Можно добавить ссылку из карточки или документа на любой URL-адрес или путь.</span><span class="sxs-lookup"><span data-stu-id="4d46a-124">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="4d46a-125">Это удобно делать, например, когда вы хотите связать карточку товара с каталогом товаров поставщика.</span><span class="sxs-lookup"><span data-stu-id="4d46a-125">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="4d46a-126">Следующая процедура основана на карточке товара.</span><span class="sxs-lookup"><span data-stu-id="4d46a-126">The following procedure is based on an item card.</span></span> <span data-ttu-id="4d46a-127">Действия для всех остальных поддерживаемых карточек и документов аналогичны.</span><span class="sxs-lookup"><span data-stu-id="4d46a-127">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="4d46a-128">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4d46a-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d46a-129">Выберите товар, ссылку из которого вы хотите добавить, а затем выберите вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="4d46a-129">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="4d46a-130">В разделе **Ссылки** выберите значок **+**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-130">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="4d46a-131">В поле **Адрес ссылки** введите ссылку.</span><span class="sxs-lookup"><span data-stu-id="4d46a-131">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="4d46a-132">Ссылка должна быть действительным URL-адресом в Интернете или интрасети.</span><span class="sxs-lookup"><span data-stu-id="4d46a-132">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="4d46a-133">В поле **Описание** введите информацию о ссылке, если необходимо.</span><span class="sxs-lookup"><span data-stu-id="4d46a-133">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="4d46a-134">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-134">Choose the **OK** button.</span></span>

<span data-ttu-id="4d46a-135">Ссылка прикреплена к карточке товара.</span><span class="sxs-lookup"><span data-stu-id="4d46a-135">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="4d46a-136">Написание заметки о заказе на продажу</span><span class="sxs-lookup"><span data-stu-id="4d46a-136">To write a note on a sales order</span></span>
<span data-ttu-id="4d46a-137">Вы можете написать заметку к документе или карточке, — например, чтобы предоставить особые указания для других пользователей документа или карточки.</span><span class="sxs-lookup"><span data-stu-id="4d46a-137">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="4d46a-138">В заметки можно включать ссылки на файлы и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="4d46a-138">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="4d46a-139">Заметки на вкладке **Вложения** не связаны с функциональностью внутренних заметок, которая используется главным образом для обмена информацией между пользователями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="4d46a-139">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="4d46a-140">Дополнительные сведения см. в разделе [Настройка уведомлений рабочего процесса](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="4d46a-140">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="4d46a-141">Следующая процедура основана на заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="4d46a-141">The following procedure is based on a sales order.</span></span> <span data-ttu-id="4d46a-142">Действия для всех остальных поддерживаемых документов и карточек аналогичны.</span><span class="sxs-lookup"><span data-stu-id="4d46a-142">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="4d46a-143">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4d46a-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d46a-144">Выберите заказ на продажу, заметку к которому вы хотите написать, а затем выберите вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="4d46a-144">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="4d46a-145">В разделе **Заметки** выберите значок **+**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-145">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="4d46a-146">В поле **Заметка** введите какой-либо текст, например "Это срочный заказ".</span><span class="sxs-lookup"><span data-stu-id="4d46a-146">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="4d46a-147">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="4d46a-147">Choose the **OK** button.</span></span>

<span data-ttu-id="4d46a-148">Заметка прикреплена к заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="4d46a-148">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="4d46a-149">См. также</span><span class="sxs-lookup"><span data-stu-id="4d46a-149">See Also</span></span>  
<span data-ttu-id="4d46a-150">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4d46a-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="4d46a-151">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="4d46a-151">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="4d46a-152">Настройка уведомлений рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="4d46a-152">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  
