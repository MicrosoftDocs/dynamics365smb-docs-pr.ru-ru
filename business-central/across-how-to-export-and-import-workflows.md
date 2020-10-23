---
title: Экспорт и импорт рабочих процессов | Документация Майкрософт
description: Для передачи рабочих процессов в другие базы данных Business Central, например для экономии времени при создании рабочих процессов, рабочие процессы можно экспортировать и импортировать.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 803af5e396df2a3eade763bfce1172a7a2627da2
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916222"
---
# <a name="export-and-import-workflows"></a><span data-ttu-id="c1ad8-103">Экспорт и импорт рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="c1ad8-103">Export and Import Workflows</span></span>
<span data-ttu-id="c1ad8-104">Для передачи рабочих процессов в другие базы данных [!INCLUDE[d365fin](includes/d365fin_md.md)], например для экономии времени при создании рабочих процессов, рабочие процессы можно экспортировать и импортировать.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="c1ad8-105">Другой способ быстрого создания рабочих процессов — создание рабочих процессов из шаблонов рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="c1ad8-106">Дополнительные сведения см. в разделе [Создание рабочих процессов из шаблонов рабочих процессов](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="c1ad8-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="c1ad8-107">На странице **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-107">On the **Workflow** page, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="c1ad8-108">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="c1ad8-109">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="c1ad8-110">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="c1ad8-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="c1ad8-111">Экспорт рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="c1ad8-111">To export a workflow</span></span>  
1.  <span data-ttu-id="c1ad8-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c1ad8-113">Выберите рабочий процесс, затем выберите действие **Экспортировать в файл**.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="c1ad8-114">На странице **Экспорт файла** нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-114">On the **Export File** page, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="c1ad8-115">На странице **Экспорт** выберите расположение файла и затем нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-115">On the **Export** page, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="c1ad8-116">Импорт рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="c1ad8-116">To import a workflow</span></span>  
1.  <span data-ttu-id="c1ad8-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c1ad8-118">Выберите действие **Импорт из файла**.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="c1ad8-119">На странице **Импорт** выберите XML-файл, содержащий рабочий процесс, а затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-119">On the **Import** page, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="c1ad8-120">Если код рабочего процесса уже есть в базе данных, шаги рабочего процесса будут перезаписаны шагами в импортированном рабочем процессе.</span><span class="sxs-lookup"><span data-stu-id="c1ad8-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c1ad8-121">См. также</span><span class="sxs-lookup"><span data-stu-id="c1ad8-121">See Also</span></span>  
 <span data-ttu-id="c1ad8-122">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="c1ad8-123">[Создание рабочих процессов из шаблонов рабочих процессов](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="c1ad8-124">[Просмотр архивированных экземпляров шагов рабочих процессов](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="c1ad8-125">[Удаление рабочих процессов](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="c1ad8-126">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="c1ad8-127">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="c1ad8-128">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="c1ad8-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="c1ad8-129">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="c1ad8-129">Workflow</span></span>](across-workflow.md)   
