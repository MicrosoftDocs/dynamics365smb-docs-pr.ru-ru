---
title: Просмотр архивированных экземпляров шагов рабочих процессов | Документация Майкрософт
description: Все завершенные экземпляры шагов рабочего процесса сохраняются на странице **Архивные экземпляры шагов рабочих процессов**.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: a6797d407b2bb307e963b35ca8d8165982864b98
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881052"
---
# <a name="view-archived-workflow-step-instances"></a><span data-ttu-id="c254d-103">Просмотр архивированных экземпляров шагов рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="c254d-103">View Archived Workflow Step Instances</span></span>
<span data-ttu-id="c254d-104">Все завершенные экземпляры шагов рабочего процесса сохраняются на странице **Архивные экземпляры шагов рабочих процессов**.</span><span class="sxs-lookup"><span data-stu-id="c254d-104">All completed workflow step instances are saved on the **Archived Workflow Step Instances** page.</span></span>  

 <span data-ttu-id="c254d-105">На странице **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="c254d-105">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="c254d-106">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="c254d-106">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="c254d-107">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="c254d-107">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="c254d-108">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="c254d-108">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-view-archived-workflow-step-instances"></a><span data-ttu-id="c254d-109">Просмотр архивированных экземпляров шагов потоков операций</span><span class="sxs-lookup"><span data-stu-id="c254d-109">To view archived workflow step instances</span></span>  
1.  <span data-ttu-id="c254d-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c254d-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c254d-111">Откройте поток операций, для которого нужно просмотреть все помещенные в архив экземпляры шагов потоков операций.</span><span class="sxs-lookup"><span data-stu-id="c254d-111">Open the workflow for which you want to view all archived workflow step instances.</span></span>  
3.  <span data-ttu-id="c254d-112">На странице **Рабочий процесс** выберите действие **Архивные экземпляры шагов рабочих процессов**.</span><span class="sxs-lookup"><span data-stu-id="c254d-112">On the **Workflow** page, choose the **Archived Workflow Step Instances** action.</span></span>  

    <span data-ttu-id="c254d-113">Откроется страница **Архивные экземпляры шагов рабочих процессов**, содержащая архивные экземпляры шагов выбранного рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c254d-113">The **Archived Workflow Step Instances** page opens showing the archived workflow step instances of the selected workflow.</span></span>  
4.  <span data-ttu-id="c254d-114">Можно также выбрать значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Архивные экземпляры шагов рабочих процессов**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c254d-114">Alternatively, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Archived Workflow Step Instances**, and then choose the related link.</span></span>  

<span data-ttu-id="c254d-115">Откроется страница **Архивные экземпляры шагов рабочих процессов**, содержащее все архивные экземпляры шагов рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="c254d-115">The **Archived Workflow Step Instances** page opens showing all archived workflow step instances.</span></span> <span data-ttu-id="c254d-116">В поле **Код рабочего процесса** можно посмотреть, к какому потоку операций относится архивированный шаг рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="c254d-116">In the **Workflow Code** field, you can see which workflow the archived workflow step instance belonged to.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c254d-117">См. также</span><span class="sxs-lookup"><span data-stu-id="c254d-117">See Also</span></span>  
 <span data-ttu-id="c254d-118">[Удаление рабочих процессов](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-118">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="c254d-119">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-119">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="c254d-120">[Включение рабочих процессов](across-how-to-enable-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-120">[Enable Workflows](across-how-to-enable-workflows.md) </span></span>  
 <span data-ttu-id="c254d-121">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-121">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="c254d-122">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-122">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="c254d-123">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c254d-123">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="c254d-124">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="c254d-124">Workflow</span></span>](across-workflow.md)
