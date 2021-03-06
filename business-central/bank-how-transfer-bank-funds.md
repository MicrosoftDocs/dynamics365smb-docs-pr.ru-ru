---
title: Перевод банковских средств
description: Вы можете переводить суммы между банковскими счетами, в том числе в различных валютах, учитывая транзакции в финансовом журнале.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 04/29/2021
ms.author: edupont
ms.openlocfilehash: da9c8711751040cecb267a3b2209bad2534b618b
ms.sourcegitcommit: 08ca5798cf3f04fc3ea38fff40c1860196a70adf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "5985391"
---
# <a name="transfer-bank-funds"></a>Перевод банковских средств

Иногда бывает необходимо перевести сумму с одного банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)] на другой. Для этого необходимо учесть транзакцию на странице **Финансовый журнал**. Задача зависит от того, используется на банковских счетах одна валюта или различные валюты.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Учет перемещения между банковскими счетами с одним кодом валюты

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.
2. В строке журнала заполните поля **Дата учета** и **Номер документа**
3. В поле **Тип счета** выберите значение **Банковский счет**.
4. В поле **Номер счета** выберите банк, из которого необходимо перевести средства.
5. В поле **Сумма** укажите сумму для перевода.

    Далее необходимо указать балансирующий счет. Если вы не видите соответствующие поля, выберите действие **Показать больше столбцов** для просмотра всех доступных полей.
6. В поле **Тип баланс. счета** выберите **Банковский счет.**
7. В поле **Номер баланс. счета** выберите банковский счет, на который необходимо перевести средства.
8. Учтите журнал.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Учет перемещения между банковскими счетами с разными кодами валют

Для переноса средств между банковскими счетами, которые используют различные валюты, необходимо учесть две строки финансового журнала.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовый журнал**, затем выберите соответствующую ссылку.
2. Создайте две строки журнала и заполните поля **Дата учета** и **Номер документа**.
3. В первой строке журнала в поле **Тип** выберите **Банковский счет**.
4. В поле **Номер счета** выберите банковский счет, с которого необходимо перевести средства.
5. В поле **Количество** введите сумму в валюте банковского счета со знаком минус или без него.

    > [!TIP]
    > Сумма без знака минус — дебет, а сумма со знаком минус — кредит.

    > [!NOTE]
    > Некоторые компании предпочитают переводить между счетами по отдельным строкам журнала. Другие компании предпочитают размещать все в одной строке журнала, используя балансирующий счет. Если вы не знаете, что делать, посоветуйтесь со своим местным экспертом.
    >
    > Если ваша компания предпочитает использовать балансирующий счет, установите поле **Тип баланс. счета** как **Банковский счет**, и установите **Номер баланс. счета** как банковский счет, на который вы хотите перевести средства. Затем переходите к шагу 9 или 10.
    >
    > Если ваша компания предпочитает использовать отдельную строку журнала, переходите к следующему шагу.
6. Во второй строке журнала в поле **Тип** выберите **Банковский счет**.
7. В поле **Номер счета** выберите банковский счет, на который необходимо перевести средства.
8. В поле **Количество** введите сумму в валюте банковского счета со знаком минус или без него.

    > [!TIP]
    > Сумма без знака минус — дебет, а сумма со знаком минус — кредит.
9. Если валютные курсы, используемые в журнале, отличаются от валютных курсов на странице **Валютные курсы**, введите новую строку журнала для прибыли или убытка по курсовым разницам.  

    1. Введите **Счет ГК** в поле **Тип счета**.  

    2. Введите номер счета ГК для прибыли или убытка по курсовой разнице в поле **Номер счета**.  

    3. Введите прибыли или убытки по курсовым разницам в поле **Количество** со знаком минус или без него.

    > [!TIP]
    > Сумма без знака минус — дебет, а сумма со знаком минус — кредит.
10. Учтите журнал.

## <a name="see-also"></a>См. также

[Выверка банковских счетов](bank-manage-bank-accounts.md)  
[Настройка банковских операций](bank-setup-banking.md)  
[Работа с финансовыми журналами](ui-work-general-journals.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]