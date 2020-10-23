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
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3107c42fd584a58fc13ad2bfeacea0ed14e28de7
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3918592"
---
# <a name="the-envestnet-yodlee-bank-feeds-extension"></a>Расширение Envestnet Yodlee Bank Feeds
Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке. Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.

Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.

> [!NOTE]
> Служба Envestnet Yodlee Bank Feeds поддерживается только в сетевой версии Business Central. Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.<br /><br />
> Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.
> Поддерживаются только банки, расположенные в этих странах, хотя банки из других стран могут появляться в окне выбора банка Envestnet Yodlee Bank Feeds в [!INCLUDE[d365fin](includes/d365fin_md.md)],

> [!IMPORTANT]
> Из-за новой Директивы об оказании платежных услуг (PSD2), вступившей в силу в Европе, после 14 сентября 2019 г. вы больше не сможете автоматически импортировать банковские выписки из банков Соединенного королевства в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Мы изучаем возможности снова сделать эту функцию доступной в будущем.

Служба Envestnet Yodlee Bank Feeds предоставляет следующие преимущества:

* Нет необходимости вводить данные вручную.
* Улучшает эффективность и точность выверки платежей.
* Поддерживает большое количество банков.
* Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[d365fin](includes/d365fin_md.md)].
* Поддерживает ручной и автоматический ввод данных из банковских выписок.
* Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.

## <a name="available-bank-feeds"></a>Доступные банковские каналы
Вы можете проверить, поддерживается ли банк, настроив и подключившись к службе Envestnet Yodlee Bank Feeds. Банк появится в списке, если он поддерживается Envestnet Yodlee.

Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).

## <a name="see-also"></a>См. также
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)    
[Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
