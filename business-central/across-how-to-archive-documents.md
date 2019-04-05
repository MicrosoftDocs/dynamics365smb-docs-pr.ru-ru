---
title: Как архивировать документы о продажах и покупке | Документы Майкрософт
description: Можно архивировать заказы продажи и покупки, предложения, заказы на возврат и общие заказы, и можно использовать архивный документ для восстановления документа, из которого он был архивирован.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 02/14/2018
ms.author: sgroespe
ms.openlocfilehash: 2f05313d30aede255e4ef49065f0189d649ce93c
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805080"
---
# <a name="archive-documents"></a><span data-ttu-id="034db-103">Архивирование документов</span><span class="sxs-lookup"><span data-stu-id="034db-103">Archive Documents</span></span>
<span data-ttu-id="034db-104">Можно поместить в архив заказы на продажу и покупку, предложения с расценками, заказы на возврат и общие заказы, например, если хотите сохранить копию документа для повторного пользования позднее.</span><span class="sxs-lookup"><span data-stu-id="034db-104">You can archive sales and purchase orders, quotes, return orders, and blanket orders, for example because you want to save a copy of a document for reuse later.</span></span> <span data-ttu-id="034db-105">Можно поместить в архив документ по продаже или покупке несколько раз, каждый раз сохраняя другую архивную версию.</span><span class="sxs-lookup"><span data-stu-id="034db-105">You can archive a sales or purchase document several times, saving a different archived version each time.</span></span>

<span data-ttu-id="034db-106">Для архивных документов, для которых оригинал все еще существует и не учтен, можно использовать функцию **Восстановить**, чтобы перезаписать оригинал архивной версией документа.</span><span class="sxs-lookup"><span data-stu-id="034db-106">For archived documents where the original still exists and is not posted, you can use the **Restore** function to overwrite the original with the archived version of the document.</span></span> <span data-ttu-id="034db-107">Это целесообразно, если необходимо восстановить содержимое документа на более раннем этапе.</span><span class="sxs-lookup"><span data-stu-id="034db-107">This is practical if you need to restore the contents of a document to an earlier state.</span></span>

<span data-ttu-id="034db-108">Для архивных документов, для которых оригинал удален, содержимое можно использовать только путем копирования данных, например с помощью функции **Копировать документ**.</span><span class="sxs-lookup"><span data-stu-id="034db-108">For archived documents where the original is deleted, you can only reuse the content by copying the data, for example with the **Copy Document** function.</span></span>   

## <a name="to-set-up-automatic-document-archiving"></a><span data-ttu-id="034db-109">Настройка автоматического архивирования документов</span><span class="sxs-lookup"><span data-stu-id="034db-109">To set up automatic document archiving</span></span>  
<span data-ttu-id="034db-110">Можно настроить автоматическое архивирование заказов продаж и покупки, предложений, общих заказов и заказов на возврат перед удалением документов.</span><span class="sxs-lookup"><span data-stu-id="034db-110">You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.</span></span>

<span data-ttu-id="034db-111">Следующая процедура описывает, как настроить автоматическое архивирование документов продажи.</span><span class="sxs-lookup"><span data-stu-id="034db-111">The following procedure describes how to set up automatic archiving of sales documents.</span></span> <span data-ttu-id="034db-112">Действия для документов на покупку аналогичны.</span><span class="sxs-lookup"><span data-stu-id="034db-112">The steps are similar for purchase documents.</span></span>
1.  <span data-ttu-id="034db-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка модуля "Продажи"**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="034db-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="034db-114">На странице **Настройка модуля "Продажи"** заполните поля, как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="034db-114">On the **Sales & Receivables Setup** page, fill in the fields as follows.</span></span>

|<span data-ttu-id="034db-115">Поле</span><span class="sxs-lookup"><span data-stu-id="034db-115">Field</span></span>|<span data-ttu-id="034db-116">Описанием</span><span class="sxs-lookup"><span data-stu-id="034db-116">Description</span></span>|
|-----|-----------|
|<span data-ttu-id="034db-117">**Архивирование предложений по продаже**</span><span class="sxs-lookup"><span data-stu-id="034db-117">**Archiving Sales Quotes**</span></span>|<span data-ttu-id="034db-118">**Никогда**, чтобы никогда не архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="034db-118">**Never** to never archive sales quotes when they are deleted.</span></span> <span data-ttu-id="034db-119">**Вопрос**, чтобы предлагать пользователю выбрать, требуется ли архивировать предложения по продаже перед их удалением.</span><span class="sxs-lookup"><span data-stu-id="034db-119">**Question** to prompt the user to choose whether to archive sales quotes when they are deleted.</span></span> <span data-ttu-id="034db-120">**Всегда**, чтобы автоматически архивировать предложения по продаже при их удалении.</span><span class="sxs-lookup"><span data-stu-id="034db-120">**Always** to archive sales quotes automatically when they are deleted.</span></span>|
|<span data-ttu-id="034db-121">**Архивирование общих заказов на продажу**</span><span class="sxs-lookup"><span data-stu-id="034db-121">**Archiving Blanket Sales Orders**</span></span>|<span data-ttu-id="034db-122">Выберите для автоматического архивирования общих заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="034db-122">Select to archive blanket sales orders automatically each time they are deleted.</span></span>|
|<span data-ttu-id="034db-123">**Архивировать заказы и заказы на возврат**</span><span class="sxs-lookup"><span data-stu-id="034db-123">**Arch. Orders and Ret. Orders**</span></span>|<span data-ttu-id="034db-124">Выберите для автоматического архивирования заказов на продажу каждый раз при их удалении.</span><span class="sxs-lookup"><span data-stu-id="034db-124">Select to automatically archive sales orders each time they are deleted.</span></span>|

## <a name="to-archive-a-sales-order"></a><span data-ttu-id="034db-125">Архивирование заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="034db-125">To archive a sales order</span></span>
<span data-ttu-id="034db-126">Следующая процедура описывает, как архивировать заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="034db-126">The following procedure describes how to archive a sales order.</span></span> <span data-ttu-id="034db-127">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="034db-127">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1.  <span data-ttu-id="034db-128">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="034db-128">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="034db-129">Откройте заказ на продажу, который требуется архивировать.</span><span class="sxs-lookup"><span data-stu-id="034db-129">Open a sales order that you want to archive.</span></span>  
3.  <span data-ttu-id="034db-130">Выберите действие **Архивировать документ**.</span><span class="sxs-lookup"><span data-stu-id="034db-130">Choose the **Archive Document** action.</span></span>

<span data-ttu-id="034db-131">Заказ на продажу архивирован.</span><span class="sxs-lookup"><span data-stu-id="034db-131">The sales order is archived.</span></span> <span data-ttu-id="034db-132">Его можно просмотреть на странице **Архивные заказы на продажу**.</span><span class="sxs-lookup"><span data-stu-id="034db-132">You can view it on the **Archived Sales orders** page.</span></span>

## <a name="to-restore-a-non-posted-sales-order-from-the-archive"></a><span data-ttu-id="034db-133">Восстановление неучтенного заказа на продажу из архива</span><span class="sxs-lookup"><span data-stu-id="034db-133">To restore a non-posted sales order from the archive</span></span>
<span data-ttu-id="034db-134">Далее описывается процедура переноса содержимого архивного заказа на продажу назад в оригинальный заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="034db-134">The following procedure describes how to bring the contents of an archived sales order back to the original sales order.</span></span> <span data-ttu-id="034db-135">Это возможно только в том случае, если исходный документ не был учтен.</span><span class="sxs-lookup"><span data-stu-id="034db-135">This is only possible when the original document has not been posted.</span></span> <span data-ttu-id="034db-136">Эти шаги аналогичны для всех заказов, общих заказов, заказов на возврат и предложений.</span><span class="sxs-lookup"><span data-stu-id="034db-136">The steps are similar for all orders, blanket orders, return orders, and quotes.</span></span>

1. <span data-ttu-id="034db-137">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Архивированные заказы на продажу**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="034db-137">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Sales Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="034db-138">Выберите архивированный заказ на продажу или ту его версию, которую требуется восстановить, затем выберите действие **Восстановить**.</span><span class="sxs-lookup"><span data-stu-id="034db-138">Select the archived sales order, or version of it, that you want to restore, and then choose the **Restore** action.</span></span>  

<span data-ttu-id="034db-139">Содержимое оригинального заказа на продажу заменяется содержимым выбранной архивной версии.</span><span class="sxs-lookup"><span data-stu-id="034db-139">The contents of the original sales order is replaced with that of the selected archived version.</span></span>

## <a name="to-delete-archived-sales-orders"></a><span data-ttu-id="034db-140">Удаление архивных заказов продажу</span><span class="sxs-lookup"><span data-stu-id="034db-140">To delete archived sales orders</span></span>
<span data-ttu-id="034db-141">Следующая процедура описывает, как удалить архивные заказы на продажу.</span><span class="sxs-lookup"><span data-stu-id="034db-141">The following procedure describes how to delete archived sales orders.</span></span> <span data-ttu-id="034db-142">Шаги аналогичны для всех остальных архивных документов продажи и покупки.</span><span class="sxs-lookup"><span data-stu-id="034db-142">The steps are similar for other archived sales and purchase documents.</span></span>

1.  <span data-ttu-id="034db-143">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Удалить архивные версии заказов продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="034db-143">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="034db-144">На странице **Удалить архивные версии заказов продажи** выберите соответствующие фильтры.</span><span class="sxs-lookup"><span data-stu-id="034db-144">On the **Delete Archived Sales Order Versions** page, select the appropriate filters.</span></span>  
3.  <span data-ttu-id="034db-145">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="034db-145">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="034db-146">См. также</span><span class="sxs-lookup"><span data-stu-id="034db-146">See Also</span></span>
[<span data-ttu-id="034db-147">Отслеживание строк документа</span><span class="sxs-lookup"><span data-stu-id="034db-147">Track Document Lines</span></span>](across-how-to-track-document-lines.md)  
[<span data-ttu-id="034db-148">Продажи</span><span class="sxs-lookup"><span data-stu-id="034db-148">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="034db-149">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="034db-149">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="034db-150">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="034db-150">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
