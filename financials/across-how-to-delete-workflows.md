---
title: "Удаление рабочих процессов | Документы Майкрософт"
description: "Если вы уверены, что рабочий процесс уже не используется, то его можно удалить. Все экземпляры шагов рабочего процесса, определенные в рабочем процессе, должны иметь статус **Завершено**."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 3e972ae6532c9531845e2739237b6ccb94d14c12
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="delete-workflows"></a><span data-ttu-id="84c8c-104">Удаление рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="84c8c-104">Delete Workflows</span></span>
<span data-ttu-id="84c8c-105">Если вы уверены, что рабочий процесс уже не используется, то его можно удалить.</span><span class="sxs-lookup"><span data-stu-id="84c8c-105">If you are certain that a workflow is no longer being used, you can delete it.</span></span> <span data-ttu-id="84c8c-106">Все экземпляры шагов рабочего процесса, определенные в рабочем процессе, должны иметь статус **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="84c8c-106">All workflow step instances that are defined in the workflow must have status **Completed**.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="84c8c-107">При удалении рабочего процесса все сведения в рабочем процессе будут утеряны.</span><span class="sxs-lookup"><span data-stu-id="84c8c-107">When you delete a workflow, all information in the workflow will be lost.</span></span>  

 <span data-ttu-id="84c8c-108">В окне **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="84c8c-108">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="84c8c-109">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="84c8c-109">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="84c8c-110">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="84c8c-110">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="84c8c-111">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="84c8c-111">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-delete-a-workflow"></a><span data-ttu-id="84c8c-112">Удаление рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="84c8c-112">To delete a workflow</span></span>  
1.  <span data-ttu-id="84c8c-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="84c8c-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="84c8c-114">Выберите рабочий процесс, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="84c8c-114">Select the workflow that you want to delete.</span></span>  
3.  <span data-ttu-id="84c8c-115">Выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="84c8c-115">Choose the **Delete** action.</span></span>  
4.  <span data-ttu-id="84c8c-116">Также можно открыть рабочий процесс, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="84c8c-116">Alternatively, open the workflow that you want to delete.</span></span>  
5.  <span data-ttu-id="84c8c-117">В окне **Рабочий процесс** выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="84c8c-117">In the **Workflow** window, choose the **Delete** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="84c8c-118">См. также</span><span class="sxs-lookup"><span data-stu-id="84c8c-118">See Also</span></span>  
 <span data-ttu-id="84c8c-119">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-119">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="84c8c-120">[Включение рабочих процессов](across-how-to-enable-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-120">[Enable Workflows](across-how-to-enable-workflows.md) </span></span>  
 <span data-ttu-id="84c8c-121">[Просмотр архивированных экземпляров шагов рабочих процессов](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-121">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="84c8c-122">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-122">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="84c8c-123">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-123">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="84c8c-124">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="84c8c-124">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="84c8c-125">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="84c8c-125">Workflow</span></span>](across-workflow.md)   

