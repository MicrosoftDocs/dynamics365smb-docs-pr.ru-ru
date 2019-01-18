---
title: "Регистрация и возмещение расходов сотрудников, связанных со служебной деятельностью | Microsoft Docs"
description: "Учет расходов сотрудников в финансовом журнале на счете сотрудника и последующий учет платежа на банковский счет сотрудника для возмещения расходов, связанных со служебной деятельностью."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 11/27/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: add32e82465610830b68a979e238103bfa10d438
ms.openlocfilehash: 1042bfbd19a4779c72d4e945d6118a9d628301e8
ms.contentlocale: ru-ru
ms.lasthandoff: 11/29/2018

---
# <a name="record-and-reimburse-employees-expenses"></a><span data-ttu-id="69264-103">Регистрация и возмещение расходов сотрудников</span><span class="sxs-lookup"><span data-stu-id="69264-103">Record and Reimburse Employees' Expenses</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="69264-104">поддерживает транзакции для сотрудников аналогично тому, как это делается для поставщиков.</span><span class="sxs-lookup"><span data-stu-id="69264-104">supports transactions for employee in a similar way as for vendors.</span></span> <span data-ttu-id="69264-105">Соответственно, учетные группы сотрудников существуют, чтобы обеспечить учет операций из книги операций по сотрудникам на соответствующих счетах в главной книге.</span><span class="sxs-lookup"><span data-stu-id="69264-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span></span>

> [!NOTE]  
> <span data-ttu-id="69264-106">Транзакции сотрудникам могут учитываться только в локальной валюте.</span><span class="sxs-lookup"><span data-stu-id="69264-106">Employee transactions can be posted in the local currency only.</span></span> <span data-ttu-id="69264-107">Возмещение сотрудникам не поддерживает скидки или отклонения в оплате.</span><span class="sxs-lookup"><span data-stu-id="69264-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span></span>

<span data-ttu-id="69264-108">Если сотрудники расходуют собственные средства во время делового активности, то можно учитывать расходы на счете сотрудника.</span><span class="sxs-lookup"><span data-stu-id="69264-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span></span> <span data-ttu-id="69264-109">Затем можно возместить расходы сотруднику путем платежа на банковский счет сотрудника, аналогично выплатам поставщикам.</span><span class="sxs-lookup"><span data-stu-id="69264-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span></span>

## <a name="to-record-an-employees-expense"></a><span data-ttu-id="69264-110">Запись расходов сотрудника</span><span class="sxs-lookup"><span data-stu-id="69264-110">To record an employee's expense</span></span>
<span data-ttu-id="69264-111">Расходы сотрудников учитываются на странице **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="69264-111">You post employees' expenses on the **General Journal** page.</span></span>
1. <span data-ttu-id="69264-112">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые журналы**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="69264-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="69264-113">Откройте соответствующий раздел финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="69264-113">Open the relevant general journal batch.</span></span> <span data-ttu-id="69264-114">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="69264-114">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="69264-115">На новой строке журнала заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="69264-115">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]    

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="69264-116">Повторите шаг 3 для всех затрат, понесенных сотрудником.</span><span class="sxs-lookup"><span data-stu-id="69264-116">Repeat step 3 for all the expenses that the employee has incurred.</span></span>

    > [!TIP]  
    > <span data-ttu-id="69264-117">Если необходимо ввести несколько строк расходов над одной строкой балансирующего счета, например, для банковского счета сотрудника, установите флажок **Предлагаемая балансирующая сумма** в строке раздела на странице **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="69264-117">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="69264-118">Затем в поле **Сумма** строки балансирующего счета автоматически будет подставлено значение, необходимое для балансировки расходов.</span><span class="sxs-lookup"><span data-stu-id="69264-118">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span></span>
5. <span data-ttu-id="69264-119">Выберите действие **Учет** для регистрации расходов на счете сотрудника.</span><span class="sxs-lookup"><span data-stu-id="69264-119">Choose the **Post** action to record the expenses on the employee's account.</span></span>

## <a name="to-reimburse-an-employee"></a><span data-ttu-id="69264-120">Для возмещения расходов сотруднику</span><span class="sxs-lookup"><span data-stu-id="69264-120">To reimburse an employee</span></span>
<span data-ttu-id="69264-121">Возмещение расходов сотрудникам производится путем учета платежей на их банковские счета на странице **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="69264-121">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span></span>
1. <span data-ttu-id="69264-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы платежей**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="69264-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="69264-123">Откройте соответствующий раздел журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="69264-123">Open the relevant payment journal batch.</span></span> <span data-ttu-id="69264-124">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="69264-124">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="69264-125">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="69264-125">Fill in the fields as necessary.</span></span> <span data-ttu-id="69264-126">Дополнительные сведения см. в разделе [Осуществление платежей](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="69264-126">For more information, see [Making Payments](payables-make-payments.md).</span></span>
4. <span data-ttu-id="69264-127">Можно также выбрать действие **Предложить оплату сотрудников**, чтобы автоматически вставлять строки журнала для ожидающих выплат для возмещения расходов сотрудников.</span><span class="sxs-lookup"><span data-stu-id="69264-127">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span></span>
5. <span data-ttu-id="69264-128">Выберите действие **Учесть** для регистрации возмещения.</span><span class="sxs-lookup"><span data-stu-id="69264-128">Choose the **Post** action to register the reimbursement.</span></span>  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a><span data-ttu-id="69264-129">Для выверки выплат возмещения расходов с книгой операций по сотрудникам</span><span class="sxs-lookup"><span data-stu-id="69264-129">To reconcile reimbursements with employee ledger entries</span></span>
<span data-ttu-id="69264-130">Выплаты сотруднику применяются к соответствующим открытым операциям книги сотрудников таким же образом, как для платежей поставщикам, например на странице **Журнал выверки платежей**, на основе соответствующих операций банковской выписки.</span><span class="sxs-lookup"><span data-stu-id="69264-130">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span></span> <span data-ttu-id="69264-131">Дополнительные сведения см. в разделе [Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="69264-131">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span> <span data-ttu-id="69264-132">Можно также применить вручную на странице **Книга операций по сотрудникам**.</span><span class="sxs-lookup"><span data-stu-id="69264-132">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span></span> <span data-ttu-id="69264-133">Дополнительные сведения см. в разделе [Выверка платежей поставщикам вручную](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="69264-133">For more information, see the related [Reconcile Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="69264-134">См. также</span><span class="sxs-lookup"><span data-stu-id="69264-134">See Also</span></span>
<span data-ttu-id="69264-135">[Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="69264-135">[Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md)</span></span>  
[<span data-ttu-id="69264-136">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="69264-136">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="69264-137">Сторнирование учета</span><span class="sxs-lookup"><span data-stu-id="69264-137">Reverse Postings</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="69264-138">Финансы</span><span class="sxs-lookup"><span data-stu-id="69264-138">Finance</span></span>](finance.md)  
<span data-ttu-id="69264-139">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="69264-139">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

