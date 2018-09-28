---
title: "Управление банковскими счетами | Microsoft Docs"
description: "Вы должны регулярно выверять операции банковских книг с соответствующими банковскими транзакциями на банковских счетах."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: f3733c3ec0048171294aae51dcfac0c2ecdc9e72
ms.contentlocale: ru-ru
ms.lasthandoff: 09/28/2018

---
# <a name="managing-bank-accounts"></a><span data-ttu-id="07521-103">Управление банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="07521-103">Managing Bank Accounts</span></span>
<span data-ttu-id="07521-104">Через равные промежутки времени вы должны выверять банковские счета в [!INCLUDE[d365fin](includes/d365fin_md.md)] с соответствующими банковскими транзакциями на счетах в вашем банке, а затем учитывать сальдо на своем банковском счете.</span><span class="sxs-lookup"><span data-stu-id="07521-104">At regular intervals, you must reconcile your bank ledger entries in [!INCLUDE[d365fin](includes/d365fin_md.md)] with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="07521-105">Эту задачу можно выполнить в рамках обработки платежей, представленных в банковской выписке в **Журнале выверки платежей**.</span><span class="sxs-lookup"><span data-stu-id="07521-105">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="07521-106">Кроме того, задачу можно выполнить отдельно от обработки платежей в окне **Выверка банковского счета**, где производится сопоставление (сверка) строк банковской выписки в левой области с вашими внутренними операциями книги банковских счетов в правой области.</span><span class="sxs-lookup"><span data-stu-id="07521-106">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="07521-107">В обоих окнах информацию банковской выписки можно ввести путем импорта файла или потока, а также можно использоваться автоматические предложения по сопоставлению.</span><span class="sxs-lookup"><span data-stu-id="07521-107">In both windows, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="07521-108">В версиях для Северной Америки выполнить банковскую выверку также можно в окне **Журнал банковской выверки**, которое лучше подходит для работы с платежными документами и депозитами, но в котором не предусмотрена возможность импорта файлов банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="07521-108">In North American versions, you can also perform bank reconciliation in the **Bank Rec. Worksheet** window, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="07521-109">Чтобы использовать это окно вместо окна **Выверка банковского счета**, снимите флажок **Банковская выверка с автосопоставлением** в окне **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="07521-109">To use this window instead of the **Bank Acc. Reconciliation** window, deselect the **Bank Recon. with Auto. Match** field in the **General Ledger Setup** window.</span></span> <span data-ttu-id="07521-110">Дополнительные сведения см. в разделе "Выверка банковских счетов" в главе "Локальная функциональность в США".</span><span class="sxs-lookup"><span data-stu-id="07521-110">For more information, see the "Reconcile Bank Accounts" section under United States Local Functionality.</span></span>

<span data-ttu-id="07521-111">Иногда необходимо переводить суммы между банковским счетом в [!INCLUDE[d365fin](includes/d365fin_md.md)] для отражения переводов в банке.</span><span class="sxs-lookup"><span data-stu-id="07521-111">Sometimes, you need to transfer amounts between bank account in [!INCLUDE[d365fin](includes/d365fin_md.md)] to reflect transfers at your bank.</span></span> <span data-ttu-id="07521-112">Эта задача выполняется в окне **Финансовый журнал** разными способами в зависимости от валюты фондов.</span><span class="sxs-lookup"><span data-stu-id="07521-112">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="07521-113">Прежде чем управлять банковскими счетами, следует настроить каждый банковский счет в качестве карточки банковского счета.</span><span class="sxs-lookup"><span data-stu-id="07521-113">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="07521-114">Кроме того, необходимо настроить электронные службы, которые можно использовать для импорта банковских выписок и экспорта файлов платежей.</span><span class="sxs-lookup"><span data-stu-id="07521-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="07521-115">Дополнительные сведения см. в разделе [Настройка банковских счетов](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="07521-115">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="07521-116">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="07521-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="07521-117">Действие</span><span class="sxs-lookup"><span data-stu-id="07521-117">To</span></span> | <span data-ttu-id="07521-118">Ссылка</span><span class="sxs-lookup"><span data-stu-id="07521-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="07521-119">Выверка банковских счетов в связи с обработкой платежей в окне **Журнал выверки платежей**.</span><span class="sxs-lookup"><span data-stu-id="07521-119">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span> |[<span data-ttu-id="07521-120">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="07521-120">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| <span data-ttu-id="07521-121">Выверка банковских счетов, включая операции книги платежных документов, как отдельная задача в окне **Выверка банковского счета**.</span><span class="sxs-lookup"><span data-stu-id="07521-121">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span> |[<span data-ttu-id="07521-122">Выверка банковских счетов по отдельности</span><span class="sxs-lookup"><span data-stu-id="07521-122">Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="07521-123">Учет переводов между банковскими счетами в одной валюте или в различных валютах.</span><span class="sxs-lookup"><span data-stu-id="07521-123">Post transfers between bank accounts in the same currency or in different currencies.</span></span> |[<span data-ttu-id="07521-124">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="07521-124">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md) |

## <a name="see-also"></a><span data-ttu-id="07521-125">См. также</span><span class="sxs-lookup"><span data-stu-id="07521-125">See Also</span></span>
[<span data-ttu-id="07521-126">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="07521-126">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="07521-127">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="07521-127">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="07521-128">[Управление кредиторской задолженностью](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="07521-128">[Managing Payables](payables-manage-payables.md)  </span></span>  
<span data-ttu-id="07521-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="07521-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="07521-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="07521-130">General Business Functionality</span></span>](ui-across-business-areas.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
 

