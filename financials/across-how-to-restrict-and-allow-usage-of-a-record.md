---
title: "Практическое руководство. Ограничение и разрешение использования записи | Microsoft Docs"
description: "Если нужно ограничить использование записи в определенных видах деятельности, например, до утверждения записи, можно встроить в рабочий процесс два отклика, управляющих использованием записи."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 0dc8b3eeecfbf3f4a96985f4e4adaf0b3a5a21d0
ms.contentlocale: ru-ru
ms.lasthandoff: 11/10/2017

---
# <a name="how-to-restrict-and-allow-usage-of-a-record"></a><span data-ttu-id="39537-103">Практическое руководство. Ограничение и разрешение использования записи</span><span class="sxs-lookup"><span data-stu-id="39537-103">How to: Restrict and Allow Usage of a Record</span></span>
<span data-ttu-id="39537-104">Если нужно ограничить использование записи в определенных видах деятельности, например, до утверждения записи, можно встроить в рабочий процесс два отклика, управляющих использованием записи.</span><span class="sxs-lookup"><span data-stu-id="39537-104">If you want to restrict a record from being used in certain activities, for example, until the record has been approved, you can incorporate two workflow responses in a workflow that controls the usage of the record.</span></span> <span data-ttu-id="39537-105">Один отклик процесса будет ограничивать использование записи, определенное событием и условиями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="39537-105">One workflow response will restrict usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="39537-106">Другой отклик рабочего процесса будет разрешать использование записи, определенное событием и условиями рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="39537-106">Another workflow response will allow usage of the record as defined by the workflow event and conditions.</span></span> <span data-ttu-id="39537-107">Для этой цели в универсальной версии [!INCLUDE[d365fin](includes/d365fin_md.md)] доступно два отклика: **Ограничить использование записи**</span><span class="sxs-lookup"><span data-stu-id="39537-107">Two responses exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] for this purpose: **Restrict usage of a record.**</span></span> <span data-ttu-id="39537-108">и **Разрешить использование записи**.</span><span class="sxs-lookup"><span data-stu-id="39537-108">and **Allow usage of a record.**.</span></span>

> [!NOTE]  
>  <span data-ttu-id="39537-109">Универсальная версия [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагает поддержку для ограничения учета записи, экспорта в качестве платежа, а также печати в чеке.</span><span class="sxs-lookup"><span data-stu-id="39537-109">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] offers support for restricting a record from being posted, from being exported as a payment, and from being printed as a check.</span></span> <span data-ttu-id="39537-110">Для поддержки других ограничений партнер Майкрософт должен настроить код приложения.</span><span class="sxs-lookup"><span data-stu-id="39537-110">To support other restrictions, a Microsoft partner must customize the application code.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="39537-111">Возможности рабочих процессов для ограничения и разрешения использования записей не связаны с функциональностью блокировки учета записей товара, клиента и поставщика.</span><span class="sxs-lookup"><span data-stu-id="39537-111">The workflow functionality to restrict and allow records from being used is not related to the functionality to block item, customer, and vendor records from being posted.</span></span>

<span data-ttu-id="39537-112">Далее описывается процедура ограничения учета заказов на покупку до их утверждения.</span><span class="sxs-lookup"><span data-stu-id="39537-112">The following procedure describes how to restrict purchase orders from being posted until they have been approved.</span></span> <span data-ttu-id="39537-113">Новый рабочий процесс будет основан на существующем шаблоне рабочего процесса "Рабочий процесс утверждения счета покупки".</span><span class="sxs-lookup"><span data-stu-id="39537-113">The new workflow will be based on the existing Purchase Invoice Approval Workflow workflow template.</span></span>  

## <a name="to-create-a-workflow-step-that-restricts-posting-of-unapproved-purchase-orders"></a><span data-ttu-id="39537-114">Создание шага рабочего процесса, ограничивающего учет неутвержденных заказов на покупку</span><span class="sxs-lookup"><span data-stu-id="39537-114">To create a workflow step that restricts posting of unapproved purchase orders</span></span>  
1. <span data-ttu-id="39537-115">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="39537-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2. <span data-ttu-id="39537-116">В окне **Рабочие процессы** создайте новый рабочий процесс с именем "Рабочий процесс утверждения заказов на покупку".</span><span class="sxs-lookup"><span data-stu-id="39537-116">In the **Workflows** window, create a new workflow named Purchase Order Approval Workflow.</span></span> <span data-ttu-id="39537-117">Дополнительные сведения см. в разделе [Практическое руководство. Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="39537-117">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  
3. <span data-ttu-id="39537-118">Выберите действие **Копировать из шаблона рабочего процесса**.</span><span class="sxs-lookup"><span data-stu-id="39537-118">Choose the **Copy From Workflow Template** action.</span></span>  
4. <span data-ttu-id="39537-119">Выберите поле **Исходный код рабочего процесса**, а затем в окне **Шаблоны рабочих процессов** выберите шаблон "Рабочий процесс утверждения счета покупки".</span><span class="sxs-lookup"><span data-stu-id="39537-119">Choose the **Source Workflow Code** field, and then, in the **Workflow Templates** window, choose the Purchase Invoice Approval Workflow workflow template.</span></span>  

     <span data-ttu-id="39537-120">Обратите внимание, что первые 2 шага рабочего процесса связаны с ограничением и последующим разрешением использования счетов покупки.</span><span class="sxs-lookup"><span data-stu-id="39537-120">Notice that the first two workflow steps are about restricting and then allowing usage of purchase invoices.</span></span> <span data-ttu-id="39537-121">Теперь измените условие события в первом шаге нового рабочего процесса, чтобы указать, что он применяется к заказам на покупку.</span><span class="sxs-lookup"><span data-stu-id="39537-121">Proceed to change the event condition on the first step of the new workflow to specify that it applies to purchase orders.</span></span>  
5. <span data-ttu-id="39537-122">На экспресс-вкладке **Шаги рабочего процесса** выберите поле **Условия события**, а затем для фильтра **Тип документа** выберите **Заказ**.</span><span class="sxs-lookup"><span data-stu-id="39537-122">On the **Workflow Steps** FastTab, choose the **Event Conditions** field, and then, for the **Document Type** filter, select **Order**.</span></span>  
6. <span data-ttu-id="39537-123">Измените, удалите или добавьте другие шаги рабочего процесса в соответствии с бизнес-процессом, который начинается с ограничения учета неутвержденных заказов на покупку.</span><span class="sxs-lookup"><span data-stu-id="39537-123">Proceed to edit, delete, or add other workflow steps to fit a business process that begins by restricting unapproved purchase orders from being posted.</span></span>  

## <a name="see-also"></a><span data-ttu-id="39537-124">См. также</span><span class="sxs-lookup"><span data-stu-id="39537-124">See Also</span></span>  
<span data-ttu-id="39537-125">[Практическое руководство. Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="39537-125">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
[<span data-ttu-id="39537-126">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="39537-126">Workflow</span></span>](across-workflow.md)   
