---
title: Покупка товаров или услуг для работы и управление запасами | Документация Майкрософт
description: Описывается, как управлять запасами и закупками материалов и услуг для работ.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, material, purchase
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d6c9b1102ca54ed6445522bc2d36088d5934e1fe
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5376466"
---
# <a name="manage-job-supplies"></a><span data-ttu-id="95e5d-103">Управление запасами для работы</span><span class="sxs-lookup"><span data-stu-id="95e5d-103">Manage Job Supplies</span></span>
<span data-ttu-id="95e5d-104">Управление поставками товаров, услуг и затратами по проекту является неотъемлемым и важным аспектом выполнения любых работ.</span><span class="sxs-lookup"><span data-stu-id="95e5d-104">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="95e5d-105">Программа позволяет пользоваться имеющимися запасами или, посредством заказов на покупку или счетов покупки, купить все необходимое для выполнения работы.</span><span class="sxs-lookup"><span data-stu-id="95e5d-105">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="95e5d-106">Пусть, например, для выполнения работы по обслуживанию компьютера необходим новый диск.</span><span class="sxs-lookup"><span data-stu-id="95e5d-106">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="95e5d-107">В этом случае необходимо создать новый счет покупки нового диска и записать работу, для которой он будет использован.</span><span class="sxs-lookup"><span data-stu-id="95e5d-107">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="95e5d-108">Если в процессе покупки не требуется отдельная запись физической транзакции, то покупка может быть обработана на странице **Журнал ГК работы**.</span><span class="sxs-lookup"><span data-stu-id="95e5d-108">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed on the **Job G/L Journal** page.</span></span> <span data-ttu-id="95e5d-109">Дополнительные сведения см. в разделе [Регистрация использования для работ](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="95e5d-109">For more information, see [Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="95e5d-110">Приобретение товаров или услуг для работы</span><span class="sxs-lookup"><span data-stu-id="95e5d-110">To purchase items or services for a job</span></span>
<span data-ttu-id="95e5d-111">В следующей процедуре показан порядок использования счета покупки для приобретения товаров для работы.</span><span class="sxs-lookup"><span data-stu-id="95e5d-111">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="95e5d-112">Эти же шаги применяются при использовании заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="95e5d-112">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="95e5d-113">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95e5d-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95e5d-114">Выберите действие **Создать** и введите в поля требуемые данные.</span><span class="sxs-lookup"><span data-stu-id="95e5d-114">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="95e5d-115">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="95e5d-115">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="95e5d-116">В полях **Код работы** и **Номер рабочего задания** выберите информацию о задании, для которой требуется приобрести товары или услуги.</span><span class="sxs-lookup"><span data-stu-id="95e5d-116">In the **Job No.** and **Job Task No.** fields, select the information of the job that you want to purchase items or services for.</span></span> <span data-ttu-id="95e5d-117">Используйте инструменты персонализации, если поле не отображается.</span><span class="sxs-lookup"><span data-stu-id="95e5d-117">Use the personalization tools if a field is not visible.</span></span> <span data-ttu-id="95e5d-118">Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).</span><span class="sxs-lookup"><span data-stu-id="95e5d-118">For more information, see [Personalize Your Workspace](ui-personalization-user.md).</span></span>

    <span data-ttu-id="95e5d-119">Значение, выбранное в поле **Тип строки работы**, определяет, создается ли строка планирования во время учета потребления товара.</span><span class="sxs-lookup"><span data-stu-id="95e5d-119">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="95e5d-120">Если поле содержит значение **К оплате**, будут созданы строки планирования работы, по которым можно выставлять счет клиенту.</span><span class="sxs-lookup"><span data-stu-id="95e5d-120">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="95e5d-121">Дополнительные сведения см. в разделе [Выставление счетов за работы](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="95e5d-121">For more information, see [Invoice Jobs](projects-how-invoice-jobs.md).</span></span>
4. <span data-ttu-id="95e5d-122">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="95e5d-122">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="95e5d-123">Просмотр значения покупок для работы</span><span class="sxs-lookup"><span data-stu-id="95e5d-123">To view the value of purchases for a job</span></span>
1. <span data-ttu-id="95e5d-124">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Работы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95e5d-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="95e5d-125">Откройте соответствующую карточку работы.</span><span class="sxs-lookup"><span data-stu-id="95e5d-125">Open a relevant job card.</span></span>

    <span data-ttu-id="95e5d-126">На экспресс-вкладке **Задачи** поле **Невыполненные заказы** показывает общую сумму по невыполненным поставкам (в локальной валюте) товарно-материальных ценностей и услуг по документам на покупку для строки рабочего задания.</span><span class="sxs-lookup"><span data-stu-id="95e5d-126">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="95e5d-127">Поле **Сумма, полученная без выст. счета** показывает объем товаров, доставленных по документам на покупку, по которым еще не выставлен счет.</span><span class="sxs-lookup"><span data-stu-id="95e5d-127">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  
3. <span data-ttu-id="95e5d-128">Выберите одно из этих полей, чтобы открыть страницу **Строки покупки**, на которой можно просмотреть сведения о соответствующих строках документов на покупку, включая информацию о полученных товарах или услугах.</span><span class="sxs-lookup"><span data-stu-id="95e5d-128">Choose either of the fields to open the **Purchase Lines** page where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="95e5d-129">Учет связанных с работой расходов</span><span class="sxs-lookup"><span data-stu-id="95e5d-129">To post a job-related expense</span></span>
<span data-ttu-id="95e5d-130">Если были произведены дополнительные или разовые расходы по работе, можно использовать страницу **Журнал ГК работы**, чтобы учесть их непосредственно на соответствующем счете работы.</span><span class="sxs-lookup"><span data-stu-id="95e5d-130">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** page to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="95e5d-131">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы ГК работ**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="95e5d-131">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="95e5d-132">Создайте новую строку и введите информацию о расходах, включая информацию в полях **Код работы** и **Номер рабочего задания**.</span><span class="sxs-lookup"><span data-stu-id="95e5d-132">Create a new line and enter information about the expense, including information in the **Job No.** and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="95e5d-133">Когда журнал будет готов, выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="95e5d-133">When the journal is complete, choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="95e5d-134">См. также</span><span class="sxs-lookup"><span data-stu-id="95e5d-134">See Also</span></span>
[<span data-ttu-id="95e5d-135">Управление проектами</span><span class="sxs-lookup"><span data-stu-id="95e5d-135">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="95e5d-136">Финансы</span><span class="sxs-lookup"><span data-stu-id="95e5d-136">Finance</span></span>](finance.md)  
<span data-ttu-id="95e5d-137">[Покупки](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="95e5d-137">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="95e5d-138">[Продажи](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="95e5d-138">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="95e5d-139">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="95e5d-139">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]