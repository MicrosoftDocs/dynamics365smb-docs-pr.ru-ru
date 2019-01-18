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
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 4827e25d97127faf691b96df9868320bb47dee39
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="archive-documents"></a><span data-ttu-id="5689b-103">Архивирование документов</span><span class="sxs-lookup"><span data-stu-id="5689b-103">Archive Documents</span></span>
<span data-ttu-id="5689b-104">Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован.</span><span class="sxs-lookup"><span data-stu-id="5689b-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to recreate the document that it was archived from.</span></span>

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="5689b-105">Настройка автоматического архивирования документов</span><span class="sxs-lookup"><span data-stu-id="5689b-105">To set up automatic document archiving</span></span>  
<span data-ttu-id="5689b-106">Можно настроить автоматическое архивирование заказов продаж и покупки, предложений, общих заказов и заказов на возврат перед удалением документов.</span><span class="sxs-lookup"><span data-stu-id="5689b-106">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="5689b-107">Следующая процедура описывает, как настроить автоматическое архивирование документов продажи.</span><span class="sxs-lookup"><span data-stu-id="5689b-107">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="5689b-108">Действия для документов на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="5689b-108">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="5689b-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи"**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5689b-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="5689b-110">На странице **Настройка модуля "Продажи"** заполните поля, как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="5689b-110">On the **Sales & Receivables Setup** page, fill in the fields as follows.</span></span>

|<span data-ttu-id="5689b-111">Поле</span><span class="sxs-lookup"><span data-stu-id="5689b-111">Field</span></span>|<span data-ttu-id="5689b-112">Описанием</span><span class="sxs-lookup"><span data-stu-id="5689b-112">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="5689b-113">**Архивирование предложений по продаже**</span><span class="sxs-lookup"><span data-stu-id="5689b-113">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="5689b-114">**Никогда**, чтобы никогда не архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="5689b-114">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="5689b-115">**Вопрос**, чтобы предлагать пользователю выбрать, требуется ли архивировать предложения по продаже перед их удалением.</span><span class="sxs-lookup"><span data-stu-id="5689b-115">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="5689b-116">**Всегда**, чтобы автоматически архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="5689b-116">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="5689b-117">**Архивирование общих заказов на продажу**</span><span class="sxs-lookup"><span data-stu-id="5689b-117">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="5689b-118">Выберите для автоматического архивирования общих заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="5689b-118">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="5689b-119">**Архивировать заказы и заказы на возврат**</span><span class="sxs-lookup"><span data-stu-id="5689b-119">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="5689b-120">Выберите для автоматического архивирования заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="5689b-120">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="5689b-121">Архивирование заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="5689b-121">To archive a sales order</span></span>
<span data-ttu-id="5689b-122">Следующая процедура описывает, как архивировать заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="5689b-122">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="5689b-123">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="5689b-123">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="5689b-124">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5689b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5689b-125">Откройте заказ на продажу, который требуется архивировать.</span><span class="sxs-lookup"><span data-stu-id="5689b-125">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="5689b-126">Выберите действие **Архивировать документ**.</span><span class="sxs-lookup"><span data-stu-id="5689b-126">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="5689b-127">Заказ на продажу архивирован.</span><span class="sxs-lookup"><span data-stu-id="5689b-127">The sales order is archived.</span></span> <span data-ttu-id="5689b-128">Его можно просмотреть на странице **Архивные заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="5689b-128">You can view it on the **Archived Sales orders** page.</span></span> <span data-ttu-id="5689b-129">Отсюда его также можно использовать для восстановления заказа на продажу, из которого был создан архив.</span><span class="sxs-lookup"><span data-stu-id="5689b-129">From here, you can also use it to recreate the sales order that it was archived from.</span></span>

## <a name="to-recreate-a-sales-order-from-the-archive"></a><span data-ttu-id="5689b-130">Восстановление заказа на продажу из архива</span><span class="sxs-lookup"><span data-stu-id="5689b-130">To recreate a sales order from the archive</span></span>
<span data-ttu-id="5689b-131">Следующая процедура описывает, как восстановить заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="5689b-131">The following procedure describes how to recreate a sales order.</span></span> <span data-ttu-id="5689b-132">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="5689b-132">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="5689b-133">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Архивированные заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5689b-133">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2.  <span data-ttu-id="5689b-134">Выберите архивированный заказ на продажу, который требуется восстановить, затем выберите действие **Восстановить**.</span><span class="sxs-lookup"><span data-stu-id="5689b-134">Select the archived sales order that you want to recreate, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="5689b-135">Заказ на продажу создается и добавляется на страницу **Заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="5689b-135">The sales order is created and added to the **Sales Orders** page.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="5689b-136">Удаление архивных заказов продажу</span><span class="sxs-lookup"><span data-stu-id="5689b-136">To delete archived sales orders</span></span>
<span data-ttu-id="5689b-137">Следующая процедура описывает, как удалить архивные заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="5689b-137">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="5689b-138">Шаги аналогичны для всех остальных архивных документов продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="5689b-138">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="5689b-139">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить архивные версии заказов продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="5689b-139">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="5689b-140">На странице **Удалить архивные версии заказов продажи** выберите соответствующие фильтры.</span><span class="sxs-lookup"><span data-stu-id="5689b-140">On the **Delete Archived Sales Order Versions** page, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="5689b-141">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="5689b-141">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="5689b-142">См. также</span><span class="sxs-lookup"><span data-stu-id="5689b-142">See Also</span></span>
[<span data-ttu-id="5689b-143">Отслеживание строк документа</span><span class="sxs-lookup"><span data-stu-id="5689b-143">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="5689b-144">Продажи</span><span class="sxs-lookup"><span data-stu-id="5689b-144">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="5689b-145">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="5689b-145">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="5689b-146">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5689b-146">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

