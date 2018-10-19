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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 6b1b23c062fdb1c4558a292c7aa454ae24ff3c71
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="archive-documents"></a><span data-ttu-id="54c81-103">Архивирование документов</span><span class="sxs-lookup"><span data-stu-id="54c81-103">Archive Documents</span></span>
<span data-ttu-id="54c81-104">Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован.</span><span class="sxs-lookup"><span data-stu-id="54c81-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span></span>

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="54c81-105">Настройка автоматического архивирования документов</span><span class="sxs-lookup"><span data-stu-id="54c81-105">To set up automatic document archiving</span></span>  
<span data-ttu-id="54c81-106">Можно настроить автоматическое архивирование заказов продаж и покупки, предложений, общих заказов и заказов на возврат перед удалением документов.</span><span class="sxs-lookup"><span data-stu-id="54c81-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="54c81-107">Следующая процедура описывает, как настроить автоматическое архивирование документов продажи.</span><span class="sxs-lookup"><span data-stu-id="54c81-107">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="54c81-108">Действия для документов на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="54c81-108">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="54c81-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи"**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c81-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="54c81-110">В окне **Настройка модуля "Продажи"** заполните поля следующим образом:</span><span class="sxs-lookup"><span data-stu-id="54c81-110">In the **Sales & Receivables Setup** window, fill in the fields as follows.</span></span>

|<span data-ttu-id="54c81-111">Поле</span><span class="sxs-lookup"><span data-stu-id="54c81-111">Field</span></span>|<span data-ttu-id="54c81-112">Описанием</span><span class="sxs-lookup"><span data-stu-id="54c81-112">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="54c81-113">**Архивирование предложений по продаже**</span><span class="sxs-lookup"><span data-stu-id="54c81-113">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="54c81-114">**Никогда**, чтобы никогда не архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="54c81-114">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="54c81-115">**Вопрос**, чтобы предлагать пользователю выбрать, требуется ли архивировать предложения по продаже перед их удалением.</span><span class="sxs-lookup"><span data-stu-id="54c81-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="54c81-116">**Всегда**, чтобы автоматически архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="54c81-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="54c81-117">**Архивирование общих заказов на продажу**</span><span class="sxs-lookup"><span data-stu-id="54c81-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="54c81-118">Выберите для автоматического архивирования общих заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="54c81-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="54c81-119">**Архивировать заказы и заказы на возврат**</span><span class="sxs-lookup"><span data-stu-id="54c81-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="54c81-120">Выберите для автоматического архивирования заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="54c81-120">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="54c81-121">Архивирование заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="54c81-121">To archive a sales order</span></span>
<span data-ttu-id="54c81-122">Следующая процедура описывает, как архивировать заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="54c81-122">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="54c81-123">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="54c81-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="54c81-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c81-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="54c81-125">Откройте заказ на продажу, который требуется архивировать.</span><span class="sxs-lookup"><span data-stu-id="54c81-125">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="54c81-126">Выберите действие **Архивировать документ**.</span><span class="sxs-lookup"><span data-stu-id="54c81-126">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="54c81-127">Заказ на продажу архивирован.</span><span class="sxs-lookup"><span data-stu-id="54c81-127">The sales order is archived.</span></span> <span data-ttu-id="54c81-128">Его можно просмотреть в окне **Архивные заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="54c81-128">You can view it in the **Archived Sales orders** window.</span></span> <span data-ttu-id="54c81-129">Отсюда его также можно использовать для восстановления заказа на продажу, из которого был создан архив.</span><span class="sxs-lookup"><span data-stu-id="54c81-129">From here, you can also use it to recreate the sales order that it was archived from.</span></span>

## <a name="to-recreate-a-sales-order-from-the-archive"></a><span data-ttu-id="54c81-130">Восстановление заказа на продажу из архива</span><span class="sxs-lookup"><span data-stu-id="54c81-130">To recreate a sales order from the archive</span></span>
<span data-ttu-id="54c81-131">Следующая процедура описывает, как восстановить заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="54c81-131">The following procedure describes how to recreate a sales order.</span></span> <span data-ttu-id="54c81-132">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="54c81-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="54c81-133">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Архивированные заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c81-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2.  <span data-ttu-id="54c81-134">Выберите архивированный заказ на продажу, который требуется восстановить, затем выберите действие **Восстановить**.</span><span class="sxs-lookup"><span data-stu-id="54c81-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="54c81-135">Заказ на продажу создается и добавляется в окно **Заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="54c81-135">The sales order is created and added to the **Sales Orders** window.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="54c81-136">Удаление архивных заказов продажу</span><span class="sxs-lookup"><span data-stu-id="54c81-136">To delete archived sales orders</span></span>
<span data-ttu-id="54c81-137">Следующая процедура описывает, как удалить архивные заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="54c81-137">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="54c81-138">Шаги аналогичны для всех остальных архивных документов продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="54c81-138">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="54c81-139">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить архивные версии заказов продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="54c81-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="54c81-140">В окне **Удалить архивные версии заказов продажи** выберите соответствующие фильтры.</span><span class="sxs-lookup"><span data-stu-id="54c81-140">In the **Delete Archived Sales Order Versions** window, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="54c81-141">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="54c81-141">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="54c81-142">См. также</span><span class="sxs-lookup"><span data-stu-id="54c81-142">See Also</span></span>
[<span data-ttu-id="54c81-143">Отслеживание строк документа</span><span class="sxs-lookup"><span data-stu-id="54c81-143">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="54c81-144">Продажи</span><span class="sxs-lookup"><span data-stu-id="54c81-144">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="54c81-145">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="54c81-145">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="54c81-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="54c81-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

