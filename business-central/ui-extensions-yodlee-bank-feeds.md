---
title: Выверка платежей с помощью расширения Envestnet Yodlee Bank Feeds | Microsoft Docs
description: Описывает расширение Envestnet Yodlee Bank Feeds, которое устанавливает связь с банковскими счетами для быстрой выверки банковских платежей.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: 53ee8bb7ee798c473e1053ea8413be28f9185d1b
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1248207"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="75e40-103">Расширение Envestnet Yodlee Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="75e40-103">The Envestnet Yodlee Bank Feeds Extension</span></span>
<span data-ttu-id="75e40-104">Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке.</span><span class="sxs-lookup"><span data-stu-id="75e40-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="75e40-105">Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.</span><span class="sxs-lookup"><span data-stu-id="75e40-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

> [!NOTE]
> <span data-ttu-id="75e40-106">Эта функция поддерживается только в сетевой версии Business Central.</span><span class="sxs-lookup"><span data-stu-id="75e40-106">This functionality is only supported in the online version of Business Central.</span></span> <span data-ttu-id="75e40-107">Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="75e40-107">To use this functionality on-premise, you must obtain a cobrand account from Envestnet Yodlee.</span></span>

<span data-ttu-id="75e40-108">Служба Envestnet Yodlee Bank Feeds обеспечивает следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="75e40-108">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="75e40-109">Нет необходимости вводить данные вручную.</span><span class="sxs-lookup"><span data-stu-id="75e40-109">Removes the need for manual entry.</span></span>
* <span data-ttu-id="75e40-110">Улучшает эффективность и точность выверки платежей.</span><span class="sxs-lookup"><span data-stu-id="75e40-110">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="75e40-111">Поддерживает большое количество банков.</span><span class="sxs-lookup"><span data-stu-id="75e40-111">Supports a large number of banks.</span></span>
* <span data-ttu-id="75e40-112">Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="75e40-112">Allows up-to-date information about bank transactions from within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
* <span data-ttu-id="75e40-113">Поддерживает ручной и автоматический ввод данных из банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="75e40-113">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="75e40-114">Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.</span><span class="sxs-lookup"><span data-stu-id="75e40-114">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

<span data-ttu-id="75e40-115">Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="75e40-115">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="75e40-116">См. также</span><span class="sxs-lookup"><span data-stu-id="75e40-116">See Also</span></span>
<span data-ttu-id="75e40-117">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="75e40-117">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="75e40-118">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="75e40-118">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="75e40-119">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="75e40-119">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
