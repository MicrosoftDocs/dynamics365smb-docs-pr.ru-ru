---
title: Поиск записей | Документация Microsoft
description: В этой статье описывается, как работать с документами и записями, которые связаны
author: jswymer
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.date: 04/01/2021
ms.author: jswymer
ms.openlocfilehash: 5f8ddd7176e69c9d1eb3b8d8ff98c93695d50993
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771165"
---
# <a name="finding-related-entries-for-posted-documents"></a><span data-ttu-id="b93ed-103">Поиск связанных записей для учтенных документов</span><span class="sxs-lookup"><span data-stu-id="b93ed-103">Finding Related Entries for Posted Documents</span></span> 

<span data-ttu-id="b93ed-104">В этой статье вы узнаете, как найти документы и записи, связанные друг с другом, на основе общей информации, например:</span><span class="sxs-lookup"><span data-stu-id="b93ed-104">In this article, you learn how to find documents and entries that are related to each other based on a common information, like:</span></span>

- <span data-ttu-id="b93ed-105">Номер документа или дата проводки</span><span class="sxs-lookup"><span data-stu-id="b93ed-105">Document number or posting date</span></span>
- <span data-ttu-id="b93ed-106">Тип делового контакта, номер или номер внешнего документа</span><span class="sxs-lookup"><span data-stu-id="b93ed-106">Business contact type, number, or external document number</span></span>
- <span data-ttu-id="b93ed-107">Серийный номер товара или номер партии</span><span class="sxs-lookup"><span data-stu-id="b93ed-107">Item serial number or lot number</span></span>

<span data-ttu-id="b93ed-108">Эта функция полезна для поиска операций книги, которые стали результатом определенных транзакций.</span><span class="sxs-lookup"><span data-stu-id="b93ed-108">This feature is useful for finding the ledger entries that resulted from certain transactions.</span></span> <span data-ttu-id="b93ed-109">При поиске по номеру документа можно также распечатывать сводку из отчета "Операции с документами".</span><span class="sxs-lookup"><span data-stu-id="b93ed-109">When you search by document number, you can print the summary from the Document Entries report.</span></span>

## <a name="get-started"></a><span data-ttu-id="b93ed-110">Начало работы</span><span class="sxs-lookup"><span data-stu-id="b93ed-110">Get started</span></span>

<span data-ttu-id="b93ed-111">Функция поиска записей доступна на большинстве страниц, на которых отображаются опубликованные документы или операции опубликованных документов — как для списков, так и для карточек.</span><span class="sxs-lookup"><span data-stu-id="b93ed-111">The find entries feature is readily available on most pages that display posted documents or posted documents entries - for both lists and cards.</span></span> <span data-ttu-id="b93ed-112">Итак, первый шаг — открыть одну из этих страниц.</span><span class="sxs-lookup"><span data-stu-id="b93ed-112">So the first step is open one of these pages.</span></span> <span data-ttu-id="b93ed-113">Затем либо выберите действие **Найти записи** или нажмите клавиши Alt+G.</span><span class="sxs-lookup"><span data-stu-id="b93ed-113">Then, either choose the **Find Entries** action or press the Alt+G keys.</span></span>

<span data-ttu-id="b93ed-114">На странице **Найти записи** включает все связанные документы и операции на основе номера документа и даты учета.</span><span class="sxs-lookup"><span data-stu-id="b93ed-114">The **Find Entries** page  includes all related documents and entries based on the document no. and posting date.</span></span> <span data-ttu-id="b93ed-115">Страница разделена на три раздела:</span><span class="sxs-lookup"><span data-stu-id="b93ed-115">The page is divided into three sections:</span></span>

- <span data-ttu-id="b93ed-116">В верхнем разделе отображаются поля и действия, которые вы используете для фильтрации поиска.</span><span class="sxs-lookup"><span data-stu-id="b93ed-116">The top section displays fields and actions that you use for filtering your search.</span></span>
- <span data-ttu-id="b93ed-117">В среднем разделе отображаются связанные документы на основе результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b93ed-117">The middle section displays related documents based on the search.</span></span>
- <span data-ttu-id="b93ed-118">В нижнем разделе отображается информация об исходном документе, найденном при поиске.</span><span class="sxs-lookup"><span data-stu-id="b93ed-118">The bottom section displays information about the source document that was found by searching.</span></span>


<!--
 There are two ways to open this page:

- Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then choose the related link.

    With this way, the **Find Entries** page might be empty, and you'll have to start searching for entries from scratch.
    
- Open a page that displays posted documents or posted documents entries, either a list or a card. Then, locate and select the **Find Entries** action.

    With this way, the **Find Entries**, page will include all related documents and entries based on the document no. and posting date.


    > [!TIP]
    > If you are on a page that has the **Find Entries** action, press crtl+G to open the **Find Entries** page directly. 
-->

## <a name="search-for-entries"></a><span data-ttu-id="b93ed-119">Искать операции</span><span class="sxs-lookup"><span data-stu-id="b93ed-119">Search for entries</span></span>

<span data-ttu-id="b93ed-120">Вы можете искать операции на основе информации о документе, деловом контакте или товаре.</span><span class="sxs-lookup"><span data-stu-id="b93ed-120">You can search for entries based on information about either the document, business contact, or item reference.</span></span> <span data-ttu-id="b93ed-121">Чтобы изменить поиск, выберите **Действия**, **Найти по**, затем одно из следующих действий:</span><span class="sxs-lookup"><span data-stu-id="b93ed-121">To change the search, select **Actions**, **Find By**, then one of the following actions:</span></span>

|<span data-ttu-id="b93ed-122">Действие</span><span class="sxs-lookup"><span data-stu-id="b93ed-122">Action</span></span>|<span data-ttu-id="b93ed-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b93ed-123">Description</span></span>|
|------|-----------|
|<span data-ttu-id="b93ed-124">Найти по документу</span><span class="sxs-lookup"><span data-stu-id="b93ed-124">Find by Document</span></span>|<span data-ttu-id="b93ed-125">Просмотр операций на основе определенного номера документа или даты публикации.</span><span class="sxs-lookup"><span data-stu-id="b93ed-125">View entries based on a specific document number or posting date.</span></span>|
|<span data-ttu-id="b93ed-126">Бизнес-контакт</span><span class="sxs-lookup"><span data-stu-id="b93ed-126">Business Contact</span></span> |<span data-ttu-id="b93ed-127">Просматривайте записи на основе определенного типа контакта, контактного номера, и/или внешнего номера документа.</span><span class="sxs-lookup"><span data-stu-id="b93ed-127">View entries based on a specific contact type, contact number, anr/or external document number.</span></span> <span data-ttu-id="b93ed-128">Можно ввести информацию о документе, назначенную поставщиком или клиентом.</span><span class="sxs-lookup"><span data-stu-id="b93ed-128">You can enter document information that was assigned by a vendor or a customer.</span></span> <span data-ttu-id="b93ed-129">Используйте доступные поля для поиска документов поставщика с использованием номеров, которые поставщик присвоил документам.</span><span class="sxs-lookup"><span data-stu-id="b93ed-129">Use the available fields to search for vendor documents by using the numbers that the vendor has assigned the documents.</span></span>|
|<span data-ttu-id="b93ed-130">Ссылка на товар</span><span class="sxs-lookup"><span data-stu-id="b93ed-130">Item reference</span></span>|<span data-ttu-id="b93ed-131">Просмотр записей по серийному номеру или номеру партии.</span><span class="sxs-lookup"><span data-stu-id="b93ed-131">View entires based on a serial number or lot number.</span></span> <span data-ttu-id="b93ed-132">Можно ввести номер партии или серийный номер либо отфильтровать по номеру партии или серийному номеру, по которым необходимо выполнить поиск.</span><span class="sxs-lookup"><span data-stu-id="b93ed-132">You can enter the lot number or serial number, or filter on the lot number or serial number that you want to search for.</span></span> <span data-ttu-id="b93ed-133">Это действие используется, чтобы увидеть, где использовался конкретный номер трассировки товаров, от какого поставщика он получен или какому клиенту продан.</span><span class="sxs-lookup"><span data-stu-id="b93ed-133">This action is useful to see where a specific item tracking number was used, what vendor it came from, or what customer it was sold to.</span></span>|

<span data-ttu-id="b93ed-134">После того, как вы сделаете выбор, введите релевантную поисковую информацию в поля вверху.</span><span class="sxs-lookup"><span data-stu-id="b93ed-134">After you make a selection, enter the relevant search information in the fields at the top.</span></span> <span data-ttu-id="b93ed-135">Используйте всплывающие подсказки на полях.</span><span class="sxs-lookup"><span data-stu-id="b93ed-135">Use the tooltips on the fields to help.</span></span> <span data-ttu-id="b93ed-136">Когда вы закончите, выберите **Найти**, чтобы начать поиск.</span><span class="sxs-lookup"><span data-stu-id="b93ed-136">When you're finished, choose **Find** to start the search.</span></span> <span data-ttu-id="b93ed-137">Если изменить любые фильтры, следует снова выбрать **Найти**.</span><span class="sxs-lookup"><span data-stu-id="b93ed-137">If you change any of the filters, you have to choose **Find** again.</span></span>

> [!TIP]
> <span data-ttu-id="b93ed-138">Для пары примеров использования **Найти записи** см. [Трассировка товаров, трассируемых по товарам](inventory-how-to-trace-item-tracked-items.md) и [Пошаговое руководство. Трассировка серийных номеров и номеров партии](walkthrough-tracing-serial-lot-numbers.md).</span><span class="sxs-lookup"><span data-stu-id="b93ed-138">For a couple examples about using **Find Entries**, see [Trace Item-Tracked Items](inventory-how-to-trace-item-tracked-items.md) and [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="b93ed-139">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/user-interface-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="b93ed-139">See Related Training at [Microsoft Learn](/learn/modules/user-interface-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="b93ed-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b93ed-140">See Also</span></span>

[<span data-ttu-id="b93ed-141">Работа с Business Central</span><span class="sxs-lookup"><span data-stu-id="b93ed-141">Working with Business Central</span></span>](ui-work-product.md)  
[<span data-ttu-id="b93ed-142">Добавление действия страницы в ролевой центр</span><span class="sxs-lookup"><span data-stu-id="b93ed-142">Add a Page Action to Your Role Center</span></span>](ui-bookmarks.md)  
[<span data-ttu-id="b93ed-143">Трассировка товаров, трассируемых по товарам</span><span class="sxs-lookup"><span data-stu-id="b93ed-143">Trace Item-Tracked Items</span></span>](inventory-how-to-trace-item-tracked-items.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]