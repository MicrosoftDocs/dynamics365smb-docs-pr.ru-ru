---
title: "Рабочий процесс | Документы Майкрософт"
description: "Можно настроить и использовать рабочие процессы, связывающие задачи бизнес-процесса, выполняемые различными пользователями. Системные задачи, такие как автоматический учет, могут включаться в качестве шагов рабочего процесса, предшествующих задачам пользователя или выполняемых после них. Типичные шаги рабочего процесса – запрос и выдача разрешения на создание новых записей."
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
ms.openlocfilehash: 7a7782fcb51eb9078cb62c4892814cd178518332
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="workflow"></a><span data-ttu-id="13c9b-105">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="13c9b-105">Workflow</span></span>
<span data-ttu-id="13c9b-106">Можно настроить и использовать рабочие процессы, связывающие задачи бизнес-процесса, выполняемые различными пользователями.</span><span class="sxs-lookup"><span data-stu-id="13c9b-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="13c9b-107">Системные задачи, такие как автоматический учет, могут включаться в качестве шагов рабочего процесса, предшествующих задачам пользователя или выполняемых после них.</span><span class="sxs-lookup"><span data-stu-id="13c9b-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="13c9b-108">Типичные шаги рабочего процесса – запрос и выдача разрешения на создание новых записей.</span><span class="sxs-lookup"><span data-stu-id="13c9b-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="13c9b-109">В окне **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="13c9b-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="13c9b-110">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="13c9b-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="13c9b-111">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="13c9b-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="13c9b-112">Универсальная версия [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит ряд заранее настроенных рабочих процессов, представленных в шаблонах рабочих процессов, которые можно копировать при создании рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="13c9b-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="13c9b-113">Код для шаблонов рабочих процессов, добавленных Майкрософт, имеет приставку "MS-".</span><span class="sxs-lookup"><span data-stu-id="13c9b-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="13c9b-114">Дополнительные сведения см. в шаблонах рабочих процессов в окне Шаблоны рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="13c9b-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="13c9b-115">Если бизнес-сценарий требует события или отклика рабочего процесса, которые не поддерживаются, партнеру Майкрософт придется реализовать их, настроив код приложения.</span><span class="sxs-lookup"><span data-stu-id="13c9b-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="13c9b-116">Дополнительные сведения см. в разделе [Пошаговое руководство. Реализация новых и событий и отзывов рабочего процесса](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) для ИТ-специалистов и разработчиков.</span><span class="sxs-lookup"><span data-stu-id="13c9b-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>

> [!NOTE]  
> <span data-ttu-id="13c9b-117">Бизнес-процессы также могут инициироваться из Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="13c9b-117">Workflows can also be initiated from Microsoft Flow.</span></span> <span data-ttu-id="13c9b-118">Дополнительные сведения см. в разделе [Использование Business Central в автоматическом бизнес-процессе](across-how-use-financials-data-source-flow.md).</span><span class="sxs-lookup"><span data-stu-id="13c9b-118">For more information, see [Using Business Central in an Automated Workflow](across-how-use-financials-data-source-flow.md).</span></span>  

 <span data-ttu-id="13c9b-119">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="13c9b-119">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="13c9b-120">**Чтобы**</span><span class="sxs-lookup"><span data-stu-id="13c9b-120">**To**</span></span>|<span data-ttu-id="13c9b-121">**Смотрите**</span><span class="sxs-lookup"><span data-stu-id="13c9b-121">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="13c9b-122">Настройте пользователей рабочего процесса, определите, как пользователи будут получать уведомления, и создайте новые рабочие процессы.</span><span class="sxs-lookup"><span data-stu-id="13c9b-122">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="13c9b-123">Для новых рабочих процессов для неподдерживаемых сценариев реализуйте необходимые элементы рабочего процесса путем настройки кода приложения.</span><span class="sxs-lookup"><span data-stu-id="13c9b-123">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="13c9b-124">Настройка рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="13c9b-124">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="13c9b-125">Включите процессы, выполните действия над уведомлениями рабочего процесса, включая запрос утверждения, и утвердите запросы на выполнение шага рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="13c9b-125">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="13c9b-126">Архивируйте и удалите рабочие процессы.</span><span class="sxs-lookup"><span data-stu-id="13c9b-126">Archive and delete workflows.</span></span>|[<span data-ttu-id="13c9b-127">Использование рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="13c9b-127">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="13c9b-128">См. также</span><span class="sxs-lookup"><span data-stu-id="13c9b-128">See Also</span></span>  
[<span data-ttu-id="13c9b-129">Продажи</span><span class="sxs-lookup"><span data-stu-id="13c9b-129">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="13c9b-130">Покупки</span><span class="sxs-lookup"><span data-stu-id="13c9b-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="13c9b-131">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="13c9b-131">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="13c9b-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="13c9b-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

