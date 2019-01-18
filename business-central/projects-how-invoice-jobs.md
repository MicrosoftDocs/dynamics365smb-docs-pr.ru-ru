---
title: "Создание счета продажи работы с целью выставления счета по работе | Документы Майкрософт"
description: "Описывается, как выставлять счета клиентам за расходы по работе по мере выполнения проекта."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 73894bb8c7193d96ca1f4c4f7c8b8394b1f26f5f
ms.contentlocale: ru-ru
ms.lasthandoff: 11/26/2018

---
# <a name="invoice-jobs"></a><span data-ttu-id="06df7-103">Выставление счетов за работы</span><span class="sxs-lookup"><span data-stu-id="06df7-103">Invoice Jobs</span></span>
<span data-ttu-id="06df7-104">Во время проекта могут накапливаться затраты на выполнение работы из-за потребления ресурсов, материалов и связанных с работой покупок.</span><span class="sxs-lookup"><span data-stu-id="06df7-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="06df7-105">В ходе выполнения работы, эти транзакции учитываются в журнале работ.</span><span class="sxs-lookup"><span data-stu-id="06df7-105">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="06df7-106">Важно, чтобы перед выставлением счета клиенту в журнал работ были занесены все затраты.</span><span class="sxs-lookup"><span data-stu-id="06df7-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

<span data-ttu-id="06df7-107">Программа позволяет выставить счет за всю работу на странице **Рабочее задание - строки** или только по выбранным строками "К оплате" на странице **Строки планирования**.</span><span class="sxs-lookup"><span data-stu-id="06df7-107">You can invoice the whole job from the **Job Task Lines** page or only invoice selected billable lines from the **Planning Lines** page.</span></span> <span data-ttu-id="06df7-108">Счета можно выставлять после завершения работы или через определенные промежутки времени в ходе выполнения работы согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="06df7-108">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

> [!NOTE]  
>   <span data-ttu-id="06df7-109">Если выбрать значение **К оплате** в поле **Тип строки работы** в документах покупки для связанных с работой покупок, то создаются строки планирования работ, которые готовы для выставления счета клиенту.</span><span class="sxs-lookup"><span data-stu-id="06df7-109">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="06df7-110">Дополнительные сведения см. в разделе [Управление запасами для проекта](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="06df7-110">For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-and-post-a-job-sales-invoice"></a><span data-ttu-id="06df7-111">Создание и учет счета продажи для работы</span><span class="sxs-lookup"><span data-stu-id="06df7-111">To create and post a job sales invoice</span></span>
<span data-ttu-id="06df7-112">Счет по работе или по одному или нескольким рабочим заданиям можно создавать, когда работа, по которой требуется выставить счет, завершена или при наступлении даты выставления счета согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="06df7-112">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="06df7-113">Со страницы **Работы** можно выставить клиенту счет, выбрав работу, затем выбрав действие **Создать счет продаж работ**.</span><span class="sxs-lookup"><span data-stu-id="06df7-113">From the **Jobs** page, you can invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> <span data-ttu-id="06df7-114">Приведенная ниже процедура показывает, как использовать пакетное задание для выставления счетов за несколько работ.</span><span class="sxs-lookup"><span data-stu-id="06df7-114">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="06df7-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работа - создание счета продажи**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="06df7-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="06df7-116">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="06df7-116">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="06df7-117">Установите фильтры, если требуется ограничить работы, которые будет обрабатывать пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="06df7-117">Set filters if you want to limit the jobs that the batch job will process.</span></span>
4. <span data-ttu-id="06df7-118">Нажмите кнопку **ОК**, чтобы создать счета.</span><span class="sxs-lookup"><span data-stu-id="06df7-118">Choose the **OK** button to create the invoices.</span></span>  

## <a name="to-create-multiple-job-sales-invoices-from-job-planning-lines"></a><span data-ttu-id="06df7-119">Создание нескольких счетов продажи по работам из строк планирования работы</span><span class="sxs-lookup"><span data-stu-id="06df7-119">To create multiple job sales invoices from job planning lines</span></span>
<span data-ttu-id="06df7-120">Можно создать счет из строк планирования работы и указать количество товара, ресурс или счет ГК, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="06df7-120">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="06df7-121">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="06df7-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="06df7-122">Откройте соответствующую работу.</span><span class="sxs-lookup"><span data-stu-id="06df7-122">Open a relevant job.</span></span>
3. <span data-ttu-id="06df7-123">Выберите рабочее задание, для которого поле **Тип рабочего задания** содержит значение **Учет**, затем выберите действие **Строки планирования работ**.</span><span class="sxs-lookup"><span data-stu-id="06df7-123">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="06df7-124">В строке планирования работы в поле **Переносимое в счет количество** введите количество товара, ресурса, типа счета Главной книги, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="06df7-124">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="06df7-125">Выберите действие **Создать счет продажи**.</span><span class="sxs-lookup"><span data-stu-id="06df7-125">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="06df7-126">На странице **Работа - создание счета продажи** введите дату учета и укажите, требуется ли создать новый счет или добавить этот счет в уже существующему.</span><span class="sxs-lookup"><span data-stu-id="06df7-126">On the **Job Create Sales Invoice** page, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="06df7-127">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="06df7-127">Choose the **OK** button.</span></span>  

    <span data-ttu-id="06df7-128">В строке планирования работы, в поле **Перенесенное в счет количество**, можно увидеть, количество.</span><span class="sxs-lookup"><span data-stu-id="06df7-128">On the job planning line, in the **Qty. Transferred to Invoice** field, you can see the quantity.</span></span>
8. <span data-ttu-id="06df7-129">На странице **Строки планирования работ** выберите действие **Счета продажи/кредит-ноты**.</span><span class="sxs-lookup"><span data-stu-id="06df7-129">On the **Job Planning Lines** page, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="06df7-130">Открывается страница **Счет продажи**, содержащая количество, которое было перемещено в счет.</span><span class="sxs-lookup"><span data-stu-id="06df7-130">The **Sales Invoice** page opens, showing the quantity that you have transferred to the invoice.</span></span>  
9. <span data-ttu-id="06df7-131">Внесите все дополнительные изменения, затем выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="06df7-131">Make any additional changes, and then choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="06df7-132">Приведенная выше процедура аналогична процедуре для создания, рассмотрения и учета кредит-ноты продажи, связанной с работой.</span><span class="sxs-lookup"><span data-stu-id="06df7-132">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="06df7-133">Расчет и учет операций выполнения работ</span><span class="sxs-lookup"><span data-stu-id="06df7-133">To calculate and post job completion entries</span></span>
<span data-ttu-id="06df7-134">После завершения всех действий по работе, включая учет потребления и выставление счетов, необходимо обновить работу, чтобы она получила **статус** **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="06df7-134">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="06df7-135">Затем необходимо обратить все НЗП, которые были учтены в главной книге.</span><span class="sxs-lookup"><span data-stu-id="06df7-135">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="06df7-136">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="06df7-136">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="06df7-137">Выберите открытую работу, затем выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="06df7-137">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="06df7-138">В поле **Статус** выберите **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="06df7-138">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="06df7-139">Следуйте шагам помощи для вычисления и учета НЗП.</span><span class="sxs-lookup"><span data-stu-id="06df7-139">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="06df7-140">Можно также выполнить шаги 5 и 6, чтобы сделать это вручную.</span><span class="sxs-lookup"><span data-stu-id="06df7-140">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="06df7-141">Выберите действие **Рассчитать НЗП**.</span><span class="sxs-lookup"><span data-stu-id="06df7-141">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="06df7-142">На странице **Расчет НЗП по работам** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="06df7-142">On the **Job Calculate WIP** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="06df7-143">У операций НЗП по работам, созданных пакетным заданием, появится флажок в поле **Работа выполнена**, указывающий, что они являются операциями выполнения.</span><span class="sxs-lookup"><span data-stu-id="06df7-143">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  
7. <span data-ttu-id="06df7-144">Выберите действие **Работа - учет НЗП в ГК**.</span><span class="sxs-lookup"><span data-stu-id="06df7-144">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="06df7-145">На странице **Работа - учет НЗП в ГК** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="06df7-145">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="06df7-146">У операций НЗП по работам в главной книге, созданных пакетным заданием, появится флажок в поле **Работа выполнена**, указывающий, что они являются операциями выполнения.</span><span class="sxs-lookup"><span data-stu-id="06df7-146">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="06df7-147">См. также</span><span class="sxs-lookup"><span data-stu-id="06df7-147">See Also</span></span>
[<span data-ttu-id="06df7-148">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="06df7-148">Managing Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="06df7-149">Финансы</span><span class="sxs-lookup"><span data-stu-id="06df7-149">Finance</span></span>](finance.md)  
<span data-ttu-id="06df7-150">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="06df7-150">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="06df7-151">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="06df7-151">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="06df7-152">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="06df7-152">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

