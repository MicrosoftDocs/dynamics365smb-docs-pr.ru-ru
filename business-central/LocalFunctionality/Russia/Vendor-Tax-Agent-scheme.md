---
title: Схема налогового агента поставщика в России
description: Российские усовершенствования включают схемы налоговых агентов поставщиков.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 7600d3a101c0e3998eb6823ed668dd9b725d93c3
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2301183"
---
# <a name="vendor-tax-agent-scheme"></a>Схема налогового агента поставщика

## <a name="vat-from-internal-funds"></a>НДС из внутренних фондов

Заполните поля в карточке поставщика.

1. На вкладке "Договор": 

    - Учет договоров - обязательно.

    - Номера договоров обязательны.

2. В карточке договора:

    - НДС бизнес-группа 
    - НДС товарная группа налогового агента
    - Тип источника оплаты НДС - Внутренние фонды

## <a name="prepayment-and-payment-vat"></a>Предоплата и оплата НДС

1. Создание и выпуск счета

Номер договора (с настройками для продавца с уплатой НДС из внутренних фондов) должен быть указан.

2. Создание строки в журнале платежей:

    - Тип документа - Платеж
    - Предоплата - да
    - Номер документа предоплаты не требуется.

3. Выполните учет строк журнала.

    Операции с НДС генерируются автоматически в рублях.

4. Создайте и учтите в журнале платежей для налогового органа строку с суммой НДС для предоплаты.

5. Выполните отгрузку и учет счета.

6. Создайте строку в журнале платежей

    - Тип документа - Платеж
    - Номер начального документа - Номер учтенного счета
    - Примен. к док. - номер - Номер учтенного счета

7. Создайте и выполните учет платежа в налоговый орган.
8. Откройте журнал НДС. Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).

## <a name="vat-from-vendor-funds"></a>НДС из фондов поставщика

Заполните поля в карточке поставщика.

1. На вкладке "Договор": 

    - Учет договоров - обязательно.
    - Номера договоров обязательны.

2. В карточке договора:

    - НДС бизнес-группа 
    - НДС товарная группа налогового агента
    - Тип источника оплаты НДС - Фонды поставщика

## <a name="prepayment-and-payment-vat"></a>Предоплата и оплата НДС

1. Создайте и выпустите счет.

2. Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в **журнале платежей**.

    **Для поставщика:**

        - Posting Date,
        - Document Type - Payment
        - Prepayment - yes
        - Account Type - Vendor
        - Account No.
        - Agreement No.
        - Bal. Account Type - G/L Account
        - Bal. Account - “ ”
        - Currency Code - “ “
        - Prepayment Document No. is required
        - Amount - in rubles

    **Для банка:**

        - Posting Date,
        - Document Type - Payment
        - Prepayment - yes
        - Account Type - Bank Account
        - Account No.
        - Agreement No.
        - Bal. Account Type -  G/L Account
        - Bal. Account - “ ”
        - Currency Code 
        - Amount - in USD/EUR

3. Выполните учет строк журнала.
4. Выполните отгрузку.

    Вы можете изменить код валюты и сумму в счете.

5. Учет счета.

6. Примените операцию.

7. Откройте журнал НДС. Выполните учет НДС (см. [Зачет НДС](Settlement-VAT.md)).

    В конце периода будут формироваться операции в результате переоценки задолженности.

8. Создайте строки в журнале платежей и учтите их.

    Для оплаты в валюте для банка и в рублях для поставщика необходимо создать две строки в журнале платежей.

    **Для поставщика:**

        - Posting Date
        - Document Type - Payment
        - Account Type - Vendor
        - Account No.
        - External Document No.
        - Internal Document No.
        - Agreement No.
        - Bal. Account Type - G/L Account
        - Bal. Account - “ ”
        - Currency Code - “ “
        - Prepayment Document No. is required
        - Amount - in rubles

    **Для банка:**

        - Posting Date,
        - Document Type - Payment
        - Account Type - Bank Account
        - Account No.
        - Agreement No.
        - Bal. Account Type -  G/L Account
        - Bal. Account - “ ”
        - Currency Code 
        - Amount - in USD/EUR

## <a name="see-also"></a>См. также

[Функциональность локальной версии для России](russia-local-functionality.md)  
