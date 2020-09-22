---
title: Управление банковскими счетами | Документация Майкрософт
description: Вы должны регулярно выверять операции банковских книг с соответствующими банковскими транзакциями на банковских счетах.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reconcile
ms.date: 06/22/2020
ms.author: edupont
ms.openlocfilehash: 7d7ca565218f45a753abd7e468e201538d0e6841
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3786525"
---
# <a name="reconciling-bank-accounts"></a><span data-ttu-id="37c4f-103">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="37c4f-103">Reconciling Bank Accounts</span></span>

<span data-ttu-id="37c4f-104">Банковская выверка должна проводиться через равные промежутки времени для всех ваших банковских счетов, чтобы обеспечить правильность кассовых записей компании.</span><span class="sxs-lookup"><span data-stu-id="37c4f-104">A bank reconciliation should be completed at regular intervals for all your bank accounts to ensure that the company's cash records are correct.</span></span> <span data-ttu-id="37c4f-105">Для этого вы сравниваете и сопоставляете записи на своих внутренних банковских счетах с банковскими операциями в вашем банке, а затем учитываете сальдо на своих внутренних банковских счетах, чтобы итоги были доступны финансовым менеджерам.</span><span class="sxs-lookup"><span data-stu-id="37c4f-105">You do this by comparing and matching entries in your internal bank accounts with bank transactions at your bank, and then posting the balances to your internal bank accounts to make totals available to finance managers.</span></span> <span data-ttu-id="37c4f-106">Банковская выверка также является практическим способом выявления и устранения недостающих платежей и ошибок в бухгалтерском учете.</span><span class="sxs-lookup"><span data-stu-id="37c4f-106">Bank reconciliation is also a practical way to discover and resolve missing payments and bookkeeping errors.</span></span>

<span data-ttu-id="37c4f-107">Задачу можно выполнить на странице **Выверка банковского счета**, где производится сопоставление (сверка) строк банковской выписки в левой области с вашими внутренними операциями книги банковских счетов в правой области.</span><span class="sxs-lookup"><span data-stu-id="37c4f-107">You can perform the task on the **Bank Acc. Reconciliation** page where you match (reconcile) bank statement lines in the left-hand pane with your internal bank account ledger entries in the right-hand pane.</span></span> <span data-ttu-id="37c4f-108">Кроме того, эту задачу можно выполнить на странице **Журнал выверки платежей** в рамках обработки платежей, представленных в банковской выписке.</span><span class="sxs-lookup"><span data-stu-id="37c4f-108">Alternatively, you can perform this task on the **Payment Reconciliation Journal** page as part of processing the payments that are represented on a bank statement.</span></span> <span data-ttu-id="37c4f-109">На обеих страницах информацию банковской выписки можно ввести путем импорта файла или потока, а также можно использовать автоматические предложения по сопоставлению.</span><span class="sxs-lookup"><span data-stu-id="37c4f-109">On both pages, you can fill in the bank statement information by importing a file or feed and you can use automatic matching suggestions.</span></span>

> [!NOTE]  
> <span data-ttu-id="37c4f-110">В версиях для Северной Америки выполнить банковскую выверку также можно на странице **Журнал банковской выверки**, которая лучше подходит для работы с платежными документами и депозитами, но на которой не предусмотрена возможность импорта файлов банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="37c4f-110">In the North American versions, you can also perform bank reconciliation on the **Bank Rec. Worksheet** page, which is better suited for checks and deposits but does not offer import of bank statement files.</span></span> <span data-ttu-id="37c4f-111">Чтобы использовать эту страницу вместо страницы **Выверка банковского счета**, снимите флажок **Банковская выверка с автосопоставлением** на странице **Настройка ГК**.</span><span class="sxs-lookup"><span data-stu-id="37c4f-111">To use this page instead of the **Bank Acc. Reconciliation** page, deselect the **Bank Recon. with Auto. Match** field on the **General Ledger Setup** page.</span></span> <span data-ttu-id="37c4f-112">Дополнительные сведения см. в [Выверка банковских счетов](LocalFunctionality/UnitedStates/how-to-reconcile-bank-accounts.md) в "Локальная функциональность в США".</span><span class="sxs-lookup"><span data-stu-id="37c4f-112">For more information, see [Reconcile Bank Accounts](LocalFunctionality/UnitedStates/how-to-reconcile-bank-accounts.md) under United States Local Functionality.</span></span>

<span data-ttu-id="37c4f-113">Прежде чем управлять банковскими счетами в [!INCLUDE[d365fin](includes/d365fin_md.md)], следует настроить каждый банковский счет в качестве карточки банковского счета.</span><span class="sxs-lookup"><span data-stu-id="37c4f-113">Before you can manage your bank accounts within [!INCLUDE[d365fin](includes/d365fin_md.md)], you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="37c4f-114">Кроме того, необходимо настроить электронные службы, которые можно использовать для импорта банковских выписок и экспорта файлов платежей.</span><span class="sxs-lookup"><span data-stu-id="37c4f-114">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="37c4f-115">Дополнительные сведения см. в разделе [Настройка банковских операций](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="37c4f-115">For more information, see [Setting Up Banking](bank-setup-banking.md).</span></span>

<span data-ttu-id="37c4f-116">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="37c4f-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="37c4f-117">Задача</span><span class="sxs-lookup"><span data-stu-id="37c4f-117">To</span></span> | <span data-ttu-id="37c4f-118">Ссылка</span><span class="sxs-lookup"><span data-stu-id="37c4f-118">See</span></span> |
| --- | --- |
| <span data-ttu-id="37c4f-119">Выверка банковских счетов как отдельная задача на странице **Выверка банковского счета**.</span><span class="sxs-lookup"><span data-stu-id="37c4f-119">Reconcile bank accounts as a separate task on the **Bank Acc. Reconciliation** page.</span></span> |[<span data-ttu-id="37c4f-120">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="37c4f-120">Reconcile Bank Accounts</span></span>](bank-how-reconcile-bank-accounts-separately.md) |
| <span data-ttu-id="37c4f-121">Выверка банковских счетов в связи с обработкой платежей на странице **Журнал выверки платежей**.</span><span class="sxs-lookup"><span data-stu-id="37c4f-121">Reconcile bank accounts in connection with payment processing on the **Payment Reconciliation Journal** page.</span></span> |[<span data-ttu-id="37c4f-122">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="37c4f-122">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md) |

> [!TIP]
> <span data-ttu-id="37c4f-123">Используйте банковскую выверку, чтобы убедиться, что ваши книги обновлены, и не публикуйте выверку, пока вы не будете удовлетворены выверкой.</span><span class="sxs-lookup"><span data-stu-id="37c4f-123">Use bank reconciliation to help verify that your books are up-to-date, and do not post the reconciliation until you are satisfied with the reconciliation.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="37c4f-124">См. соответствующее обучение на странице [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="37c4f-124">See Related Training at [Microsoft Learn](/learn/paths/reconcile-bank-accounts-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="37c4f-125">См. также</span><span class="sxs-lookup"><span data-stu-id="37c4f-125">See Also</span></span>

[<span data-ttu-id="37c4f-126">Настройка банковских операций</span><span class="sxs-lookup"><span data-stu-id="37c4f-126">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="37c4f-127">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="37c4f-127">Reconcile Bank Accounts</span></span>](bank-how-reconcile-bank-accounts-separately.md)  
[<span data-ttu-id="37c4f-128">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="37c4f-128">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[<span data-ttu-id="37c4f-129">Перевод банковских средств</span><span class="sxs-lookup"><span data-stu-id="37c4f-129">Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)  
[<span data-ttu-id="37c4f-130">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="37c4f-130">Managing Receivables</span></span>](receivables-manage-receivables.md)  
[<span data-ttu-id="37c4f-131">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="37c4f-131">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="37c4f-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="37c4f-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="37c4f-133">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="37c4f-133">General Business Functionality</span></span>](ui-across-business-areas.md)
