---
title: Управление банковскими счетами | Microsoft Docs
description: Вы должны регулярно выверять операции банковских книг с соответствующими банковскими транзакциями на банковских счетах.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 25e1242541e98cc47e2fcc4f016a860ad08c635d
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1246960"
---
# <a name="managing-bank-accounts"></a><span data-ttu-id="532c2-103">Управление банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="532c2-103">Managing Bank Accounts</span></span>
<span data-ttu-id="532c2-104">Через равные промежутки времени вы должны выверять банковские счета в [!INCLUDE[d365fin](includes/d365fin_md.md)] с соответствующими банковскими транзакциями на счетах в вашем банке, а затем учитывать сальдо на своем банковском счете.</span><span class="sxs-lookup"><span data-stu-id="532c2-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="532c2-105">Эту задачу можно выполнить в рамках обработки платежей, представленных в банковской выписке в **Журнале выверки платежей**.</span><span class="sxs-lookup"><span data-stu-id="532c2-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="532c2-106">Кроме того, задачу можно выполнить отдельно от обработки платежей на странице **Выверка банковского счета**, где производится сопоставление (сверка) строк банковской выписки в левой области с вашими внутренними операциями книги банковских счетов в правой области.</span><span class="sxs-lookup"><span data-stu-id="532c2-106">Alternatively, you can perform the task separately from payment processing, on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="532c2-107">На обеих страницах информацию банковской выписки можно ввести путем импорта файла или потока, а также можно использоваться автоматические предложения по сопоставлению.</span><span class="sxs-lookup"><span data-stu-id="532c2-107">In both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="532c2-108">В версиях для Северной Америки выполнить банковскую выверку также можно на странице **Журнал банковской выверки**, которая лучше подходит для работы с платежными документами и депозитами, но на которой не предусмотрена возможность импорта файлов банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="532c2-108">In North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="532c2-109">Чтобы использовать эту страницу вместо страницы **Выверка банковского счета**, снимите флажок **Банковская выверка с автосопоставлением** на странице **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="532c2-109">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span></span> <span data-ttu-id="532c2-110">Дополнительные сведения см. в разделе "Выверка банковских счетов" в главе "Локальная функциональность в США".</span><span class="sxs-lookup"><span data-stu-id="532c2-110">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span></span>

<span data-ttu-id="532c2-111">Иногда необходимо переводить суммы между банковским счетом в [!INCLUDE[d365fin](includes/d365fin_md.md)] для отражения переводов в банке.</span><span class="sxs-lookup"><span data-stu-id="532c2-111">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span></span> <span data-ttu-id="532c2-112">Эта задача выполняется на странице **Финансовый журнал** разными способами в зависимости от валюты фондов.</span><span class="sxs-lookup"><span data-stu-id="532c2-112">You perform this task on the **General Journal** page, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="532c2-113">Прежде чем управлять банковскими счетами, следует настроить каждый банковский счет в качестве карточки банковского счета.</span><span class="sxs-lookup"><span data-stu-id="532c2-113">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="532c2-114">Кроме того, необходимо настроить электронные службы, которые можно использовать для импорта банковских выписок и экспорта файлов платежей.</span><span class="sxs-lookup"><span data-stu-id="532c2-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="532c2-115">Дополнительные сведения см. в разделе [Настройка банковских счетов](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="532c2-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="532c2-116">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="532c2-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="532c2-117">Действие</span><span class="sxs-lookup"><span data-stu-id="532c2-117">To</span></span> | <span data-ttu-id="532c2-118">Ссылка</span><span class="sxs-lookup"><span data-stu-id="532c2-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="532c2-119">Выверка банковских счетов в связи с обработкой платежей на странице **Журнал выверки платежей**.</span><span class="sxs-lookup"><span data-stu-id="532c2-119">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span></span> |[<span data-ttu-id="532c2-120">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="532c2-120">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="532c2-121">Выверка банковских счетов, включая операции книги платежных документов, как отдельная задача на странице **Выверка банковского счета**.</span><span class="sxs-lookup"><span data-stu-id="532c2-121">Reconcile bank accounts, including check ledger entries, as a separate task on the **Bank Acc. Reconciliation** page.</span></span> |[<span data-ttu-id="532c2-122">Выверка банковских счетов по отдельности</span><span class="sxs-lookup"><span data-stu-id="532c2-122">Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="532c2-123">Учет переводов между банковскими счетами в одной валюте или в различных валютах.</span><span class="sxs-lookup"><span data-stu-id="532c2-123">Post transfers between bank accounts in the same currency or in different currencies.</span></span> |[<span data-ttu-id="532c2-124">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="532c2-124">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a><span data-ttu-id="532c2-125">См. также</span><span class="sxs-lookup"><span data-stu-id="532c2-125">See Also</span></span>
[<span data-ttu-id="532c2-126">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="532c2-126">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="532c2-127">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="532c2-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="532c2-128">[Управление кредиторской задолженностью](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="532c2-128">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="532c2-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="532c2-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="532c2-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="532c2-130">General Business Functionality</span></span>](ui-across-business-areas.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 
