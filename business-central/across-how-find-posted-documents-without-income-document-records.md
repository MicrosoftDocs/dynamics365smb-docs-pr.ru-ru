---
title: Поиск документов без вложений| Документация Майкрософт
Description: Вы можете осуществлять поиск операций главной книги для учтенных документов покупок и продаж, у которых нет входящих электронных документов, например для импортированных счетов.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 75615d653c21ea62af2c621c892010ee985f1166
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5384678"
---
# <a name="find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="b7bca-103">Поиск учтенных документов без записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="b7bca-103">Find Posted Documents without Incoming Document Records</span></span>
<span data-ttu-id="b7bca-104">На страницах **План счетов** и **Операции главной книги** с помощью функции поиска можно найти операции главной книги для учтенных документов покупки и продажи, которые не имеют записей входящих документов, и затем централизованно связать их с существующими записями или создать новые записи с прикрепленными файлами документов.</span><span class="sxs-lookup"><span data-stu-id="b7bca-104">From the **Chart of Accounts** and **General Ledger Entries** pages, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span>

## <a name="to-find-posted-documents-without-incoming-document-records"></a><span data-ttu-id="b7bca-105">Поиск учтенных документов без записей входящих документов</span><span class="sxs-lookup"><span data-stu-id="b7bca-105">To find posted documents without incoming document records</span></span>
1. <span data-ttu-id="b7bca-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **План счетов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="b7bca-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="b7bca-107">Выберите строку счета ГК для тех операций главной книги, для которых вы ходите увидеть учтенные документы покупки и продажи без записей входящих документов, а затем выберите действие **Учтенные документы без входящего документа**.</span><span class="sxs-lookup"><span data-stu-id="b7bca-107">Select a line for a G/L account for whose general ledger entries you want to see posted purchase and sales documents without incoming document records, and then choose the **Posted Documents without Incoming Document** action.</span></span>
3. <span data-ttu-id="b7bca-108">Альтернативный вариант — выберите действие **Книга операций**.</span><span class="sxs-lookup"><span data-stu-id="b7bca-108">Alternatively, choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="b7bca-109">На странице **Операции главной книги** выберите действие **Учтенные документы без входящих документов**.</span><span class="sxs-lookup"><span data-stu-id="b7bca-109">On the **General Ledger Entries** page, choose the **Posted Documents without Incoming Documents** action.</span></span>

<span data-ttu-id="b7bca-110">Откроется страница **Учтенные документы без входящего документа**, содержащее сведения об учтенных документах покупки и продажи без записей входящего документа, представленных записями ГК в счете ГК, для которого открыто эту страницу.</span><span class="sxs-lookup"><span data-stu-id="b7bca-110">The **Posted Documents without Incoming Document** page opens showing posted purchase and sales documents without incoming document records represented by general ledger entries on the G/L account that you opened the page for.</span></span> <span data-ttu-id="b7bca-111">Страница может содержать до 1000 строк.</span><span class="sxs-lookup"><span data-stu-id="b7bca-111">The page can show a maximum of 1000 lines.</span></span> <span data-ttu-id="b7bca-112">Таким образом, по умолчанию поле **Фильтр по дате** содержит фильтр, который ограничивает строки записями, имеющими дату учета с начала отчетного периода до рабочей даты.</span><span class="sxs-lookup"><span data-stu-id="b7bca-112">By default, the **Date Filter** field therefore contains a filter that limits the lines to entries with posting dates from the beginning of the accounting period to the work date.</span></span>

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a><span data-ttu-id="b7bca-113">Подключение найденных документов к существующим записям входящих документов</span><span class="sxs-lookup"><span data-stu-id="b7bca-113">To connect found documents to existing incoming document records</span></span>
1. <span data-ttu-id="b7bca-114">На странице **Учтенные документы без входящего документа** выберите строку для учтенного документа, который нужно связать с существующей записью входящего документа, и выберите действие **Выбрать входящий документ**.</span><span class="sxs-lookup"><span data-stu-id="b7bca-114">On the **Posted Documents without Incoming Document** page, select the line for a posted document that you want to connect to an existing incoming document record, and then choose the **Select Incoming Document** action.</span></span>
2. <span data-ttu-id="b7bca-115">На странице **Входящие документы** выберите запись входящего документа, которую требуется связать с найденным учтенным документом, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b7bca-115">On the **Incoming Documents** page, select the incoming document record that you want to connect to posted document found, and then choose the **OK** button.</span></span>
3. <span data-ttu-id="b7bca-116">На странице **Учтенные документы без входящего документа** выбранная запись входящего документа будет связана с учтенным документом, как показано на информационной панели **Файлы входящих документов** .</span><span class="sxs-lookup"><span data-stu-id="b7bca-116">On the **Posted Documents without Incoming Document** page, the selected incoming document record is now connected to the posted document, as you can see in the **Incoming Document Files** FactBox.</span></span>

<span data-ttu-id="b7bca-117">Если нужная запись входящего документа отсутствует на странице **Входящие документы**, ее можно создать.</span><span class="sxs-lookup"><span data-stu-id="b7bca-117">If a relevant incoming document record does not exist on the **Incoming Documents** page, then you can create it.</span></span> <span data-ttu-id="b7bca-118">Дополнительные сведения см. в разделе [Создание записей входящих документов](across-how-create-income-document-records.md).</span><span class="sxs-lookup"><span data-stu-id="b7bca-118">For more information, see [Create Incoming Document Records](across-how-create-income-document-records.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="b7bca-119">См. также</span><span class="sxs-lookup"><span data-stu-id="b7bca-119">See Also</span></span>
[<span data-ttu-id="b7bca-120">Обработка входящих документов</span><span class="sxs-lookup"><span data-stu-id="b7bca-120">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="b7bca-121">Входящие документы</span><span class="sxs-lookup"><span data-stu-id="b7bca-121">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="b7bca-122">Покупки</span><span class="sxs-lookup"><span data-stu-id="b7bca-122">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="b7bca-123">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b7bca-123">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]