---
title: Практическое руководство. Ограничение и разрешение использования записи | Microsoft Docs
description: Если нужно ограничить использование записи в определенных видах деятельности, например, до утверждения записи, можно встроить в рабочий процесс два отклика, управляющих использованием записи.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2a2ff204f2d4b44c84bf1eecfce374b6174432fa
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "927131"
---
# <a name="restrict-and-allow-usage-of-a-record"></a><span data-ttu-id="75116-103">Ограничение и разрешение использования записи</span><span class="sxs-lookup"><span data-stu-id="75116-103">Restrict and Allow Usage of a Record</span></span>
<span data-ttu-id="75116-104">Если нужно ограничить использование записи в определенных видах деятельности, например, до утверждения записи, можно встроить в рабочий процесс два отклика, управляющих использованием записи.</span><span class="sxs-lookup"><span data-stu-id="75116-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span></span> <span data-ttu-id="75116-105">Один отклик процесса будет ограничивать использование записи, определенное событием и условиями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="75116-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="75116-106">Другой отклик рабочего процесса будет разрешать использование записи, определенное событием и условиями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="75116-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="75116-107">Для этой цели в универсальной версии [!INCLUDE[d365fin](includes/d365fin_md.md)] доступно два отклика: **Ограничить использование записи**</span><span class="sxs-lookup"><span data-stu-id="75116-107">Two responses exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span></span> <span data-ttu-id="75116-108">и **Разрешить использование записи**.</span><span class="sxs-lookup"><span data-stu-id="75116-108">and **Allow usage of a record.**.</span></span>

> [!NOTE]  
>  <span data-ttu-id="75116-109">Универсальная версия [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагает поддержку для ограничения учета записи, экспорта в качестве платежа, а также печати в чеке.</span><span class="sxs-lookup"><span data-stu-id="75116-109">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span></span> <span data-ttu-id="75116-110">Для поддержки других ограничений партнер Майкрософт должен настроить код приложения.</span><span class="sxs-lookup"><span data-stu-id="75116-110">To support other restrictions, a Microsoft partner must customize the application code.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="75116-111">Возможности рабочих процессов для ограничения и разрешения использования записей не связаны с функциональностью блокировки учета записей товара, клиента и поставщика.</span><span class="sxs-lookup"><span data-stu-id="75116-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span></span>

<span data-ttu-id="75116-112">Далее описывается процедура ограничения учета заказов на покупку до их утверждения.</span><span class="sxs-lookup"><span data-stu-id="75116-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span></span> <span data-ttu-id="75116-113">Новый рабочий процесс будет основан на существующем шаблоне рабочего процесса "Рабочий процесс утверждения счета покупки".</span><span class="sxs-lookup"><span data-stu-id="75116-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span></span>  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a><span data-ttu-id="75116-114">Создание шага рабочего процесса, ограничивающего учет неутвержденных заказов на покупку</span><span class="sxs-lookup"><span data-stu-id="75116-114">To create a workflow step that restricts posting of unapproved purchase orders</span></span>  
1. <span data-ttu-id="75116-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="75116-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="75116-116">На странице **Рабочие процессы** создайте новый рабочий процесс с именем "Рабочий процесс утверждения заказов на покупку".</span><span class="sxs-lookup"><span data-stu-id="75116-116">On the **Workflows** page, create a new workflow named Purchase Order Approval Workflow.</span></span> <span data-ttu-id="75116-117">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="75116-117">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  
3. <span data-ttu-id="75116-118">Выберите действие **Копировать из шаблона рабочего процесса**.</span><span class="sxs-lookup"><span data-stu-id="75116-118">Choose the **Copy From Workflow Template** action.</span></span>  
4. <span data-ttu-id="75116-119">Выберите поле **Исходный код рабочего процесса**, а затем на странице **Шаблоны рабочих процессов** выберите шаблон "Рабочий процесс утверждения счета покупки".</span><span class="sxs-lookup"><span data-stu-id="75116-119">Choose the **Source Workflow Code** field, and then, on the **Workflow Templates** page, choose the Purchase Invoice Approval Workflow workflow template.</span></span>  

     <span data-ttu-id="75116-120">Обратите внимание, что первые 2 шага рабочего процесса связаны с ограничением и последующим разрешением использования счетов покупки.</span><span class="sxs-lookup"><span data-stu-id="75116-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span></span> <span data-ttu-id="75116-121">Теперь измените условие события в первом шаге нового рабочего процесса, чтобы указать, что он применяется к заказам на покупку.</span><span class="sxs-lookup"><span data-stu-id="75116-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span></span>  
5. <span data-ttu-id="75116-122">На экспресс-вкладке **Шаги рабочего процесса** выберите поле **Условия события**, а затем для фильтра **Тип документа** выберите **Заказ**.</span><span class="sxs-lookup"><span data-stu-id="75116-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span></span>  
6. <span data-ttu-id="75116-123">Измените, удалите или добавьте другие шаги рабочего процесса в соответствии с бизнес-процессом, который начинается с ограничения учета неутвержденных заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="75116-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="75116-124">См. также</span><span class="sxs-lookup"><span data-stu-id="75116-124">See Also</span></span>  
<span data-ttu-id="75116-125">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="75116-125">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
[<span data-ttu-id="75116-126">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="75116-126">Workflow</span></span>](across-workflow.md)   
