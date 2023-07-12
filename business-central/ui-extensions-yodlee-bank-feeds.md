---
title: Выверка платежей с использованием расширения Envestnet Yodlee Bank Feeds
description: 'Описание расширения Envestnet Yodlee Bank Feeds, которое устанавливает связь с банковскими счетами для быстрой выверки банковских платежей.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'app, add-in, manifest, customize, stream, bank account link'
ms.search.form: '1450, 1451, 1452, 1453, 1454, 1458, 1460,'
ms.date: 04/01/2021
ms.author: edupont
---
# Расширение Envestnet Yodlee Bank Feeds

Для быстрой выверки платежей на ваши банковские счета вы можете использовать службу Envestnet Yodlee Bank Feeds, которая позволяет связать банковский счет в вашей системе со счетом в интернет-банке. Это означает, что последняя банковская выписка автоматически или вручную будет передаваться в ваш журнал выверки, чтобы вы всегда обрабатывали последний платежи с минимальным риском ошибок.

Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.

> [!NOTE]
> Служба Envestnet Yodlee Bank Feeds поддерживается только в сетевой версии Business Central. Чтобы воспользоваться этой функцией в локальной версии, необходимо получить кобрендинговую учетную запись у Envestnet Yodlee.<br /><br />
> Служба Envestnet Yodlee Bank Feeds поддерживается только в США и Канаде.
> Поддерживаются только банки, расположенные в этих странах/регионах, хотя банки из других стран/регионов могут появляться в окне выбора банка Envestnet Yodlee Bank Feeds в [!INCLUDE[prod_short](includes/prod_short.md)],

> [!IMPORTANT]
> Из-за новой Директивы об оказании платежных услуг (PSD2), вступившей в силу в Европе, после 14 сентября 2019 г. вы больше не сможете автоматически импортировать банковские выписки из банков Соединенного королевства в [!INCLUDE[prod_short](includes/prod_short.md)]. Мы изучаем возможности снова сделать эту функцию доступной в будущем.

Служба Envestnet Yodlee Bank Feeds предоставляет следующие преимущества:

* Нет необходимости вводить данные вручную.
* Улучшает эффективность и точность выверки платежей.
* Поддерживает большое количество банков.
* Позволяет использовать актуальную информацию о банковских транзакциях из [!INCLUDE[prod_short](includes/prod_short.md)].
* Поддерживает ручной и автоматический ввод данных из банковских выписок.
* Позволяет поручать выверку платежей бухгалтеру, предоставляя ему доступ к банковским выпискам.

## Доступные банковские каналы

Вы можете проверить, поддерживается ли банк, настроив и подключившись к службе Envestnet Yodlee Bank Feeds. Банк появится в списке, если он поддерживается Envestnet Yodlee.

Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).

## См. также

[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)  
[Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
