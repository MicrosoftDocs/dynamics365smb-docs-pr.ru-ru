---
title: "Как архивировать документы о продажах и покупке | Документы Майкрософт"
description: "Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 74460bfcff36d293006229f4a89719f8c05c2631
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="archive-documents"></a><span data-ttu-id="2a53e-103">Архивирование документов</span><span class="sxs-lookup"><span data-stu-id="2a53e-103">Archive Documents</span></span>
<span data-ttu-id="2a53e-104">Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован.</span><span class="sxs-lookup"><span data-stu-id="2a53e-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span></span>

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="2a53e-105">Настройка автоматического архивирования документов</span><span class="sxs-lookup"><span data-stu-id="2a53e-105">To set up automatic document archiving</span></span>  
<span data-ttu-id="2a53e-106">Можно настроить автоматическое архивирование заказов продаж и покупки, предложений, общих заказов и заказов на возврат перед удалением документов.</span><span class="sxs-lookup"><span data-stu-id="2a53e-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="2a53e-107">Следующая процедура описывает, как настроить автоматическое архивирование документов продажи.</span><span class="sxs-lookup"><span data-stu-id="2a53e-107">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="2a53e-108">Действия для документов на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="2a53e-108">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="2a53e-109">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Настройка модуля "Продажи"**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2a53e-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="2a53e-110">В окне **Настройка модуля "Продажи"** заполните поля следующим образом:</span><span class="sxs-lookup"><span data-stu-id="2a53e-110">In the **Sales & Receivables Setup** window, fill in the fields as follows.</span></span>

|<span data-ttu-id="2a53e-111">Поле</span><span class="sxs-lookup"><span data-stu-id="2a53e-111">Field</span></span>|<span data-ttu-id="2a53e-112">Описанием</span><span class="sxs-lookup"><span data-stu-id="2a53e-112">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="2a53e-113">**Архивирование предложений по продаже**</span><span class="sxs-lookup"><span data-stu-id="2a53e-113">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="2a53e-114">**Никогда**, чтобы никогда не архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="2a53e-114">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="2a53e-115">**Вопрос**, чтобы предлагать пользователю выбрать, требуется ли архивировать предложения по продаже перед их удалением.</span><span class="sxs-lookup"><span data-stu-id="2a53e-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="2a53e-116">**Всегда**, чтобы автоматически архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="2a53e-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="2a53e-117">**Архивирование общих заказов на продажу**</span><span class="sxs-lookup"><span data-stu-id="2a53e-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="2a53e-118">Выберите для автоматического архивирования общих заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="2a53e-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="2a53e-119">**Архивировать заказы и заказы на возврат**</span><span class="sxs-lookup"><span data-stu-id="2a53e-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="2a53e-120">Выберите для автоматического архивирования заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="2a53e-120">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="2a53e-121">Архивирование заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="2a53e-121">To archive a sales order</span></span>
<span data-ttu-id="2a53e-122">Следующая процедура описывает, как архивировать заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="2a53e-122">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="2a53e-123">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="2a53e-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="2a53e-124">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Заказы на продажу**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2a53e-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2a53e-125">Откройте заказ на продажу, который требуется архивировать.</span><span class="sxs-lookup"><span data-stu-id="2a53e-125">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="2a53e-126">Выберите действие **Архивировать документ**.</span><span class="sxs-lookup"><span data-stu-id="2a53e-126">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="2a53e-127">Заказ на продажу архивирован.</span><span class="sxs-lookup"><span data-stu-id="2a53e-127">The sales order is archived.</span></span> <span data-ttu-id="2a53e-128">Его можно просмотреть в окне **Архивные заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="2a53e-128">You can view it in the **Archived Sales orders** window.</span></span> <span data-ttu-id="2a53e-129">Отсюда его также можно использовать для восстановления заказа на продажу, из которого был создан архив.</span><span class="sxs-lookup"><span data-stu-id="2a53e-129">From here, you can also use it to recreate the sales order that it was archived from.</span></span>

## <a name="to-recreate-a-sales-order-from-the-archive"></a><span data-ttu-id="2a53e-130">Восстановление заказа на продажу из архива</span><span class="sxs-lookup"><span data-stu-id="2a53e-130">To recreate a sales order from the archive</span></span>
<span data-ttu-id="2a53e-131">Следующая процедура описывает, как восстановить заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="2a53e-131">The following procedure describes how to recreate a sales order.</span></span> <span data-ttu-id="2a53e-132">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="2a53e-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="2a53e-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Архивированные заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2a53e-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2.  <span data-ttu-id="2a53e-134">Выберите архивированный заказ на продажу, который требуется восстановить, затем выберите действие **Восстановить**.</span><span class="sxs-lookup"><span data-stu-id="2a53e-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="2a53e-135">Заказ на продажу создается и добавляется в окно **Заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="2a53e-135">The sales order is created and added to the **Sales Orders** window.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="2a53e-136">Удаление архивных заказов продажу</span><span class="sxs-lookup"><span data-stu-id="2a53e-136">To delete archived sales orders</span></span>
<span data-ttu-id="2a53e-137">Следующая процедура описывает, как удалить архивные заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="2a53e-137">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="2a53e-138">Шаги аналогичны для всех остальных архивных документов продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="2a53e-138">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="2a53e-139">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Удалить архивные версии заказов продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="2a53e-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2a53e-140">В окне **Удалить архивные версии заказов продажи** выберите соответствующие фильтры.</span><span class="sxs-lookup"><span data-stu-id="2a53e-140">In the **Delete Archived Sales Order Versions** window, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="2a53e-141">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="2a53e-141">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="2a53e-142">См. также</span><span class="sxs-lookup"><span data-stu-id="2a53e-142">See Also</span></span>
[<span data-ttu-id="2a53e-143">Отслеживание строк документа</span><span class="sxs-lookup"><span data-stu-id="2a53e-143">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="2a53e-144">Продажи</span><span class="sxs-lookup"><span data-stu-id="2a53e-144">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="2a53e-145">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="2a53e-145">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="2a53e-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2a53e-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

