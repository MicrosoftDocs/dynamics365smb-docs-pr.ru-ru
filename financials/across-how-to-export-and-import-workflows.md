---
title: "Экспорт и импорт рабочих процессов | Документы Майкрософт"
description: "Для передачи рабочих процессов в другие базы данных Finance and Operations, Business edition, например для экономии времени при создании рабочих процессов, рабочие процессы можно экспортировать и импортировать."
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
ms.openlocfilehash: 6da772f9eefab9aa0ef8b9f47f6ea7656ebef1b4
ms.contentlocale: ru-ru
ms.lasthandoff: 01/30/2018

---
# <a name="export-and-import-workflows"></a><span data-ttu-id="6bb5f-103">Экспорт и импорт рабочих процессов</span><span class="sxs-lookup"><span data-stu-id="6bb5f-103">Export and Import Workflows</span></span>
<span data-ttu-id="6bb5f-104">Для передачи рабочих процессов в другие базы данных [!INCLUDE[d365fin](includes/d365fin_md.md)], например для экономии времени при создании рабочих процессов, рабочие процессы можно экспортировать и импортировать.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="6bb5f-105">Другой способ быстрого создания рабочих процессов — создание рабочих процессов из шаблонов рабочих процессов.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="6bb5f-106">Дополнительные сведения см. в разделе [Создание рабочих процессов из шаблонов рабочих процессов](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="6bb5f-106">For more information, see [Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="6bb5f-107">В окне **Рабочий процесс** создайте рабочий процесс, указав в строках связанные с ним шаги.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="6bb5f-108">Каждый шаг состоит из события рабочего процесса, ограниченного условиями события, и отклика рабочего процесса, ограниченного параметрами отклика.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="6bb5f-109">Шаги рабочего процесса заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="6bb5f-110">Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="6bb5f-110">For more information, see [Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="6bb5f-111">Экспорт рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="6bb5f-111">To export a workflow</span></span>  
1.  <span data-ttu-id="6bb5f-112">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6bb5f-113">Выберите рабочий процесс, затем выберите действие **Экспортировать в файл**.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="6bb5f-114">В диалоговом окне **Экспорт файла** нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="6bb5f-115">В окне **Экспорт** выберите расположение файла и затем нажмите кнопку **Сохранить**.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="6bb5f-116">Импорт рабочего процесса</span><span class="sxs-lookup"><span data-stu-id="6bb5f-116">To import a workflow</span></span>  
1.  <span data-ttu-id="6bb5f-117">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Рабочие процессы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6bb5f-118">Выберите действие **Импорт из файла**.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="6bb5f-119">В окне **Импорт** выберите XML-файл, содержащий рабочий процесс, а затем нажмите кнопку **Открыть**.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="6bb5f-120">Если код рабочего процесса уже есть в базе данных, шаги рабочего процесса будут перезаписаны шагами в импортированном рабочем процессе.</span><span class="sxs-lookup"><span data-stu-id="6bb5f-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6bb5f-121">См. также</span><span class="sxs-lookup"><span data-stu-id="6bb5f-121">See Also</span></span>  
 <span data-ttu-id="6bb5f-122">[Создание рабочих процессов](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-122">[Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="6bb5f-123">[Создание рабочих процессов из шаблонов рабочих процессов](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-123">[Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="6bb5f-124">[Просмотр архивированных экземпляров шагов рабочих процессов](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-124">[View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="6bb5f-125">[Удаление рабочих процессов](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-125">[Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="6bb5f-126">[Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="6bb5f-127">[Настройка рабочих процессов](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="6bb5f-128">[Использование рабочих процессов](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="6bb5f-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="6bb5f-129">Рабочий процесс</span><span class="sxs-lookup"><span data-stu-id="6bb5f-129">Workflow</span></span>](across-workflow.md)   

