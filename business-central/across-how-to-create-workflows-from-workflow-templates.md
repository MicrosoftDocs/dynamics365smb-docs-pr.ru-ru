---
title: Создание рабочих процессов из шаблонов рабочих процессов | Документы Майкрософт
description: Для экономии времени при создании новых рабочих процессов можно создавать рабочие процессы из шаблонов рабочих процессов.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 0ae5a7a308568dd8ede10c485564824685963bf4
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805194"
---
# <a name="create-workflows-from-workflow-templates"></a><span data-ttu-id="35cca-103">Создание рабочих процессов из шаблонов рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="35cca-103">Create Workflows from Workflow Templates</span></span>
<span data-ttu-id="35cca-104">Для экономии времени при создании новых рабочих процессов можно создавать рабочие процессы из шаблонов рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="35cca-104">To save time when creating new workflows, you can create workflows from workflow templates.</span></span>  

 <span data-ttu-id="35cca-105">Шаблоны рабочих процессов не подлежат редактированию и существуют в универсальной версии [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="35cca-105">Workflow templates are non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="35cca-106">Коды для шаблонов рабочих процессов, добавленных Майкрософт, имеют приставку "MS-".</span><span class="sxs-lookup"><span data-stu-id="35cca-106">The codes for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span>  

 <span data-ttu-id="35cca-107">Другой способ быстрого создания рабочего процесса — импорт существующего рабочего процесса из файла за пределами [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="35cca-107">Another way to quickly create a workflow is to import an existing workflow that you have on a file outside of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="35cca-108">Дополнительные сведения см. в разделе [Экспорт и импорт рабочих процессов](across-how-to-export-and-import-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="35cca-108">For more information, see [Export and Import Workflows](across-how-to-export-and-import-workflows.md).</span></span>  

<span data-ttu-id="35cca-109">На странице **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="35cca-109">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="35cca-110">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="35cca-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="35cca-111">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="35cca-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="35cca-112">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="35cca-112">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-create-a-workflow-from-workflow-template"></a><span data-ttu-id="35cca-113">Создание рабочего процесса из шаблона рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="35cca-113">To create a workflow from workflow template</span></span>  
1.  <span data-ttu-id="35cca-114">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="35cca-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="35cca-115">Выберите действие **Создать рабочий процесс из шаблона**.</span><span class="sxs-lookup"><span data-stu-id="35cca-115">Choose the **Create Workflow from Template** action.</span></span> <span data-ttu-id="35cca-116">Открывается страница **Шаблоны рабочих процессов**.</span><span class="sxs-lookup"><span data-stu-id="35cca-116">The **Workflow Templates** page opens.</span></span>  
3.  <span data-ttu-id="35cca-117">Выберите рабочий процесс, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="35cca-117">Select a workflow template, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="35cca-118">Откроется страница **Рабочий процесс** для нового рабочего процесса, содержащее всю информацию из выбранного шаблона.</span><span class="sxs-lookup"><span data-stu-id="35cca-118">The **Workflow** page opens for a new workflow containing all the information of the selected template.</span></span> <span data-ttu-id="35cca-119">Значение в поле **Код** дополняется символами, например "01", которые указывают, что это первый рабочий процесс, созданный на основе шаблона рабочего процесса.</span><span class="sxs-lookup"><span data-stu-id="35cca-119">The value in the **Code** field is extended with, for example, “-01” to indicate that this is the first workflow that is created from the workflow template.</span></span>  
4.  <span data-ttu-id="35cca-120">Для продолжения создания потока операций измените шаги рабочего процесса или добавьте новые.</span><span class="sxs-lookup"><span data-stu-id="35cca-120">Proceed to create the workflow by editing the workflow steps or add new steps.</span></span> <span data-ttu-id="35cca-121">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="35cca-121">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="35cca-122">См. также</span><span class="sxs-lookup"><span data-stu-id="35cca-122">See Also</span></span>  
 <span data-ttu-id="35cca-123">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-123">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="35cca-124">[Экспорт и импорт рабочих процессов](across-how-to-export-and-import-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-124">[Export and Import Workflows](across-how-to-export-and-import-workflows.md) </span></span>  
 <span data-ttu-id="35cca-125">[Просмотр архивированных экземпляров шагов рабочих процессов](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-125">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="35cca-126">[Удаление рабочих процессов](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-126">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="35cca-127">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-127">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="35cca-128">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-128">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="35cca-129">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="35cca-129">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="35cca-130">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="35cca-130">Workflow</span></span>](across-workflow.md)   
