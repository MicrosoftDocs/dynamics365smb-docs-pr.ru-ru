---
title: Настройка и управление бюджетом для работы | Документация Майкрософт
description: Далее описывается процедура планирования ресурсов и прогнозирования и контроля себестоимости для проекта путем настройки бюджета для каждой работы.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project budget, forecast
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: e8de8d35ee036d2819ba40b1fdf50b6d5ed2dab5
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3913175"
---
# <a name="manage-job-budgets"></a><span data-ttu-id="e8a82-103">Управление бюджетами работ</span><span class="sxs-lookup"><span data-stu-id="e8a82-103">Manage Job Budgets</span></span>
<span data-ttu-id="e8a82-104">Бюджет можно настроить для каждой работы.</span><span class="sxs-lookup"><span data-stu-id="e8a82-104">You can set up a budget for each job.</span></span> <span data-ttu-id="e8a82-105">Бюджет необходим для планирования ресурсов, выделенных для выполнения работы.</span><span class="sxs-lookup"><span data-stu-id="e8a82-105">The budget is used to plan the resources that you allocate to a job.</span></span> <span data-ttu-id="e8a82-106">Бюджет может быть общим, с небольшим количеством операций, или же он может содержать больше операций, которые разделены по уровням деятельности.</span><span class="sxs-lookup"><span data-stu-id="e8a82-106">The budget can be either general with few entries or it can contain more entries that are divided into activity levels.</span></span> <span data-ttu-id="e8a82-107">Затем можно сравнивать бюджетные суммы с фактическим потреблением, занесенным в журнал работ.</span><span class="sxs-lookup"><span data-stu-id="e8a82-107">You can then compare the budgeted amounts with the actual usage as recorded in the job journal.</span></span> <span data-ttu-id="e8a82-108">Контролируя различия между фактическим и бюджетным потреблением, можно контролировать текущий проект и улучшить качество будущих работ за счет снижения риска неправильной оценки затрат.</span><span class="sxs-lookup"><span data-stu-id="e8a82-108">By monitoring differences between actual usage and budgeted usage, you can control an ongoing project and improve the quality of future jobs by reducing the risk of underestimating costs.</span></span>

<span data-ttu-id="e8a82-109">Следующая процедура показывает, как оценить бюджетные затраты во время планирования.</span><span class="sxs-lookup"><span data-stu-id="e8a82-109">The following procedure describes how to estimate budgeted costs during planning.</span></span> <span data-ttu-id="e8a82-110">Информацию о регистрации бюджетных и фактических цен и затрат для работ см. в разделе [Регистрация потребления для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="e8a82-110">For information about recording budgeted versus actual job prices and costs, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>  

## <a name="to-estimate-the-budgeted-costs-for-a-job"></a><a name="JobBudgetCosts"></a> <span data-ttu-id="e8a82-111">Оценка бюджетных затрат для работы</span><span class="sxs-lookup"><span data-stu-id="e8a82-111">To estimate the budgeted costs for a job</span></span>
<span data-ttu-id="e8a82-112">Когда клиент хочет знать цену работы, накладная по которой будет выставлена на основе потребления, необходимо определить бюджетные затраты на работу.</span><span class="sxs-lookup"><span data-stu-id="e8a82-112">When a customer wants to know the price of a job that will be invoiced based on usage, you must have to determine the budgeted costs for the job.</span></span> <span data-ttu-id="e8a82-113">Для этого используйте страницу **Строки задач по работе**.</span><span class="sxs-lookup"><span data-stu-id="e8a82-113">You use the **Job Task Lines** page to do this.</span></span>

1. <span data-ttu-id="e8a82-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Задания**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e8a82-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e8a82-115">Откройте соответствующую работу.</span><span class="sxs-lookup"><span data-stu-id="e8a82-115">Open a relevant job.</span></span>
3. <span data-ttu-id="e8a82-116">Выделите строку задачи типа "Учет", затем выберите действие **Строки планирования работ**.</span><span class="sxs-lookup"><span data-stu-id="e8a82-116">Select a task line of type Posting, and then choose the **Job Planning Lines** action.</span></span>
4. <span data-ttu-id="e8a82-117">На новой строке заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="e8a82-117">On a new line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]   

<span data-ttu-id="e8a82-118">Для поля **Тип строки** см. следующую информацию.</span><span class="sxs-lookup"><span data-stu-id="e8a82-118">For the **Line Type** field, refer to the following information.</span></span>  

| <span data-ttu-id="e8a82-119">Тип строки</span><span class="sxs-lookup"><span data-stu-id="e8a82-119">Line Type</span></span> | <span data-ttu-id="e8a82-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8a82-120">Description</span></span> |
| --- | --- |
| <span data-ttu-id="e8a82-121">**Бюджет и к оплате**</span><span class="sxs-lookup"><span data-stu-id="e8a82-121">**Both Budget and Billable**</span></span> |<span data-ttu-id="e8a82-122">Суммы затрат и цен, введенные в строку планирования, представляют собой бюджетные затраты для данной строки планирования.</span><span class="sxs-lookup"><span data-stu-id="e8a82-122">The cost and price amounts entered on the planning line are the budgeted costs for the particular planning line.</span></span> <span data-ttu-id="e8a82-123">По этой цене будет выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="e8a82-123">The price amount will be invoiced.</span></span> |
| <span data-ttu-id="e8a82-124">**Бюджет**</span><span class="sxs-lookup"><span data-stu-id="e8a82-124">**Budget**</span></span> |<span data-ttu-id="e8a82-125">Клиенту не оплачивает потребление.</span><span class="sxs-lookup"><span data-stu-id="e8a82-125">The customer is not charged for usage.</span></span> <span data-ttu-id="e8a82-126">Потребление не может быть переведено в счет, но будет использоваться в расчете НЗП.</span><span class="sxs-lookup"><span data-stu-id="e8a82-126">Usage is not transferred to an invoice, but will still be used in the calculation of WIP.</span></span> |
| <span data-ttu-id="e8a82-127">**К оплате**</span><span class="sxs-lookup"><span data-stu-id="e8a82-127">**Billable**</span></span> |<span data-ttu-id="e8a82-128">Клиенту оплачивает потребление.</span><span class="sxs-lookup"><span data-stu-id="e8a82-128">The customer is charged for usage.</span></span> <span data-ttu-id="e8a82-129">Потребление переводится в счет на основании количества, указанного в поле Переносимое в счет количество.</span><span class="sxs-lookup"><span data-stu-id="e8a82-129">Usage is transferred to the invoice, based on the quantity specified in the Qty. to Transfer to Invoice field.</span></span> |

> [!NOTE]  
> <span data-ttu-id="e8a82-130">Поле **Плановая дата доставки** для строки планирования содержит дата, когда ожидается завершение потребления, связанного со строкой планирования.</span><span class="sxs-lookup"><span data-stu-id="e8a82-130">The **Planned Delivery Date** field for the planning line contains the date when usage related to the planning line is expected to be completed.</span></span> <span data-ttu-id="e8a82-131">Это также дата, когда строка планирования может быть перенесена в счет по продаже и учтена.</span><span class="sxs-lookup"><span data-stu-id="e8a82-131">It is also the date when the planning line may be transferred to a sales invoice and posted.</span></span> <br /><br /> <span data-ttu-id="e8a82-132">В базовой задаче работы на странице **Карточка работы** поля **Дата начала** и **Дата окончания** содержат, соответственно, значение поля **Плановая дата доставки** на самой ранней и самой поздней строках планирования работы на связанной странице **Строки планирования работ**.</span><span class="sxs-lookup"><span data-stu-id="e8a82-132">On the underlying job task on the **Job Card** page, the **Start Date** and **End Date** fields respectively contain the value of the **Planned Delivery Date** field on the earliest and latest job planning lines in the related **Job Planning Lines** page.</span></span>

> [!NOTE]  
>   <span data-ttu-id="e8a82-133">При заполнении поля **Количество** вся информация об общих ценах и затратах будет рассчитана и заполнена для данной строки планирования.</span><span class="sxs-lookup"><span data-stu-id="e8a82-133">When you fill in the **Quantity** field, all total price and total cost information will be calculated and filled in for that planning line.</span></span> <span data-ttu-id="e8a82-134">Ее можно изменить в любое время.</span><span class="sxs-lookup"><span data-stu-id="e8a82-134">You can edit them at any time.</span></span>

<span data-ttu-id="e8a82-135">На странице **Карточка работы** можно увидеть общие бюджетные затраты, бюджетную цену, себестоимость к оплате и сумму к оплате для каждой задачи.</span><span class="sxs-lookup"><span data-stu-id="e8a82-135">On the **Job Card** page, you can now see a summary of the total budgeted costs, budgeted price, billable cost and billable price for each task.</span></span>

<span data-ttu-id="e8a82-136">Информацию о регистрации бюджетных и фактических цен и затрат для работ см. в разделе [Регистрация потребления для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="e8a82-136">For information about recording budgeted versus actual job prices and costs, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="e8a82-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e8a82-137">See Also</span></span>
[<span data-ttu-id="e8a82-138">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="e8a82-138">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="e8a82-139">Финансы</span><span class="sxs-lookup"><span data-stu-id="e8a82-139">Finance</span></span>](finance.md)  
<span data-ttu-id="e8a82-140">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="e8a82-140">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="e8a82-141">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="e8a82-141">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="e8a82-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e8a82-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
