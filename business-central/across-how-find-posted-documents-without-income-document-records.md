---
title: "Поиск документов без вложений| Microsoft Docs"
Description: You can search for general ledger entries for posted purchase and sales documents that do not have incoming electronic documents, such as imported invoices.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 34bbc67c0f2bcc5afe408e75a7d3ceb582160d87
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="e82c6-102">Поиск учтенных документов без записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="e82c6-102">Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="e82c6-103">На страницах **План счетов** и **Операции главной книги** с помощью функции поиска можно найти операции главной книги для учтенных документов покупки и продажи, которые не имеют записей входящих документов, и затем централизованно связать их с существующими записями или создать новые записи с прикрепленными файлами документов.</span><span class="sxs-lookup"><span data-stu-id="e82c6-103">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="e82c6-104">Поиск учтенных документов без записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="e82c6-104">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="e82c6-105">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **План счетов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e82c6-105">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="e82c6-106">Выберите строку счета ГК для тех операций главной книги, для которых вы ходите увидеть учтенные документы покупки и продажи без записей входящих документов, а затем выберите действие **Учтенные документы без входящего документа**.</span><span class="sxs-lookup"><span data-stu-id="e82c6-106">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="e82c6-107">Альтернативный вариант — выберите действие **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="e82c6-107">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="e82c6-108">На странице **Операции главной книги** выберите действие **Учтенные документы без входящих документов**.</span><span class="sxs-lookup"><span data-stu-id="e82c6-108">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="e82c6-109">Откроется страница **Учтенные документы без входящего документа**, содержащее сведения об учтенных документах покупки и продажи без записей входящего документа, представленных записями ГК в счете ГК, для которого открыто эту страницу.</span><span class="sxs-lookup"><span data-stu-id="e82c6-109">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span></span> <span data-ttu-id="e82c6-110">Страница может содержать до 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="e82c6-110">The page can show a maximum of 1000 lines.</span></span> <span data-ttu-id="e82c6-111">Таким образом, по умолчанию поле **Фильтр по дате** содержит фильтр, который ограничивает строки записями, имеющими дату учета с начала отчетного периода до рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="e82c6-111">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="e82c6-112">Подключение найденных документов к существующим записям входящих документов</span><span class="sxs-lookup"><span data-stu-id="e82c6-112">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="e82c6-113">На странице **Учтенные документы без входящего документа** выберите строку для учтенного документа, который нужно связать с существующей записью входящего документа, и выберите действие **Выбрать входящий документ**.</span><span class="sxs-lookup"><span data-stu-id="e82c6-113">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="e82c6-114">На странице **Входящие документы** выберите запись входящего документа, которую требуется связать с найденным учтенным документом, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="e82c6-114">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="e82c6-115">На странице **Учтенные документы без входящего документа** выбранная запись входящего документа будет связана с учтенным документом, как показано на информационной панели **Файлы входящих документов** .</span><span class="sxs-lookup"><span data-stu-id="e82c6-115">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="e82c6-116">Если нужная запись входящего документа отсутствует на странице **Входящие документы**, ее можно создать.</span><span class="sxs-lookup"><span data-stu-id="e82c6-116">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span></span> <span data-ttu-id="e82c6-117">Дополнительные сведения см. в разделе [Создание записей входящих документов](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="e82c6-117">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="e82c6-118">См. также</span><span class="sxs-lookup"><span data-stu-id="e82c6-118">See Also</span></span>
[<span data-ttu-id="e82c6-119">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="e82c6-119">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="e82c6-120">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="e82c6-120">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="e82c6-121">Покупки</span><span class="sxs-lookup"><span data-stu-id="e82c6-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="e82c6-122">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e82c6-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

