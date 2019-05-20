---
title: Удаление рабочих процессов | Документы Майкрософт
description: Если вы уверены, что рабочий процесс уже не используется, то его можно удалить. Все экземпляры шагов рабочего процесса, определенные в рабочем процессе, должны иметь статус **Завершено**.
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
ms.openlocfilehash: 31a92e70e044a82313b5329ed2bf007b2b809c11
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244939"
---
# <a name="delete-workflows"></a><span data-ttu-id="18b4b-104">Удаление рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="18b4b-104">Delete Workflows</span></span>
<span data-ttu-id="18b4b-105">Если вы уверены, что рабочий процесс уже не используется, то его можно удалить.</span><span class="sxs-lookup"><span data-stu-id="18b4b-105">If you are certain that a workflow is no longer being used, you can delete it.</span></span> <span data-ttu-id="18b4b-106">Все экземпляры шагов рабочего процесса, определенные в рабочем процессе, должны иметь статус **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="18b4b-106">All workflow step instances that are defined in the workflow must have status **Completed**.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="18b4b-107">При удалении рабочего процесса все сведения в рабочем процессе будут утеряны.</span><span class="sxs-lookup"><span data-stu-id="18b4b-107">When you delete a workflow, all information in the workflow will be lost.</span></span>  

 <span data-ttu-id="18b4b-108">На странице **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="18b4b-108">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="18b4b-109">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="18b4b-109">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="18b4b-110">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="18b4b-110">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="18b4b-111">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="18b4b-111">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-delete-a-workflow"></a><span data-ttu-id="18b4b-112">Удаление рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="18b4b-112">To delete a workflow</span></span>  
1.  <span data-ttu-id="18b4b-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="18b4b-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="18b4b-114">Выберите рабочий процесс, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="18b4b-114">Select the workflow that you want to delete.</span></span>  
3.  <span data-ttu-id="18b4b-115">Выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="18b4b-115">Choose the **Delete** action.</span></span>  
4.  <span data-ttu-id="18b4b-116">Также можно открыть рабочий процесс, который требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="18b4b-116">Alternatively, open the workflow that you want to delete.</span></span>  
5.  <span data-ttu-id="18b4b-117">На странице **Рабочий процесс** выберите действие **Удалить**.</span><span class="sxs-lookup"><span data-stu-id="18b4b-117">On the **Workflow** page, choose the **Delete** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="18b4b-118">См. также</span><span class="sxs-lookup"><span data-stu-id="18b4b-118">See Also</span></span>  
 <span data-ttu-id="18b4b-119">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-119">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="18b4b-120">[Включение рабочих процессов](across-how-to-enable-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-120">[Enable Workflows](across-how-to-enable-workflows.md) </span></span>  
 <span data-ttu-id="18b4b-121">[Просмотр архивированных экземпляров шагов рабочих процессов](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-121">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="18b4b-122">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-122">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="18b4b-123">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-123">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="18b4b-124">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="18b4b-124">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="18b4b-125">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="18b4b-125">Workflow</span></span>](across-workflow.md)   
