---
title: "Рабочий процесс | Документы Майкрософт"
description: "Можно настроить и использовать рабочие процессы, связывающие задачи бизнес-процесса, выполняемые различными пользователями. Системные задачи, такие как автоматический учет, могут включаться в качестве шагов рабочего процесса, предшествующих задачам пользователя или выполняемых после них. Типичные шаги рабочего процесса – запрос и выдача разрешения на создание новых записей."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 02/20/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e6e662ee13db1f9002e1c3e74a0d15e2aa2e2a98
ms.openlocfilehash: 861ff6ac3c2789f83379e4c01c0e1b8f5847d2d6
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="workflow"></a><span data-ttu-id="74935-105">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="74935-105">Workflow</span></span>
<span data-ttu-id="74935-106">Можно настроить и использовать рабочие процессы, связывающие задачи бизнес-процесса, выполняемые различными пользователями.</span><span class="sxs-lookup"><span data-stu-id="74935-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="74935-107">Системные задачи, такие как автоматический учет, могут включаться в качестве шагов рабочего процесса, предшествующих задачам пользователя или выполняемых после них.</span><span class="sxs-lookup"><span data-stu-id="74935-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="74935-108">Типичные шаги рабочего процесса – запрос и выдача разрешения на создание новых записей.</span><span class="sxs-lookup"><span data-stu-id="74935-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="74935-109">В окне **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="74935-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="74935-110">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="74935-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="74935-111">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="74935-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="74935-112">Универсальная версия [!INCLUDE[d365fin](includes/d365fin_md.md)] содержит ряд заранее настроенных рабочих процессов, представленных в шаблонах рабочих процессов, которые можно копировать при создании рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="74935-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="74935-113">Код для шаблонов рабочих процессов, добавленных Майкрософт, имеет приставку "MS-".</span><span class="sxs-lookup"><span data-stu-id="74935-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="74935-114">Дополнительные сведения см. в шаблонах рабочих процессов в окне Шаблоны рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="74935-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="74935-115">Если бизнес-сценарий требует события или отклика рабочего процесса, которые не поддерживаются, партнеру Майкрософт придется реализовать их, настроив код приложения.</span><span class="sxs-lookup"><span data-stu-id="74935-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="74935-116">Дополнительные сведения см. в разделе [Пошаговое руководство. Реализация новых и событий и отзывов рабочего процесса](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) для ИТ-специалистов и разработчиков.</span><span class="sxs-lookup"><span data-stu-id="74935-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>  

 <span data-ttu-id="74935-117">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="74935-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="74935-118">**Чтобы**</span><span class="sxs-lookup"><span data-stu-id="74935-118">**To**</span></span>|<span data-ttu-id="74935-119">**Смотрите**</span><span class="sxs-lookup"><span data-stu-id="74935-119">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="74935-120">Настройте пользователей рабочего процесса, определите, как пользователи будут получать уведомления, и создайте новые рабочие процессы.</span><span class="sxs-lookup"><span data-stu-id="74935-120">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="74935-121">Для новых рабочих процессов для неподдерживаемых сценариев реализуйте необходимые элементы рабочего процесса путем настройки кода приложения.</span><span class="sxs-lookup"><span data-stu-id="74935-121">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="74935-122">Настройка рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="74935-122">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="74935-123">Включите процессы, выполните действия над уведомлениями рабочего процесса, включая запрос утверждения, и утвердите запросы на выполнение шага рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="74935-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="74935-124">Архивируйте и удалите рабочие процессы.</span><span class="sxs-lookup"><span data-stu-id="74935-124">Archive and delete workflows.</span></span>|[<span data-ttu-id="74935-125">Использование рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="74935-125">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="74935-126">См. также</span><span class="sxs-lookup"><span data-stu-id="74935-126">See Also</span></span>  
[<span data-ttu-id="74935-127">Продажи</span><span class="sxs-lookup"><span data-stu-id="74935-127">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="74935-128">Покупки</span><span class="sxs-lookup"><span data-stu-id="74935-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="74935-129">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="74935-129">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="74935-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="74935-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

