---
title: Как учесть несколько документов одновременно | Документация Майкрософт
description: Вместо того чтобы учитывать отдельные документы по одному, вы можете выбрать несколько неучтенных документов в списке для пакетного учета, — либо немедленного, либо запланированного (например, в конце дня).
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 08/18/2020
ms.author: edupont
ms.openlocfilehash: 2c04dac37b043995a9b78e2f662f9411c3cf9ae1
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3782522"
---
# <a name="post-multiple-documents-at-the-same-time"></a><span data-ttu-id="f7f9a-103">Одновременный учет нескольких документов</span><span class="sxs-lookup"><span data-stu-id="f7f9a-103">Post Multiple Documents at the Same Time</span></span>

<span data-ttu-id="f7f9a-104">Вместо того чтобы учитывать отдельные документы по одному, вы можете выбрать несколько неучтенных документов в списке для немедленного учета или для пакетного учета по расписанию (например, в конце дня).</span><span class="sxs-lookup"><span data-stu-id="f7f9a-104">Instead of posting individual documents one by one, you can select multiple non-posted documents in a list for immediate posting or for batch posting according to a schedule, such as at the end of the day.</span></span> <span data-ttu-id="f7f9a-105">Это имеет смысл делать, если только контролер может учитывать документы, созданные другими пользователями, или во избежание проблем с быстродействием системы из-за учета документов в рабочие часы.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-105">This may be useful if only a supervisor can post documents created by other users or to avoid system performance issues from posting during work hours.</span></span>

## <a name="to-post-multiple-purchase-orders-immediately"></a><span data-ttu-id="f7f9a-106">Немедленный одновременный учет нескольких заказов на покупку</span><span class="sxs-lookup"><span data-stu-id="f7f9a-106">To post multiple purchase orders immediately</span></span>

<span data-ttu-id="f7f9a-107">В следующей процедуре рассматривается, как немедленно учесть несколько заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-107">The following procedure explains how to post multiple purchase orders immediately.</span></span> <span data-ttu-id="f7f9a-108">Действия для всех остальных документов продажи и покупки аналогичны.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-108">The steps are similar for all purchase and sales documents.</span></span>

1. <span data-ttu-id="f7f9a-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="f7f9a-110">На странице **Заказы** выберите все заказы для учета:</span><span class="sxs-lookup"><span data-stu-id="f7f9a-110">On the **Purchase Orders** page, proceed to select all orders to be posted:</span></span>
3. <span data-ttu-id="f7f9a-111">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="f7f9a-111">In the **No.**</span></span> <span data-ttu-id="f7f9a-112">выберите три вертикальные точки, чтобы открыть контекстное меню, а затем выберите действие **Выбрать больше**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-112">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span></span>
4. <span data-ttu-id="f7f9a-113">Установите флажки для всех строк, представляющих заказы, которые вы хотите одновременно учесть.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-113">Select the check box for all the lines representing orders that you want to post at the same time.</span></span>
5. <span data-ttu-id="f7f9a-114">Выберите действие **Учет**, а затем выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-114">Choose the **Posting** action, and then choose the **Post** action.</span></span>
6. <span data-ttu-id="f7f9a-115">Нажмите кнопку **Да** в сообщении подтверждения.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-115">Choose the **Yes** button on the confirmation message.</span></span>

## <a name="to-batch-post-multiple-purchase-orders"></a><span data-ttu-id="f7f9a-116">Пакетный учет нескольких заказов на покупку</span><span class="sxs-lookup"><span data-stu-id="f7f9a-116">To batch post multiple purchase orders</span></span>

<span data-ttu-id="f7f9a-117">В следующей процедуре рассматривается пакетный учет заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-117">The following procedure explains how to batch post purchase orders.</span></span> <span data-ttu-id="f7f9a-118">Действия для всех остальных документов покупки и продажи, где доступно действие **Пакетный учет**, аналогичны.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-118">The steps are similar for all purchase and sales documents where the **Batch Post** action is available.</span></span>

> [!NOTE]
> <span data-ttu-id="f7f9a-119">Пакетный учет документов происходит в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-119">Batch posting of documents happens in the background.</span></span> <span data-ttu-id="f7f9a-120">[!INCLUDE [prodshort](includes/prodshort.md)] Online включает задания по умолчанию для фонового учета и пакетного учета.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-120">[!INCLUDE [prodshort](includes/prodshort.md)] online includes default jobs for background posting and batch posting.</span></span> <span data-ttu-id="f7f9a-121">Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="f7f9a-121">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

1. <span data-ttu-id="f7f9a-122">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f7f9a-123">На странице **Заказы** выберите все заказы для учета:</span><span class="sxs-lookup"><span data-stu-id="f7f9a-123">On the **Purchase Orders** page, proceed to select all orders to be posted:</span></span>
3. <span data-ttu-id="f7f9a-124">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="f7f9a-124">In the **No.**</span></span> <span data-ttu-id="f7f9a-125">выберите три вертикальные точки, чтобы открыть контекстное меню, а затем выберите действие **Выбрать больше**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-125">field, choose the three vertical dots to open the context menu, and then choose the **Select More** action.</span></span>
4. <span data-ttu-id="f7f9a-126">Установите флажки для всех строк, представляющих заказы, которые вы хотите одновременно учесть.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-126">Select the check box for all the lines representing orders that you want to post at the same time.</span></span>
5. <span data-ttu-id="f7f9a-127">Выберите действие **Учет**, а затем выберите действие **Пакетный учет**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-127">Choose the **Posting** action, and then choose the **Post Batch** action.</span></span>
6. <span data-ttu-id="f7f9a-128">На странице **Пакет. учет заказов на покупку** заполните поля требуемым образом.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-128">On the **Batch Post Purchase Order** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. <span data-ttu-id="f7f9a-129">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-129">Choose the **OK** button.</span></span>
8. <span data-ttu-id="f7f9a-130">Для просмотра потенциальных проблем, возникших во время пакетного учета документов, откройте страницу **Регистр сообщений об ошибках**.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-130">To view potential issues that occurred during batch posting of documents, open the **Error Message Register** page.</span></span>

<span data-ttu-id="f7f9a-131">Заказы на покупку теперь будут добавлены в отдельную операцию очереди работ, которая определяет, когда будут учтены документы.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-131">The purchase orders will now be added to a dedicated job queue entry, which defines when the documents are posted.</span></span> <span data-ttu-id="f7f9a-132">Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="f7f9a-132">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

<span data-ttu-id="f7f9a-133">Если вы выберете **PDF** в поле **Тип вывода отчета**, успешно учтенные заказы на покупку будут доступны в части **Входящие отчеты** вашего ролевого центра.</span><span class="sxs-lookup"><span data-stu-id="f7f9a-133">If you select **PDF** in the **Report Output Type** field, successfully posted purchase orders will be available in the **Report Inbox** part on your Role Center.</span></span>

## <a name="see-also"></a><span data-ttu-id="f7f9a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="f7f9a-134">See Also</span></span>

[<span data-ttu-id="f7f9a-135">Учет документов и журналов</span><span class="sxs-lookup"><span data-stu-id="f7f9a-135">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
[<span data-ttu-id="f7f9a-136">Использование очередей работ для планирования задач</span><span class="sxs-lookup"><span data-stu-id="f7f9a-136">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)  
[<span data-ttu-id="f7f9a-137">Изменение учтенных документов</span><span class="sxs-lookup"><span data-stu-id="f7f9a-137">Edit Posted Documents</span></span>](across-edit-posted-document.md)  
[<span data-ttu-id="f7f9a-138">Исправление или отмена неоплаченных счетов покупки</span><span class="sxs-lookup"><span data-stu-id="f7f9a-138">Correct or Cancel Unpaid Purchase Invoices</span></span>](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[<span data-ttu-id="f7f9a-139">Поиск страниц и информации с помощью функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="f7f9a-139">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
<span data-ttu-id="f7f9a-140">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f7f9a-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
