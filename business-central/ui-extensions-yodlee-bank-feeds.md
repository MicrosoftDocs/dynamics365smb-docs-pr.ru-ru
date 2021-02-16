---
title: Выверка платежей с использованием расширения Envestnet Yodlee Bank Feeds
description: Описание расширения Envestnet Yodlee Bank Feeds, которое устанавливает связь с банковскими счетами для быстрой выверки банковских платежей.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d8a04218e44c4a40d96f5e84677434c51f6ef5f3
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4757396"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a><span data-ttu-id="77d55-103">Расширение Envestnet Yodlee Bank Feeds</span><span class="sxs-lookup"><span data-stu-id="77d55-103">The Envestnet Yodlee Bank Feeds Extension</span></span>

<span data-ttu-id="77d55-104">Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке.</span><span class="sxs-lookup"><span data-stu-id="77d55-104">To quickly reconcile payments made to your bank accounts, the Envestnet Yodlee Bank Feeds service allows you to link your system bank account to your online bank account.</span></span> <span data-ttu-id="77d55-105">Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.</span><span class="sxs-lookup"><span data-stu-id="77d55-105">This means that the latest bank statement is automatically or manually fed into your reconciliation journal, ensuring that you are always processing the latest payments with minimal risk of errors.</span></span>

<span data-ttu-id="77d55-106">Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.</span><span class="sxs-lookup"><span data-stu-id="77d55-106">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>

> [!NOTE]
> <span data-ttu-id="77d55-107">Служба Envestnet Yodlee Bank Feeds поддерживается только в сетевой версии Business Central.</span><span class="sxs-lookup"><span data-stu-id="77d55-107">The Envestnet Yodlee Bank Feeds service is only supported in the online version of Business Central.</span></span> <span data-ttu-id="77d55-108">Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="77d55-108">To use this functionality on-premises, you must obtain a cobrand account from Envestnet Yodlee.</span></span><br /><br />
> <span data-ttu-id="77d55-109">Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.</span><span class="sxs-lookup"><span data-stu-id="77d55-109">The Envestnet Yodlee Bank Feeds service is only supported in the United States and Canada.</span></span>
> <span data-ttu-id="77d55-110">Поддерживаются только банки, расположенные в этих странах, хотя банки из других стран могут появляться в окне выбора банка Envestnet Yodlee Bank Feeds в [!INCLUDE[prod_short](includes/prod_short.md)],</span><span class="sxs-lookup"><span data-stu-id="77d55-110">Only banks residing in these countries are supported, even though banks from other countries may appear in the Envestnet Yodlee Bank Feeds bank selection window in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>

> [!IMPORTANT]
> <span data-ttu-id="77d55-111">Из-за новой Директивы об оказании платежных услуг (PSD2), вступившей в силу в Европе, после 14 сентября 2019 г. вы больше не сможете автоматически импортировать банковские выписки из банков Соединенного королевства в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="77d55-111">Due to the new Payment Services Directive in Europe (PSD2), after September 14, 2019, you will no longer be able to automatically import bank statements from banks in the United Kingdom into [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="77d55-112">Мы изучаем возможности снова сделать эту функцию доступной в будущем.</span><span class="sxs-lookup"><span data-stu-id="77d55-112">We are looking into the possibility of offering this feature again in the future.</span></span>

<span data-ttu-id="77d55-113">Служба Envestnet Yodlee Bank Feeds предоставляет следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="77d55-113">The Envestnet Yodlee Bank Feeds service provides the following benefits:</span></span>

* <span data-ttu-id="77d55-114">Нет необходимости вводить данные вручную.</span><span class="sxs-lookup"><span data-stu-id="77d55-114">Removes the need for manual entry.</span></span>
* <span data-ttu-id="77d55-115">Улучшает эффективность и точность выверки платежей.</span><span class="sxs-lookup"><span data-stu-id="77d55-115">Improves efficiency and accuracy when doing payment reconciliation.</span></span>
* <span data-ttu-id="77d55-116">Поддерживает большое количество банков.</span><span class="sxs-lookup"><span data-stu-id="77d55-116">Supports a large number of banks.</span></span>
* <span data-ttu-id="77d55-117">Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="77d55-117">Allows up-to-date information about bank transactions from within [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>
* <span data-ttu-id="77d55-118">Поддерживает ручной и автоматический ввод данных из банковских выписок.</span><span class="sxs-lookup"><span data-stu-id="77d55-118">Supports manual as well as automatic bank feeds.</span></span>
* <span data-ttu-id="77d55-119">Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.</span><span class="sxs-lookup"><span data-stu-id="77d55-119">Enables outsourcing of payment reconciliation to an accountant by providing access to bank statements.</span></span>

## <a name="available-bank-feeds"></a><span data-ttu-id="77d55-120">Доступные банковские каналы</span><span class="sxs-lookup"><span data-stu-id="77d55-120">Available Bank Feeds</span></span>
<span data-ttu-id="77d55-121">Вы можете проверить, поддерживается ли банк, настроив и подключившись к службе Envestnet Yodlee Bank Feeds.</span><span class="sxs-lookup"><span data-stu-id="77d55-121">You can check whether a bank is supported by setting up and connecting to the Envestnet Yodlee Bank Feeds service.</span></span> <span data-ttu-id="77d55-122">Банк появится в списке, если он поддерживается Envestnet Yodlee.</span><span class="sxs-lookup"><span data-stu-id="77d55-122">The bank will appear on the list if it is supported by Envestnet Yodlee.</span></span>

<span data-ttu-id="77d55-123">Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).</span><span class="sxs-lookup"><span data-stu-id="77d55-123">For more information, see [Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="77d55-124">См. также</span><span class="sxs-lookup"><span data-stu-id="77d55-124">See Also</span></span>
<span data-ttu-id="77d55-125">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="77d55-125">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions ](ui-extensions.md)  </span></span>  
[<span data-ttu-id="77d55-126">Автоматическое применение платежей и выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="77d55-126">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
<span data-ttu-id="77d55-127">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="77d55-127">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
