---
title: "Покупка товаров или услуг для работы и управление запасами | Документы Майкрософт"
description: "Описывается, как управлять запасами и закупками материалов и услуг для работ."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 46cae53022ba5d65a370694c9818f52a7bf45525
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017


---
# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="e15ad-103">Практическое руководство. Управление запасами для работы</span><span class="sxs-lookup"><span data-stu-id="e15ad-103">How to: Manage Job Supplies</span></span>
<span data-ttu-id="e15ad-104">Управление поставками товаров, услуг и затратами по проекту является неотъемлемым и важным аспектом выполнения любых работ.</span><span class="sxs-lookup"><span data-stu-id="e15ad-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="e15ad-105">Программа позволяет пользоваться имеющимися запасами или, посредством заказов на покупку или счетов покупки, купить все необходимое для выполнения работы.</span><span class="sxs-lookup"><span data-stu-id="e15ad-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="e15ad-106">Пусть, например, для выполнения работы по обслуживанию компьютера необходим новый диск.</span><span class="sxs-lookup"><span data-stu-id="e15ad-106">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="e15ad-107">В этом случае необходимо создать новый счет покупки нового диска и записать работу, для которой он будет использован.</span><span class="sxs-lookup"><span data-stu-id="e15ad-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="e15ad-108">Если в процессе покупки не требуется отдельная запись физической транзакции, то покупка может быть обработана в окне **Журнал ГК работы**.</span><span class="sxs-lookup"><span data-stu-id="e15ad-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="e15ad-109">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация использования для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="e15ad-109">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="e15ad-110">Приобретение товаров или услуг для работы</span><span class="sxs-lookup"><span data-stu-id="e15ad-110">To purchase items or services for a job</span></span>
<span data-ttu-id="e15ad-111">В следующей процедуре показан порядок использования счета покупки для приобретения товаров для работы.</span><span class="sxs-lookup"><span data-stu-id="e15ad-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="e15ad-112">Эти же шаги применяются при использовании заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="e15ad-112">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="e15ad-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Счета покупки**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e15ad-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e15ad-114">Выберите действие **Создать** и введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="e15ad-114">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="e15ad-115">Дополнительные сведения см. в разделе [Практическое руководство. Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="e15ad-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="e15ad-116">В полях **Код работы**</span><span class="sxs-lookup"><span data-stu-id="e15ad-116">In the **Job No.**</span></span> <span data-ttu-id="e15ad-117">и **Номер рабочего задания**</span><span class="sxs-lookup"><span data-stu-id="e15ad-117">and **Job Task No.**</span></span> <span data-ttu-id="e15ad-118">выберите информацию о задании, для которой требуется приобрести товары или услуги.</span><span class="sxs-lookup"><span data-stu-id="e15ad-118">fields, select the information of the job that you want to purchase items or services for.</span></span> <span data-ttu-id="e15ad-119">Используйте функцию **Выбрать столбцы**, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="e15ad-119">Use the **Choose Columns** function if the field is not visible.</span></span> <span data-ttu-id="e15ad-120">Дополнительные сведения см. в разделе [Персонализация пользователя](ui-user-personalization.md).</span><span class="sxs-lookup"><span data-stu-id="e15ad-120">For more information, see [User Personalization](ui-user-personalization.md).</span></span>

    <span data-ttu-id="e15ad-121">Значение, выбранное в поле **Тип строки работы**, определяет, создается ли строка планирования во время учета потребления товара.</span><span class="sxs-lookup"><span data-stu-id="e15ad-121">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="e15ad-122">Если поле содержит значение **К оплате**, будут созданы строки планирования работы, по которым можно выставлять счет клиенту.</span><span class="sxs-lookup"><span data-stu-id="e15ad-122">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="e15ad-123">Дополнительные сведения см. в разделе [Практическое руководство. Выставление счетов за работы](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="e15ad-123">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>
4. <span data-ttu-id="e15ad-124">Выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="e15ad-124">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="e15ad-125">Просмотр значения покупок для работы</span><span class="sxs-lookup"><span data-stu-id="e15ad-125">To view the value of purchases for a job</span></span>
1. <span data-ttu-id="e15ad-126">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Работы**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e15ad-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="e15ad-127">Откройте соответствующую карточку работы.</span><span class="sxs-lookup"><span data-stu-id="e15ad-127">Open a relevant job card.</span></span>

    <span data-ttu-id="e15ad-128">На экспресс-вкладке **Задачи** поле **Невыполненные заказы** показывает общую сумму по невыполненным поставкам (в локальной валюте) товарно-материальных ценностей и услуг по документам на покупку для строки рабочего задания.</span><span class="sxs-lookup"><span data-stu-id="e15ad-128">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="e15ad-129">Поле **Сумма, полученная без выст. счета** показывает объем товаров, доставленных по документам на покупку, по которым еще не выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="e15ad-129">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  
3. <span data-ttu-id="e15ad-130">Выберите одно из этих полей, чтобы открыть окно **Строки покупки**, в котором можно просмотреть сведения о соответствующих строках документов на покупку, включая информацию о полученных товарах или услугах.</span><span class="sxs-lookup"><span data-stu-id="e15ad-130">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="e15ad-131">Учет связанных с работой расходов</span><span class="sxs-lookup"><span data-stu-id="e15ad-131">To post a job-related expense</span></span>
<span data-ttu-id="e15ad-132">Если были произведены дополнительные или разовые расходы по работе, можно использовать окно **Журнал ГК работы**, чтобы учесть их непосредственно на соответствующем счете работы.</span><span class="sxs-lookup"><span data-stu-id="e15ad-132">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="e15ad-133">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы ГК работ**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e15ad-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e15ad-134">Создайте новую строку и введите информацию о расходах, включая информацию в полях **Код работы**</span><span class="sxs-lookup"><span data-stu-id="e15ad-134">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="e15ad-135">и **Номер рабочего задания**.</span><span class="sxs-lookup"><span data-stu-id="e15ad-135">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="e15ad-136">Когда журнал будет готов, выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="e15ad-136">When the journal is complete, choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="e15ad-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e15ad-137">See Also</span></span>
[<span data-ttu-id="e15ad-138">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="e15ad-138">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="e15ad-139">Финансы</span><span class="sxs-lookup"><span data-stu-id="e15ad-139">Finance</span></span>](finance.md)  
<span data-ttu-id="e15ad-140">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="e15ad-140">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="e15ad-141">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="e15ad-141">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="e15ad-142">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e15ad-142">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
