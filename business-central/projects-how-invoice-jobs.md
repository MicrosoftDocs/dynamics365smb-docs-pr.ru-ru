---
title: Создание счета продажи работы с целью выставления счета по работе | Документация Майкрософт
description: Описывается, как выставлять счета клиентам за расходы по работе по мере выполнения проекта.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project invoice
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 873135d2fa6053b7101a999981fb3117ee8689ab
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938150"
---
# <a name="invoice-jobs"></a><span data-ttu-id="d398b-103">Выставление счетов за работы</span><span class="sxs-lookup"><span data-stu-id="d398b-103">Invoice Jobs</span></span>
<span data-ttu-id="d398b-104">Во время проекта могут накапливаться затраты на выполнение работы из-за потребления ресурсов, материалов и связанных с работой покупок.</span><span class="sxs-lookup"><span data-stu-id="d398b-104">During the project, job costs from resource usage, materials, and job-related purchases can accumulate.</span></span> <span data-ttu-id="d398b-105">В ходе выполнения работы, эти транзакции учитываются в журнале работ.</span><span class="sxs-lookup"><span data-stu-id="d398b-105">As the job progresses, these transactions get posted to the job journal.</span></span> <span data-ttu-id="d398b-106">Важно, чтобы перед выставлением счета клиенту в журнал работ были занесены все затраты.</span><span class="sxs-lookup"><span data-stu-id="d398b-106">It is important that all costs get recorded in the job journal before you invoice the customer.</span></span>

> [!NOTE]
> <span data-ttu-id="d398b-107">Вы также можете приобрести внешние ресурсы, не связанные с работой, например, чтобы выставить счет поставщику за выполненную работу.</span><span class="sxs-lookup"><span data-stu-id="d398b-107">You can also purchase external resources unrelated to a job, for example, to invoice a vendor for work delivered.</span></span> <span data-ttu-id="d398b-108">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="d398b-108">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

<span data-ttu-id="d398b-109">Программа позволяет выставить счет за всю работу на странице **Рабочее задание - строки** или только по выбранным строками "К оплате" на странице **Строки планирования**.</span><span class="sxs-lookup"><span data-stu-id="d398b-109">You can invoice the whole job from the **Job Task Lines** page or only invoice selected billable lines from the **Planning Lines** page.</span></span> <span data-ttu-id="d398b-110">Счета можно выставлять после завершения работы или через определенные промежутки времени в ходе выполнения работы согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d398b-110">Invoicing can be done after the job is finished or at certain intervals during the job's progress based on an invoicing schedule.</span></span>

> [!NOTE]  
> <span data-ttu-id="d398b-111">Если выбрать значение **К оплате** в поле **Тип строки работы** в документах покупки для связанных с работой покупок, то создаются строки планирования работ, которые готовы для выставления счета клиенту.</span><span class="sxs-lookup"><span data-stu-id="d398b-111">If you select **Billable** in the **Job Line Type** field on the purchase documents for job-related purchases, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="d398b-112">Дополнительные сведения см. в разделе [Управление запасами для проекта](projects-how-manage-project-supplies.md).</span><span class="sxs-lookup"><span data-stu-id="d398b-112">For more information, see [Manage Project Supplies](projects-how-manage-project-supplies.md).</span></span>

## <a name="to-create-multiple-job-sales-invoices"></a><span data-ttu-id="d398b-113">Создание нескольких счетов продажи по работам</span><span class="sxs-lookup"><span data-stu-id="d398b-113">To create multiple job sales invoices</span></span>
<span data-ttu-id="d398b-114">Счет по работе или по одному или нескольким рабочим заданиям можно создавать, когда работа, по которой требуется выставить счет, завершена или при наступлении даты выставления счета согласно плану выставления счетов.</span><span class="sxs-lookup"><span data-stu-id="d398b-114">You can create an invoice for a job or for one or more job tasks for a customer when either the work to be invoiced is complete or the date for invoicing based on an invoicing schedule has been reached.</span></span>

<span data-ttu-id="d398b-115">Приведенная ниже процедура показывает, как использовать пакетное задание для выставления счетов за несколько работ.</span><span class="sxs-lookup"><span data-stu-id="d398b-115">The following procedure shows how to use a batch job to invoice multiple jobs.</span></span>  

1. <span data-ttu-id="d398b-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работа - создать счет продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d398b-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job Create Sales Invoice**, and then choose the related link.</span></span>  
2. <span data-ttu-id="d398b-117">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="d398b-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="d398b-118">Установите фильтры, если требуется ограничить работы, которые будет обрабатывать пакетное задание.</span><span class="sxs-lookup"><span data-stu-id="d398b-118">Set filters if you want to limit the jobs that the batch job will process.</span></span>
4. <span data-ttu-id="d398b-119">Нажмите кнопку **ОК**, чтобы создать счета.</span><span class="sxs-lookup"><span data-stu-id="d398b-119">Choose the **OK** button to create the invoices.</span></span>  

<span data-ttu-id="d398b-120">Вы можете просмотреть и опубликовать созданные счета в окне **Счета продаж**.</span><span class="sxs-lookup"><span data-stu-id="d398b-120">You can review and post created invoices in the **Sales Invoices** window.</span></span>

> [!NOTE]
> <span data-ttu-id="d398b-121">Вы также можете выставить клиенту счет, выбрав работу, затем выбрав действие **Создать счет продаж работ**.</span><span class="sxs-lookup"><span data-stu-id="d398b-121">Alternatively, invoice a customer by selecting the job, and then choosing the **Create Job Sales Invoice** action.</span></span> 

## <a name="to-create-and-post-job-sales-invoice-from-job-planning-lines"></a><span data-ttu-id="d398b-122">Создание и учет счета продажи по работе из строк планирования работы</span><span class="sxs-lookup"><span data-stu-id="d398b-122">To create and post job sales invoice from job planning lines</span></span>
<span data-ttu-id="d398b-123">Можно создать счет из строк планирования работы и указать количество товара, ресурс или счет ГК, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="d398b-123">You can create an invoice from a job planning lines, and indicate at that time the quantity of the item, resource, or general ledger account that you want to invoice.</span></span>

1. <span data-ttu-id="d398b-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="d398b-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="d398b-125">Откройте соответствующую работу.</span><span class="sxs-lookup"><span data-stu-id="d398b-125">Open a relevant job.</span></span>
3. <span data-ttu-id="d398b-126">Выберите рабочее задание, для которого поле **Тип рабочего задания** содержит значение **Учет**, затем выберите действие **Строки планирования работ**.</span><span class="sxs-lookup"><span data-stu-id="d398b-126">Select a job task for which the **Job Task Type** field contains **Posting**, and then choose the **Job Planning Lines** action.</span></span>  
4. <span data-ttu-id="d398b-127">В строке планирования работы в поле **Переносимое в счет количество** введите количество товара, ресурса, типа счета Главной книги, по которому следует выставить счет.</span><span class="sxs-lookup"><span data-stu-id="d398b-127">On a job planning line, in the **Qty. To Transfer to Invoice** field, enter the quantity of the item, resource, general ledger account type that you want to invoice.</span></span>  
5. <span data-ttu-id="d398b-128">Выберите действие **Создать счет продажи**.</span><span class="sxs-lookup"><span data-stu-id="d398b-128">Choose the **Create Sales Invoice** action.</span></span>
6. <span data-ttu-id="d398b-129">На странице **Работа - создание счета продажи** введите дату учета и укажите, требуется ли создать новый счет или добавить этот счет в уже существующему.</span><span class="sxs-lookup"><span data-stu-id="d398b-129">On the **Job Create Sales Invoice** page, enter the posting date and whether you want to create a new invoice or append this invoice to an existing one.</span></span>
7. <span data-ttu-id="d398b-130">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="d398b-130">Choose the **OK** button.</span></span>  
8. <span data-ttu-id="d398b-131">На странице **Строки планирования работ** выберите действие **Счета продажи/кредит-ноты**.</span><span class="sxs-lookup"><span data-stu-id="d398b-131">On the **Job Planning Lines** page, choose the **Sales Invoices/Credit Memos** action.</span></span>

    <span data-ttu-id="d398b-132">Открывается страница **Счет продажи**, содержащая количество, которое было перемещено в счет.</span><span class="sxs-lookup"><span data-stu-id="d398b-132">The **Sales Invoice** page opens, showing the quantity that you have transferred to the invoice.</span></span>
9. <span data-ttu-id="d398b-133">Внесите все дополнительные изменения, затем выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="d398b-133">Make any additional changes, and then choose the **Post** action.</span></span>

> [!NOTE]  
>   <span data-ttu-id="d398b-134">Приведенная выше процедура аналогична процедуре для создания, рассмотрения и учета кредит-ноты продажи, связанной с работой.</span><span class="sxs-lookup"><span data-stu-id="d398b-134">The above procedure is similar for creating, reviewing, and posting a job-related sales credit memo.</span></span>


## <a name="see-also"></a><span data-ttu-id="d398b-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d398b-135">See Also</span></span>
[<span data-ttu-id="d398b-136">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="d398b-136">Managing Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="d398b-137">Финансы</span><span class="sxs-lookup"><span data-stu-id="d398b-137">Finance</span></span>](finance.md)  
<span data-ttu-id="d398b-138">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="d398b-138">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="d398b-139">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="d398b-139">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="d398b-140">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d398b-140">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]
