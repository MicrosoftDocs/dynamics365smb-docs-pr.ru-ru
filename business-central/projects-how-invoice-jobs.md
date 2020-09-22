---
title: Создание счета продажи работы с целью выставления счета по работе | Документация Майкрософт
description: Описывается, как выставлять счета клиентам за расходы по работе по мере выполнения проекта.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 05/25/2020
ms.author: edupont
ms.openlocfilehash: 66e5dd52eb01e8a396156d0c646a43916fdc0021
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3783961"
---
# <a name="invoice-jobs"></a><span data-ttu-id="1fbe6-103">Выставление счетов за работы</span><span class="sxs-lookup"><span data-stu-id="1fbe6-103">Invoice Jobs</span></span>
<span data-ttu-id="1fbe6-104">Во время проекта могут накапливаться затраты на выполнение работы из-за потребления ресурсов, материалов и связанных с работой покупок.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="1fbe6-105">В ходе выполнения работы, эти транзакции учитываются в журнале работ.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-105">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="1fbe6-106">Важно, чтобы перед выставлением счета клиенту в журнал работ были занесены все затраты.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

> [!NOTE]
> <span data-ttu-id="1fbe6-107">Вы также можете приобрести внешние ресурсы, не связанные с работой, например, чтобы выставить счет поставщику за выполненную работу.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-107">You can also purchase external resources unrelated to a job, for example, to invoice a vendor for work delivered.</span></span> <span data-ttu-id="1fbe6-108">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="1fbe6-108">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

<span data-ttu-id="1fbe6-109">Программа позволяет выставить счет за всю работу на странице **Рабочее задание - строки** или только по выбранным строками "К оплате" на странице **Строки планирования**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-109">You can invoice the whole job from the **Job Task Lines** page or only invoice selected billable lines from the **Planning Lines** page.</span></span> <span data-ttu-id="1fbe6-110">Счета можно выставлять после завершения работы или через определенные промежутки времени в ходе выполнения работы согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-110">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

> [!NOTE]  
> <span data-ttu-id="1fbe6-111">Если выбрать значение **К оплате** в поле **Тип строки работы** в документах покупки для связанных с работой покупок, то создаются строки планирования работ, которые готовы для выставления счета клиенту.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-111">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="1fbe6-112">Дополнительные сведения см. в разделе [Управление запасами для проекта](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="1fbe6-112">For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-multiple-job-sales-invoices"></a><span data-ttu-id="1fbe6-113">Создание нескольких счетов продажи по работам</span><span class="sxs-lookup"><span data-stu-id="1fbe6-113">To create multiple job sales invoices</span></span>
<span data-ttu-id="1fbe6-114">Счет по работе или по одному или нескольким рабочим заданиям можно создавать, когда работа, по которой требуется выставить счет, завершена или при наступлении даты выставления счета согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-114">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="1fbe6-115">Приведенная ниже процедура показывает, как использовать пакетное задание для выставления счетов за несколько работ.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-115">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="1fbe6-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работа - создать счет продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1fbe6-117">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="1fbe6-118">Установите фильтры, если требуется ограничить работы, которые будет обрабатывать пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-118">Set filters if you want to limit the jobs that the batch job will process.</span></span>
4. <span data-ttu-id="1fbe6-119">Нажмите кнопку **ОК**, чтобы создать счета.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-119">Choose the **OK** button to create the invoices.</span></span>  

<span data-ttu-id="1fbe6-120">Вы можете просмотреть и опубликовать созданные счета в окне **Счета продаж**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-120">You can review and post created invoices in the **Sales Invoices** window.</span></span>

> [!NOTE]
> <span data-ttu-id="1fbe6-121">Вы также можете выставить клиенту счет, выбрав работу, затем выбрав действие **Создать счет продаж работ**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-121">Alternatively, invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> 

## <a name="to-create-and-post-job-sales-invoice-from-job-planning-lines"></a><span data-ttu-id="1fbe6-122">Создание и учет счета продажи по работе из строк планирования работы</span><span class="sxs-lookup"><span data-stu-id="1fbe6-122">To create and post job sales invoice from job planning lines</span></span>
<span data-ttu-id="1fbe6-123">Можно создать счет из строк планирования работы и указать количество товара, ресурс или счет ГК, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-123">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="1fbe6-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="1fbe6-125">Откройте соответствующую работу.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-125">Open a relevant job.</span></span>
3. <span data-ttu-id="1fbe6-126">Выберите рабочее задание, для которого поле **Тип рабочего задания** содержит значение **Учет**, затем выберите действие **Строки планирования работ**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-126">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="1fbe6-127">В строке планирования работы в поле **Переносимое в счет количество** введите количество товара, ресурса, типа счета Главной книги, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-127">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="1fbe6-128">Выберите действие **Создать счет продажи**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-128">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="1fbe6-129">На странице **Работа - создание счета продажи** введите дату учета и укажите, требуется ли создать новый счет или добавить этот счет в уже существующему.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-129">On the **Job Create Sales Invoice** page, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="1fbe6-130">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-130">Choose the **OK** button.</span></span>  
8. <span data-ttu-id="1fbe6-131">На странице **Строки планирования работ** выберите действие **Счета продажи/кредит-ноты**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-131">On the **Job Planning Lines** page, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="1fbe6-132">Открывается страница **Счет продажи**, содержащая количество, которое было перемещено в счет.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-132">The **Sales Invoice** page opens, showing the quantity that you have transferred to the invoice.</span></span>
9. <span data-ttu-id="1fbe6-133">Внесите все дополнительные изменения, затем выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-133">Make any additional changes, and then choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="1fbe6-134">Приведенная выше процедура аналогична процедуре для создания, рассмотрения и учета кредит-ноты продажи, связанной с работой.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-134">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>

## <a name="to-calculate-and-post-job-completion-entries"></a><span data-ttu-id="1fbe6-135">Расчет и учет операций выполнения работ</span><span class="sxs-lookup"><span data-stu-id="1fbe6-135">To calculate and post job completion entries</span></span>
<span data-ttu-id="1fbe6-136">После завершения всех действий по работе, включая учет потребления и выставление счетов, необходимо обновить работу, чтобы она получила **статус** **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-136">When you have completed all activities for a job, including usage posting and invoicing, you must update the job to have a **Status** of **Completed**.</span></span> <span data-ttu-id="1fbe6-137">Затем необходимо обратить все НЗП, которые были учтены в главной книге.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-137">Then, you must reverse any WIP that has been posted to the general ledger.</span></span>

1. <span data-ttu-id="1fbe6-138">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-138">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>  
2. <span data-ttu-id="1fbe6-139">Выберите открытую работу, затем выберите действие **Изменить**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-139">Select an open job, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="1fbe6-140">В поле **Статус** выберите **Завершено**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-140">In the **Status** field, select **Completed**.</span></span>
4. <span data-ttu-id="1fbe6-141">Следуйте шагам помощи для вычисления и учета НЗП.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-141">Follow the assistance steps to calculate and post WIP.</span></span> <span data-ttu-id="1fbe6-142">Можно также выполнить шаги 5 и 6, чтобы сделать это вручную.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-142">Alternatively, follows steps 5 and 6 to do so manually.</span></span>  
5. <span data-ttu-id="1fbe6-143">Выберите действие **Рассчитать НЗП**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-143">Choose the **Calculate WIP** action.</span></span>
6. <span data-ttu-id="1fbe6-144">На странице **Расчет НЗП по работам** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-144">On the **Job Calculate WIP** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="1fbe6-145">У операций НЗП по работам, созданных пакетным заданием, появится флажок в поле **Работа выполнена**, указывающий, что они являются операциями выполнения.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-145">The job WIP entries created by running the batch job will have the **Job Complete** check box selected to show that they are completion entries.</span></span>  
7. <span data-ttu-id="1fbe6-146">Выберите действие **Работа - учет НЗП в ГК**.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-146">Choose the **Job Post WIP to G/L** action.</span></span>
8. <span data-ttu-id="1fbe6-147">На странице **Работа - учет НЗП в ГК** заполните требуемые поля.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-147">On the **Job Post WIP to G/L** page, fill in the fields as necessary.</span></span>  

     <span data-ttu-id="1fbe6-148">У операций НЗП по работам в главной книге, созданных пакетным заданием, появится флажок в поле **Работа выполнена**, указывающий, что они являются операциями выполнения.</span><span class="sxs-lookup"><span data-stu-id="1fbe6-148">The job WIP general ledger entries created by running the batch job will have the **Job Complete** check box selected to show they are completion entries.</span></span>

## <a name="see-also"></a><span data-ttu-id="1fbe6-149">См. также</span><span class="sxs-lookup"><span data-stu-id="1fbe6-149">See Also</span></span>
[<span data-ttu-id="1fbe6-150">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="1fbe6-150">Managing Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="1fbe6-151">Финансы</span><span class="sxs-lookup"><span data-stu-id="1fbe6-151">Finance</span></span>](finance.md)  
<span data-ttu-id="1fbe6-152">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="1fbe6-152">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="1fbe6-153">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="1fbe6-153">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="1fbe6-154">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="1fbe6-154">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
