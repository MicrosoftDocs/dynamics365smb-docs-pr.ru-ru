---
title: Выверка платежей с использованием расширения Envestnet Yodlee Bank Feeds | Документация Майкрософт
description: Описание расширения Envestnet Yodlee Bank Feeds, которое устанавливает связь с банковскими счетами для быстрой выверки банковских платежей.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: d79ef7c076ec3a529aeb0c679b8b61658ef65af5
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2315352"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="aea5d-103">Расширение Envestnet Yodlee Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="aea5d-103">The Envestnet Yodlee Bank Feeds Extension</span></span>
<span data-ttu-id="aea5d-104">Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке.</span><span class="sxs-lookup"><span data-stu-id="aea5d-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="aea5d-105">Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.</span><span class="sxs-lookup"><span data-stu-id="aea5d-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

<span data-ttu-id="aea5d-106">Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.</span><span class="sxs-lookup"><span data-stu-id="aea5d-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>

> [!NOTE]
> <span data-ttu-id="aea5d-107">Эта функция поддерживается только в сетевой версии Business Central.</span><span class="sxs-lookup"><span data-stu-id="aea5d-107">This functionality is only supported in the online version of Business Central.</span></span> <span data-ttu-id="aea5d-108">Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="aea5d-108">To use this functionality on-premise, you must obtain a cobrand account from Envestnet Yodlee.</span></span><br /><br />

> [!IMPORTANT]
> <span data-ttu-id="aea5d-109">Из-за новой Директивы об оказании платежных услуг (PSD2), вступившей в силу в Европе, после 14 сентября 2019 г. вы больше не сможете автоматически импортировать банковские выписки из банков Соединенного королевства в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="aea5d-109">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="aea5d-110">Мы изучаем возможности снова сделать эту функцию доступной в будущем.</span><span class="sxs-lookup"><span data-stu-id="aea5d-110">We are looking into the possibility of offering this feature again in the future.</span></span>

<span data-ttu-id="aea5d-111">Служба Envestnet Yodlee Bank Feeds предоставляет следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="aea5d-111">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="aea5d-112">Нет необходимости вводить данные вручную.</span><span class="sxs-lookup"><span data-stu-id="aea5d-112">Removes the need for manual entry.</span></span>
* <span data-ttu-id="aea5d-113">Улучшает эффективность и точность выверки платежей.</span><span class="sxs-lookup"><span data-stu-id="aea5d-113">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="aea5d-114">Поддерживает большое количество банков.</span><span class="sxs-lookup"><span data-stu-id="aea5d-114">Supports a large number of banks.</span></span>
* <span data-ttu-id="aea5d-115">Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="aea5d-115">Allows up-to-date information about bank transactions from within [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
* <span data-ttu-id="aea5d-116">Поддерживает ручной и автоматический ввод данных из банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="aea5d-116">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="aea5d-117">Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.</span><span class="sxs-lookup"><span data-stu-id="aea5d-117">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

<span data-ttu-id="aea5d-118">Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="aea5d-118">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="aea5d-119">См. также</span><span class="sxs-lookup"><span data-stu-id="aea5d-119">See Also</span></span>
<span data-ttu-id="aea5d-120">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="aea5d-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="aea5d-121">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="aea5d-121">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="aea5d-122">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="aea5d-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
