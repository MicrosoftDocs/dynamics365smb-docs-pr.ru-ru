---
title: Регистрация и возмещение расходов сотрудников, связанных со служебной деятельностью
description: Учет расходов сотрудников в финансовом журнале на счете сотрудника и последующий учет платежа на банковский счет сотрудника для возмещения расходов, связанных со служебной деятельностью.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: dd4ce755e3414f19ae501c1d437f3e1d78d565a1
ms.sourcegitcommit: 1aab52477956bf1aa7376fc7fb984644bc398c61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "6184403"
---
# <a name="record-and-reimburse-employees-expenses"></a><span data-ttu-id="7b6dc-103">Регистрация и возмещение расходов сотрудников</span><span class="sxs-lookup"><span data-stu-id="7b6dc-103">Record and Reimburse Employees' Expenses</span></span>

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="7b6dc-104">поддерживает транзакции для сотрудников аналогично тому, как это делается для поставщиков.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-104">supports transactions for employees in a similar way as for vendors.</span></span> <span data-ttu-id="7b6dc-105">Соответственно, учетные группы сотрудников существуют, чтобы обеспечить учет операций из книги операций по сотрудникам на соответствующих счетах в главной книге.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-105">Accordingly, employee posting groups exist to make sure that employee ledger entries are posted to the relevant accounts in the general ledger.</span></span>

> [!NOTE]  
> <span data-ttu-id="7b6dc-106">Транзакции сотрудникам могут учитываться только в локальной валюте.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-106">Employee transactions can be posted in the local currency only.</span></span> <span data-ttu-id="7b6dc-107">Возмещение сотрудникам не поддерживает скидки или отклонения в оплате.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-107">Reimbursement payments to employees do not support discounts and payment tolerances.</span></span>

<span data-ttu-id="7b6dc-108">Если сотрудники расходуют собственные средства во время делового активности, то можно учитывать расходы на счете сотрудника.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-108">If employees spend their own money during business activities, you can post the expense to the employee's account.</span></span> <span data-ttu-id="7b6dc-109">Затем можно возместить расходы сотруднику путем платежа на банковский счет сотрудника, аналогично выплатам поставщикам.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-109">Then you can reimburse the employee by making a payment to the employee's bank account, similarly to how you pay vendors.</span></span>  

> [!TIP]
> <span data-ttu-id="7b6dc-110">В этой статье объясняется, как записать расходы в книгах и как возместить затраты работнику.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-110">This article explains how to record the expense in the books and how to reimburse the employee.</span></span> <span data-ttu-id="7b6dc-111">В вашей организации может быть портал или приложение, где сотрудники могут отправлять свои отчеты о расходах.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-111">Your organization may have a portal or app where employees can submit their expense reports.</span></span>

<span data-ttu-id="7b6dc-112">[!INCLUDE [prod_short](includes/prod_short.md)] достаточно гибок, чтобы соответствовать многим различным ситуациям.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-112">[!INCLUDE [prod_short](includes/prod_short.md)] is flexible enough to suit many different practices.</span></span> <span data-ttu-id="7b6dc-113">Точные номера счетов для использования зависят от конфигурации и процессов вашей организации.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-113">The exact account numbers to use depends on your organization's configuration and processes.</span></span>  

## <a name="to-record-an-employees-expense"></a><span data-ttu-id="7b6dc-114">Запись расходов сотрудника</span><span class="sxs-lookup"><span data-stu-id="7b6dc-114">To record an employee's expense</span></span>

<span data-ttu-id="7b6dc-115">Расходы сотрудников учитываются на странице **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-115">You post employees' expenses on the **General Journal** page.</span></span>

1. <span data-ttu-id="7b6dc-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые журналы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="7b6dc-117">Откройте соответствующий раздел финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-117">Open the relevant general journal batch.</span></span> <span data-ttu-id="7b6dc-118">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="7b6dc-118">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="7b6dc-119">На новой строке журнала заполните поля, как требуется.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-119">On a new journal line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    > [!NOTE]
    > [!INCLUDE[journal-showhide-columns-inline-tip](includes/journal-showhide-columns-inline-tip.md)]
4. <span data-ttu-id="7b6dc-120">Повторите шаг 3 для всех затрат, понесенных сотрудником.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-120">Repeat step 3 for all the expenses that the employee has incurred.</span></span>

    > [!TIP]  
    > <span data-ttu-id="7b6dc-121">Если необходимо ввести несколько строк расходов над одной строкой балансирующего счета, например, для банковского счета сотрудника, установите флажок **Предлагаемая балансирующая сумма** в строке раздела на странице **Разделы финансового журнала**.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-121">If you want to enter multiple expense lines above one balance-account line for the employee's bank account, then select the **Suggest Balancing Amount** check box on the line for your batch on the **General Journal Batches** page.</span></span> <span data-ttu-id="7b6dc-122">Затем в поле **Сумма** строки балансирующего счета автоматически будет подставлено значение, необходимое для балансировки расходов.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-122">Then the **Amount** field on the balance-account line is automatically prefilled with the value that is required to balance the expenses.</span></span>
5. <span data-ttu-id="7b6dc-123">Выберите действие **Учет** для регистрации расходов на счете сотрудника.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-123">Choose the **Post** action to record the expenses on the employee's account.</span></span>

## <a name="to-reimburse-an-employee"></a><span data-ttu-id="7b6dc-124">Для возмещения расходов сотруднику</span><span class="sxs-lookup"><span data-stu-id="7b6dc-124">To reimburse an employee</span></span>

<span data-ttu-id="7b6dc-125">Возмещение расходов сотрудникам производится путем учета платежей на их банковские счета на странице **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-125">You reimburse employees by posting payments to their bank account on the **Payment Journal** page.</span></span>  

1. <span data-ttu-id="7b6dc-126">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журналы платежей**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-126">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="7b6dc-127">Откройте соответствующий раздел журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-127">Open the relevant payment journal batch.</span></span> <span data-ttu-id="7b6dc-128">Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="7b6dc-128">For more information, see [Working with General Journals](ui-work-general-journals.md).</span></span>
3. <span data-ttu-id="7b6dc-129">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-129">Fill in the fields as necessary.</span></span> <span data-ttu-id="7b6dc-130">Дополнительные сведения см. в разделе [Осуществление платежей](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="7b6dc-130">For more information, see [Making Payments](payables-make-payments.md).</span></span>
4. <span data-ttu-id="7b6dc-131">Можно также выбрать действие **Предложить оплату сотрудников**, чтобы автоматически вставлять строки журнала для ожидающих выплат для возмещения расходов сотрудников.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-131">Alternatively, choose the **Suggest Employee Payment** action to automatically insert journal lines for pending employee reimbursements.</span></span>
5. <span data-ttu-id="7b6dc-132">Выберите действие **Учесть** для регистрации возмещения.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-132">Choose the **Post** action to register the reimbursement.</span></span>  

## <a name="to-reconcile-reimbursements-with-employee-ledger-entries"></a><span data-ttu-id="7b6dc-133">Для выверки выплат возмещения расходов с книгой операций по сотрудникам</span><span class="sxs-lookup"><span data-stu-id="7b6dc-133">To reconcile reimbursements with employee ledger entries</span></span>

<span data-ttu-id="7b6dc-134">Выплаты сотруднику применяются к соответствующим открытым операциям книги сотрудников таким же образом, как для платежей поставщикам, например на странице **Журнал выверки платежей**, на основе соответствующих операций банковской выписки.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-134">You apply employee payments to their related open employee ledger entries in the same way as you do for vendor payments, for example on the **Payment Reconciliation Journal** page, based on the related bank statement entries.</span></span> <span data-ttu-id="7b6dc-135">Дополнительные сведения см. в разделе [Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="7b6dc-135">For more information, see [Applying Payments Automatically and Reconciling Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span> <span data-ttu-id="7b6dc-136">Можно также применить вручную на странице **Книга операций по сотрудникам**.</span><span class="sxs-lookup"><span data-stu-id="7b6dc-136">Alternatively, you can apply manually on the **Employee Ledger Entries** page.</span></span> <span data-ttu-id="7b6dc-137">Дополнительные сведения см. в разделе [Выверка платежей поставщикам с журналом платежей или из книги операций по поставщикам](payables-how-apply-purchase-transactions-manually.md).</span><span class="sxs-lookup"><span data-stu-id="7b6dc-137">For more information, see the related [Reconcile Vendor Payments with the Payment Journal or from Vendor Ledger Entries](payables-how-apply-purchase-transactions-manually.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="7b6dc-138">См. также</span><span class="sxs-lookup"><span data-stu-id="7b6dc-138">See Also</span></span>

[<span data-ttu-id="7b6dc-139">Учет транзакций непосредственно в главной книге</span><span class="sxs-lookup"><span data-stu-id="7b6dc-139">Post Transactions Directly to the General Ledger</span></span>](finance-how-post-transactions-directly.md)  
[<span data-ttu-id="7b6dc-140">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="7b6dc-140">Working with General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="7b6dc-141">Сторнирование учета в журнале и отмена приходных/расходных накладных</span><span class="sxs-lookup"><span data-stu-id="7b6dc-141">Reverse Journal Postings and Undo Receipts/Shipments</span></span>](finance-how-reverse-journal-posting.md)  
[<span data-ttu-id="7b6dc-142">Финансы</span><span class="sxs-lookup"><span data-stu-id="7b6dc-142">Finance</span></span>](finance.md)  
<span data-ttu-id="7b6dc-143">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7b6dc-143">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]