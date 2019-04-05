---
title: Выверка платежей с помощью расширения "Банковские выписки Envestnet Yodlee" | Microsoft Docs
description: Описывает расширение "Банковские выписки Envestnet Yodlee", которое устанавливает связь с банковскими счетами для быстрой выверки банковских платежей.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, bank account link
ms.date: 02/26/2019
ms.author: sgroespe
ms.openlocfilehash: 36400b3265517c29f68f7eb59d17d968334e0fb1
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "805238"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a>Расширение "Банковские выписки Envestnet Yodlee"
Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке. Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.

> [!NOTE]
> Эта функция поддерживается только в сетевой версии Business Central. Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.

Служба Envestnet Yodlee Bank Feeds обеспечивает следующие преимущества:

* Нет необходимости вводить данные вручную.
* Улучшает эффективность и точность выверки платежей.
* Поддерживает большое количество банков.
* Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[d365fin](includes/d365fin_md.md)].
* Поддерживает ручной и автоматический ввод данных из банковских выписок.
* Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.

Дополнительные сведения см. в разделе [Настройка службы банковских выписок Envestnet Yodlee](bank-how-setup-bank-statement-service.md).

## <a name="see-also"></a>См. также
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)    
[Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
