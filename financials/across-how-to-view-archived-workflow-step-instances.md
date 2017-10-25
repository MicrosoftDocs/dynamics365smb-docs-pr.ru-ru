---
title: "Просмотр архивированных экземпляров шагов рабочих процессов | Документы Майкрософт"
description: "Все завершенные экземпляры шагов рабочего процесса сохраняются в окне **Архивные экземпляры шагов рабочих процессов**."
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 31954eca30012b8b5d494dd0a06d6ffefa9cbd6c
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-view-archived-workflow-step-instances"></a><span data-ttu-id="054f7-103">Практическое руководство. Просмотр архивированных экземпляров шагов рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="054f7-103">How to: View Archived Workflow Step Instances</span></span>
<span data-ttu-id="054f7-104">Все завершенные экземпляры шагов рабочего процесса сохраняются в окне **Архивные экземпляры шагов рабочих процессов**.</span><span class="sxs-lookup"><span data-stu-id="054f7-104">All completed workflow step instances are saved in the **Archived Workflow Step Instances** window.</span></span>  

 <span data-ttu-id="054f7-105">В окне **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="054f7-105">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="054f7-106">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="054f7-106">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="054f7-107">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="054f7-107">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="054f7-108">Дополнительные сведения см. в разделе [Практическое руководство. Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="054f7-108">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-view-archived-workflow-step-instances"></a><span data-ttu-id="054f7-109">Просмотр архивированных экземпляров шагов потоков операций</span><span class="sxs-lookup"><span data-stu-id="054f7-109">To view archived workflow step instances</span></span>  
1.  <span data-ttu-id="054f7-110">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="054f7-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="054f7-111">Откройте поток операций, для которого нужно просмотреть все помещенные в архив экземпляры шагов потоков операций.</span><span class="sxs-lookup"><span data-stu-id="054f7-111">Open the workflow for which you want to view all archived workflow step instances.</span></span>  
3.  <span data-ttu-id="054f7-112">В окне **Рабочий процесс** выберите действие **Архивные экземпляры шагов рабочих процессов**.</span><span class="sxs-lookup"><span data-stu-id="054f7-112">In the **Workflow** window, choose the **Archived Workflow Step Instances** action.</span></span>  

    <span data-ttu-id="054f7-113">Откроется окно **Архивные экземпляры шагов рабочих процессов**, содержащее архивные экземпляры шагов выбранного рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="054f7-113">The **Archived Workflow Step Instances** window opens showing the archived workflow step instances of the selected workflow.</span></span>  
4.  <span data-ttu-id="054f7-114">Можно также выбрать значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), ввести **Архивные экземпляры шагов рабочих процессов**, затем выбрать связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="054f7-114">Alternatively, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Archived Workflow Step Instances**, and then choose the related link.</span></span>  

<span data-ttu-id="054f7-115">Откроется окно **Архивные экземпляры шагов рабочих процессов**, содержащее все архивные экземпляры шагов рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="054f7-115">The **Archived Workflow Step Instances** window opens showing all archived workflow step instances.</span></span> <span data-ttu-id="054f7-116">В поле **Код рабочего процесса** можно посмотреть, к какому потоку операций относится архивированный шаг рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="054f7-116">In the **Workflow Code** field, you can see which workflow the archived workflow step instance belonged to.</span></span>  

## <a name="see-also"></a><span data-ttu-id="054f7-117">См. также</span><span class="sxs-lookup"><span data-stu-id="054f7-117">See Also</span></span>  
 <span data-ttu-id="054f7-118">[Практическое руководство. Удаление рабочих процессов](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-118">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="054f7-119">[Практическое руководство. Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-119">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="054f7-120">[Практическое руководство. Включение рабочих процессов](across-how-to-enable-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-120">[How to: Enable Workflows](across-how-to-enable-workflows.md) </span></span>  
 <span data-ttu-id="054f7-121">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-121">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="054f7-122">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-122">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="054f7-123">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="054f7-123">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="054f7-124">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="054f7-124">Workflow</span></span>](across-workflow.md)

