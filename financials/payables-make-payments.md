---
title: "Обзор задач управления платежами поставщикам | Документы Майкрософт"
description: "Описываются задачи по управлению платежами поставщикам или кредиторам, включая учет строк платежей и получение обзора сумм к оплате."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, vendor payment, creditor, debt, balance due, AP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: d0b9020596484a8910db2f5720adfe159ad96fe7
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="make-payments"></a><span data-ttu-id="8b3eb-103">Создание платежей</span><span class="sxs-lookup"><span data-stu-id="8b3eb-103">Make Payments</span></span>
<span data-ttu-id="8b3eb-104">При учете выполнении платежей поставщикам вы учитываете соответствующие строки платежей в окне **Журнал платежей**.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-104">When you make payments to vendors, you post the related payment lines in the **Payment Journal** window.</span></span> <span data-ttu-id="8b3eb-105">С помощью функции **Предлож. оплаты поставщикам** вы можете находить платежей, подлежащие выполнению.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-105">You can use the **Suggest Vendor Payments** function to find payments that are due.</span></span> <span data-ttu-id="8b3eb-106">Для просмотра таких платежей можно также использовать отчет **Поставщик - сводка задолженности с распределением по срокам**.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-106">You can also use the **Vendor - Summary Aging** report to get an overview of due payments.</span></span>

<span data-ttu-id="8b3eb-107">Из журнала платежей можно распечатывать электронные платежные документы или записывать, когда платежные документы были выписаны.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-107">From the payment journal, you can print computer checks or record when checks are written.</span></span> <span data-ttu-id="8b3eb-108">Если в поле **Тип банковского платежа** выбрано значение **Компьютерный**, то все строки, представляющие платежные документы, должны печататься до учета строк журнала платежей.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-108">If you select **Computer Check** in the **Bank Payment Type** field, then any lines representing checks must be printed before the payment journal can be posted.</span></span>

<span data-ttu-id="8b3eb-109">При учете платежей вы можете экспортировать их в банковский файл для загрузки в банк в целях обработки.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-109">When the payments are posted, you can export them to a bank file for upload to your bank for processing.</span></span>

<span data-ttu-id="8b3eb-110">После выполнения всех платежей в банке их необходимо применить к соответствующим открытым операциям книги поставщиков.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-110">After the payments are made at your bank, you must apply them to their related open vendor ledger entries.</span></span> <span data-ttu-id="8b3eb-111">Это можно сделать вручную или путем импорта файла банковской выписки и применения платежей автоматически.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-111">You can do this manually or by importing a bank statement file and applying the payments automatically.</span></span> <span data-ttu-id="8b3eb-112">Дополнительные сведения см. в разделе [Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="8b3eb-112">For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span>

<span data-ttu-id="8b3eb-113">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-113">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

| <span data-ttu-id="8b3eb-114">Действие</span><span class="sxs-lookup"><span data-stu-id="8b3eb-114">To</span></span> | <span data-ttu-id="8b3eb-115">Ссылка</span><span class="sxs-lookup"><span data-stu-id="8b3eb-115">See</span></span> |
| --- | --- |
| <span data-ttu-id="8b3eb-116">Используйте функцию для предложения оплат поставщикам в соответствии с выбранными критериями, такими как срок оплаты, доступность скидки и ваша ликвидность.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-116">Use a function to suggest vendor payments according to selected criteria, such as due date, discount eligibility, and your liquidity.</span></span> |[<span data-ttu-id="8b3eb-117">Практическое руководство. Предложение оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="8b3eb-117">How to: Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md) |
| <span data-ttu-id="8b3eb-118">Выписывайте чеки по платежам, в печатном виде или в электронном виде.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-118">Issue checks for payments, either as print-outs or as computer checks.</span></span> <span data-ttu-id="8b3eb-119">Аннулируйте чеки перед учетом или после него.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-119">Void checks before or after posting.</span></span> |[<span data-ttu-id="8b3eb-120">Практическое руководство. Работа с платежными документами</span><span class="sxs-lookup"><span data-stu-id="8b3eb-120">How to: Work with Checks</span></span>](payables-how-work-checks.md) |
| <span data-ttu-id="8b3eb-121">Убедитесь, что банк выполняет клиринг только проверенных платежных документов и сумм, отправив ему файл, содержащий сведения о поставщике, платежном документе и платеже.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-121">Make sure that your bank only clears validated checks and amounts by sending them a file that contains vendor, check, and payment information.</span></span> |[<span data-ttu-id="8b3eb-122">Практическое руководство. Экспорт файла Positive Pay</span><span class="sxs-lookup"><span data-stu-id="8b3eb-122">How to: Export a Positive Pay file</span></span>](finance-how-positive-pay.md) |
|<span data-ttu-id="8b3eb-123">Экспортируйте платежи из окна **Журнал платежей** в банковский файл, отправленный в банк для обработки, включая EFT (электронный платеж) в Северной Америке.</span><span class="sxs-lookup"><span data-stu-id="8b3eb-123">Export payments from the **Payment Journal** window to a bank file that you upload to your bank for processing, including EFT (electronic funds transfer) in North America.</span></span> |[<span data-ttu-id="8b3eb-124">Практическое руководство. Экспорт платежей в банковский файл</span><span class="sxs-lookup"><span data-stu-id="8b3eb-124">How to: Export Payments to a Bank File</span></span>](payables-how-export-payments-bank-file.md)|  

## <a name="see-also"></a><span data-ttu-id="8b3eb-125">См. также</span><span class="sxs-lookup"><span data-stu-id="8b3eb-125">See Also</span></span>
[<span data-ttu-id="8b3eb-126">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="8b3eb-126">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="8b3eb-127">Покупки</span><span class="sxs-lookup"><span data-stu-id="8b3eb-127">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="8b3eb-128">Управление дебиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="8b3eb-128">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="8b3eb-129">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8b3eb-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

