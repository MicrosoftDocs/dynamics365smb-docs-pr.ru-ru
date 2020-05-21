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
ms.date: 04/27/2020
ms.author: sgroespe
ms.openlocfilehash: 9d456fba507977121809124d1de0d23a098406f5
ms.sourcegitcommit: 7d54d8abe52e0546378cf760f5082f46e8441b90
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/30/2020
ms.locfileid: "3324418"
---
# <a name="manage-attachments-links-and-notes-on-cards-and-documents"></a><span data-ttu-id="b352d-103">Управление вложениями, ссылками и заметками в карточках и документах</span><span class="sxs-lookup"><span data-stu-id="b352d-103">Manage Attachments, Links, and Notes on Cards and Documents</span></span>

<span data-ttu-id="b352d-104">В информационных панелях в большинстве карточек и документов можно вкладывать файлы, добавлять ссылки и писать заметки.</span><span class="sxs-lookup"><span data-stu-id="b352d-104">In the FactBox on most cards and documents, you can attach files, add links, and write notes.</span></span> <span data-ttu-id="b352d-105">В случае ссылок и заметок это также можно делать на странице списка, предварительно выбрав соответствующую строку.</span><span class="sxs-lookup"><span data-stu-id="b352d-105">For links and notes, you can also do this on the list page by first selecting the related line.</span></span>

<span data-ttu-id="b352d-106">Чтобы просмотреть или изменить какой-либо из этих прикрепленных типов информации, необходимо сначала открыть вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="b352d-106">To view or change any of these attached information types, you must first open the **Attachments** tab in the FactBox.</span></span> <span data-ttu-id="b352d-107">Цифра в заголовке вкладки показывает, сколько вложенных файлов, ссылок или заметок существует для карточки или документа.</span><span class="sxs-lookup"><span data-stu-id="b352d-107">The number behind the tab title indicates how many attached files, links, or notes exist for the card or document.</span></span>

<span data-ttu-id="b352d-108">Вложения, ссылки и заметки остаются прикрепленными, когда в результате обработки карточка или документ переходят в другое состояние, например когда текущий заказ на продажу превращается в учтенный счет продажи.</span><span class="sxs-lookup"><span data-stu-id="b352d-108">Attachments, links, and notes stay attached as the card or document is processed into other states, such as from an ongoing sales order to a posted sales invoice.</span></span> <span data-ttu-id="b352d-109">Однако ни один из типов вложений не выводится из системы, например при печати или при сохранении в файл.</span><span class="sxs-lookup"><span data-stu-id="b352d-109">However, none of the attachment types are output from the system, for example, when printing or when saving to a file.</span></span>

> [!NOTE]
> <span data-ttu-id="b352d-110">Когда вы делаете частичную откгрузку и выставляете счет по заказу на продажу или покупку, вложение добавляется только к окончательному счету по этому заказу.</span><span class="sxs-lookup"><span data-stu-id="b352d-110">When you partially ship and invoice a sales order or purchase order, the attachment will only be attached to the final invoice of that order.</span></span> <span data-ttu-id="b352d-111">Аналогичным образом, когда вы выставляете счет с использованием функции отсрочки, вложение прикрепляется только к операциям ГК для документа, но не к записям расходов будущих периодов.</span><span class="sxs-lookup"><span data-stu-id="b352d-111">Likewise, when you invoice using the Deferrals feature, the attachment is only attached to the G/L entries for the document but not for the deferral entries.</span></span>

## <a name="to-attach-a-file-to-a-purchase-invoice"></a><span data-ttu-id="b352d-112">Прикрепление файла к счету покупки</span><span class="sxs-lookup"><span data-stu-id="b352d-112">To attach a file to a purchase invoice</span></span>
<span data-ttu-id="b352d-113">К карточке или документу можно прикрепить файл любого типа, содержащий текст, изображение или видео.</span><span class="sxs-lookup"><span data-stu-id="b352d-113">You can attach any type of file, containing text, image, or video, to a card or document.</span></span> <span data-ttu-id="b352d-114">Это удобно делать, например, когда вы хотите сохранить счет поставщика в виде файла PDF в соответствующем счете покупки в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b352d-114">This is useful, for example, when you want to store a vendor's invoice as a PDF file on the related purchase invoice in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

> [!NOTE]
> <span data-ttu-id="b352d-115">Файлы, прикрепленные с помощью функции "Входящие документы", на вкладке **Вложения** не отображаются. Дополнительные сведения см. в разделе [Входящие документы](across-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="b352d-115">Files attached with the Incoming Documents feature are not included on the **Attachments** tab. For more information, see [Incoming Documents](across-income-documents.md).</span></span>

<span data-ttu-id="b352d-116">Следующая процедура основана на счете покупки.</span><span class="sxs-lookup"><span data-stu-id="b352d-116">The following procedure is based on a purchase invoice.</span></span> <span data-ttu-id="b352d-117">Действия для всех остальных поддерживаемых документов и карточек аналогичны.</span><span class="sxs-lookup"><span data-stu-id="b352d-117">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="b352d-118">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b352d-118">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="b352d-119">Откройте заказ на продажу, к которому требуется прикрепить файл.</span><span class="sxs-lookup"><span data-stu-id="b352d-119">Open the sales order that you want to attach a file to.</span></span>
3. <span data-ttu-id="b352d-120">В информационной панели откройте вкладку **Вложения**.</span><span class="sxs-lookup"><span data-stu-id="b352d-120">In the FactBox, open the **Attachments** tab.</span></span>
4. <span data-ttu-id="b352d-121">Выберите значение за полем **Документы**, например "0".</span><span class="sxs-lookup"><span data-stu-id="b352d-121">Choose the value behind the **Documents** field, such as "0".</span></span>
5. <span data-ttu-id="b352d-122">На странице **Вложенные документы** в поле **Вложение** выберите действие **Выбрать файл**.</span><span class="sxs-lookup"><span data-stu-id="b352d-122">On the **Attached Documents** page, in the **Attachment** field, choose the **Select File** action.</span></span>
5. <span data-ttu-id="b352d-123">Выберите файл из любого расположения, затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="b352d-123">Select a file from any location, and then choose the **Open** button.</span></span>

<span data-ttu-id="b352d-124">Файл прикреплен к счету покупки.</span><span class="sxs-lookup"><span data-stu-id="b352d-124">The file is now attached to the purchase invoice.</span></span>

## <a name="to-view-an-attached-file"></a><span data-ttu-id="b352d-125">Просмотр вложенного файла</span><span class="sxs-lookup"><span data-stu-id="b352d-125">To view an attached file</span></span>
1. <span data-ttu-id="b352d-126">В информационной панели откройте вкладку **Вложения**.</span><span class="sxs-lookup"><span data-stu-id="b352d-126">In the FactBox, open the **Attachments** tab.</span></span>
2. <span data-ttu-id="b352d-127">Выберите значение за полем **Документы**, например "1".</span><span class="sxs-lookup"><span data-stu-id="b352d-127">Choose the value behind the **Documents** field, such as "1".</span></span>
3. <span data-ttu-id="b352d-128">На странице **Вложенные документы** выберите действие **Предварительный просмотр**.</span><span class="sxs-lookup"><span data-stu-id="b352d-128">On the **Attached Documents** page, choose the **Preview** action.</span></span>
4. <span data-ttu-id="b352d-129">Откройте загруженный файл.</span><span class="sxs-lookup"><span data-stu-id="b352d-129">Open the downloaded file.</span></span>

## <a name="to-save-a-document-as-a-pdf-attachment"></a><span data-ttu-id="b352d-130">Чтобы сохранить документ в виде PDF-вложения</span><span class="sxs-lookup"><span data-stu-id="b352d-130">To save a document as a PDF attachment</span></span>
<span data-ttu-id="b352d-131">Всякий раз, когда вам нужно сохранить документ в виде файла, вы можете использовать действие **Вложить как PDF** для захвата содержимого текущего документа в виде файла PDF, прикрепленного к информационной панели документа.</span><span class="sxs-lookup"><span data-stu-id="b352d-131">Whenever you need to save a document as a file, you can use the **Attach as PDF** action to capture the current document content as a PDF file attached to the FactBox of the document.</span></span> <span data-ttu-id="b352d-132">Это полезно, например, когда документы сопровождают несколько этапов процесса, такого как процесс продажи или рабочий процесс утверждения, и вы хотите сослаться на распечатку предыдущего шага.</span><span class="sxs-lookup"><span data-stu-id="b352d-132">This is useful, for example, when documents follow multiple steps in a process, such as a sales process or an approval workflow, and you want to refer to a printout of the previous step.</span></span>

<span data-ttu-id="b352d-133">Следующая процедура основана на заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="b352d-133">The following procedure is based on a sales order.</span></span> <span data-ttu-id="b352d-134">Шаги аналогичны для всех поддерживаемых документов.</span><span class="sxs-lookup"><span data-stu-id="b352d-134">The steps are similar for all supported documents.</span></span>

1. <span data-ttu-id="b352d-135">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b352d-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b352d-136">Выберите заказ на продажу, затем выберите действие **Вложить как PDF**.</span><span class="sxs-lookup"><span data-stu-id="b352d-136">Select a sales order, and then choose the **Attach as PDF** action.</span></span>

<span data-ttu-id="b352d-137">PDF-файл с текущим содержимым заказа на продажу добавляется на вкладку **Вложения** на информационной панели.</span><span class="sxs-lookup"><span data-stu-id="b352d-137">A PDF file with the current content of the sales order is added to the **Attachments** tab in the FactBox.</span></span>

## <a name="to-add-a-link-from-an-item-card"></a><span data-ttu-id="b352d-138">Добавление ссылки из карточки товара</span><span class="sxs-lookup"><span data-stu-id="b352d-138">To add a link from an item card</span></span>
<span data-ttu-id="b352d-139">Можно добавить ссылку из карточки или документа на любой URL-адрес или путь.</span><span class="sxs-lookup"><span data-stu-id="b352d-139">You can add a link from a card or document to any URL or path.</span></span> <span data-ttu-id="b352d-140">Это удобно делать, например, когда вы хотите связать карточку товара с каталогом товаров поставщика.</span><span class="sxs-lookup"><span data-stu-id="b352d-140">This is useful, for example, when you want to link an item card with the supplier's item catalog.</span></span>

<span data-ttu-id="b352d-141">Следующая процедура основана на карточке товара.</span><span class="sxs-lookup"><span data-stu-id="b352d-141">The following procedure is based on an item card.</span></span> <span data-ttu-id="b352d-142">Действия для всех остальных поддерживаемых карточек и документов аналогичны.</span><span class="sxs-lookup"><span data-stu-id="b352d-142">The steps are similar for all other supported cards and documents.</span></span>

1. <span data-ttu-id="b352d-143">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b352d-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="b352d-144">Выберите товар, ссылку из которого вы хотите добавить, а затем выберите вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="b352d-144">Select the item that you want to add a link from, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="b352d-145">В разделе **Ссылки** выберите значок **+**.</span><span class="sxs-lookup"><span data-stu-id="b352d-145">In the **Links**, choose the **+** icon.</span></span>
4. <span data-ttu-id="b352d-146">В поле **Адрес ссылки** введите ссылку.</span><span class="sxs-lookup"><span data-stu-id="b352d-146">In the **Link Address** field, enter the link.</span></span>

    <span data-ttu-id="b352d-147">Ссылка должна быть действительным URL-адресом в Интернете или интрасети.</span><span class="sxs-lookup"><span data-stu-id="b352d-147">The link must be a valid internet or intranet URL.</span></span>

5. <span data-ttu-id="b352d-148">В поле **Описание** введите информацию о ссылке, если необходимо.</span><span class="sxs-lookup"><span data-stu-id="b352d-148">In the **Description** field, enter any information about the link.</span></span>  
6. <span data-ttu-id="b352d-149">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b352d-149">Choose the **OK** button.</span></span>

<span data-ttu-id="b352d-150">Ссылка прикреплена к карточке товара.</span><span class="sxs-lookup"><span data-stu-id="b352d-150">The link is now attached to the item card.</span></span>  

## <a name="to-write-a-note-on-a-sales-order"></a><span data-ttu-id="b352d-151">Написание заметки о заказе на продажу</span><span class="sxs-lookup"><span data-stu-id="b352d-151">To write a note on a sales order</span></span>
<span data-ttu-id="b352d-152">Вы можете написать заметку к документе или карточке, — например, чтобы предоставить особые указания для других пользователей документа или карточки.</span><span class="sxs-lookup"><span data-stu-id="b352d-152">You can write a note on a document or card, for example, to communicate special instructions to other users of the document or card.</span></span> <span data-ttu-id="b352d-153">В заметки можно включать ссылки на файлы и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="b352d-153">You can include file links and URLs in notes.</span></span>

> [!NOTE]
> <span data-ttu-id="b352d-154">Заметки на вкладке **Вложения** не связаны с функциональностью внутренних заметок, которая используется главным образом для обмена информацией между пользователями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="b352d-154">Notes on the **Attachments** tab are not related to internal notes functionality, which is mainly used to communicate between workflow users.</span></span> <span data-ttu-id="b352d-155">Дополнительные сведения см. в разделе [Настройка уведомлений рабочего процесса](across-setting-up-workflow-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="b352d-155">For more information, see [Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md).</span></span>

<span data-ttu-id="b352d-156">Следующая процедура основана на заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="b352d-156">The following procedure is based on a sales order.</span></span> <span data-ttu-id="b352d-157">Действия для всех остальных поддерживаемых документов и карточек аналогичны.</span><span class="sxs-lookup"><span data-stu-id="b352d-157">The steps are similar for all other supported documents and cards.</span></span>

1. <span data-ttu-id="b352d-158">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b352d-158">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="b352d-159">Выберите заказ на продажу, заметку к которому вы хотите написать, а затем выберите вкладку **Вложения** в информационной панели.</span><span class="sxs-lookup"><span data-stu-id="b352d-159">Select the sales order that you want to write a note on, and then choose the **Attachments** tab in the FactBox.</span></span>
3. <span data-ttu-id="b352d-160">В разделе **Заметки** выберите значок **+**.</span><span class="sxs-lookup"><span data-stu-id="b352d-160">In the **Notes** section, choose the **+** icon.</span></span>
4. <span data-ttu-id="b352d-161">В поле **Заметка** введите какой-либо текст, например "Это срочный заказ".</span><span class="sxs-lookup"><span data-stu-id="b352d-161">In the **Note** field, write any text, such as "This is an urgent order.".</span></span>
5. <span data-ttu-id="b352d-162">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b352d-162">Choose the **OK** button.</span></span>

<span data-ttu-id="b352d-163">Заметка прикреплена к заказу на продажу.</span><span class="sxs-lookup"><span data-stu-id="b352d-163">The note is now attached to the sales order.</span></span>

## <a name="see-also"></a><span data-ttu-id="b352d-164">См. также</span><span class="sxs-lookup"><span data-stu-id="b352d-164">See Also</span></span>  
<span data-ttu-id="b352d-165">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b352d-165">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="b352d-166">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="b352d-166">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="b352d-167">Настройка уведомлений рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="b352d-167">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)  
