---
title: Настройка банковских счетов поставщика
description: 'Узнайте, как связать банковские счета с карточками поставщиков в Business Central, включая контактную информацию, коды SWIFT и IBAN.'
author: brentholtorf
ms.service: dynamics-365-business-central
ms.topic: article
ms.date: 07/04/2022
ms.author: bholtorf
---
# Настройка банковских счетов поставщика

Вы можете использовать информацию о банковском счете в [!INCLUDE [prod_short](includes/prod_short.md)], чтобы отслеживать банковские транзакции вашей компании, но также вы также можете задать банковские реквизиты для поставщиков. Данные банковского счета поставщика могут упростить платежи поставщикам, если использовать [расширение AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) или, например, функцию [Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md).

## Добавление и изменение банковского счета поставщика

[!INCLUDE [purchase-vendor-bank-account](includes/purchase-vendor-bank-account.md)]

> [!TIP]
> Вы можете установить дополнительные банковские счета поставщика на странице **Список банковских счетов поставщика**.

## Настройка предпочтительного банковского счета поставщика

Если у поставщика есть один или несколько банковских счетов и вы хотите выбрать предпочтительный вариант для строк журнала платежей, выполните следующие действия:

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 1.](media/ui-search/search_small.png "Что вы хотите сделать") и введите **Поставщики**, а затем выберите связанную ссылку.
2. Открытие карточки поставщика.
3. На экспресс-вкладке **Платежи** выберите банковский счет поставщика по умолчанию в поле **Код предпочитаемого банковского счета**.

## См. также

[Настройка покупки](purchasing-setup-purchasing.md)  
[Регистрация новых поставщиков](purchasing-how-register-new-vendors.md)  
[Настройка банковских счетов](bank-how-setup-bank-accounts.md)  
[Использование расширения AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md)  
[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
