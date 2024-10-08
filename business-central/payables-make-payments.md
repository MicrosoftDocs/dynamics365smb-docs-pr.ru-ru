---
title: Обзор задач по управлению платежами поставщикам
description: 'Описываются задачи по управлению платежами поставщикам или кредиторам, включая учет строк платежей и получение обзора сумм к оплате.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: overview
ms.search.keywords: 'print check, vendor payment, creditor, debt, balance due, AP'
ms.search.form: '254, 256, 1190, 1191, 1227, 1228, 1229'
ms.date: 07/15/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="make-payments"></a>Совершение платежей

Платежи поставщика или клиентам, а также возмещение расходов сотрудникам, осуществляется путем учета строк платежей на странице **Журнал платежей**. Журнал платежей — это финансовый журнал, оптимизированный для совершения платежей и содержащий множество мощных действий. Например, действие **Предлож. оплаты поставщикам**, которое находит платежи поставщикам, срок которых наступил, и отчет **Поставщик - сводка задолженности с распределением по срокам**, который представляет собой обзор причитающихся платежей поставщикам.  

Процесс оплаты можно запускать из списков, карточек и операций книг учета по поставщикам, клиентам и сотрудникам. Каждая из этих страниц содержит кнопку, которая начинает процесс платежа и помогает в заполнении журнала платежей.  

Из журнала платежей можно распечатывать электронные платежные документы или записывать, когда платежные документы были выписаны. Если в поле **Тип банковского платежа** выбрано значение **Компьютерный плат. документ**, перед учетом журнала платежей необходимо напечатать строки, представляющие платежные документы.

При учете платежей вы можете экспортировать их в банковский файл для отправки в банк для дальнейшей обработки.

После выполнения всех платежей в банке их необходимо применить к соответствующим открытым операциям книги поставщиков или сотрудников. Применить их можно вручную или путем импорта файла банковской выписки и применения платежей автоматически. Дополнительные сведения см. в разделе [Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md).

В следующей таблице приводится последовательность задач со ссылками на статьи, в которых они описываются.

| По | Ссылка |
| --- | --- |
|Описание основных функций страницы **Журнал платежей**, которое основано на финансовом журнале, для подготовки к учету платежей поставщикам или сотрудникам.|[Работа с финансовыми журналами](ui-work-general-journals.md)|
|Учет платежей в адрес поставщиков или сотрудников и возвратов в адрес клиентов и (при необходимости) применение платежей к соответствующим неоплаченным счетам/кредит-нотам для их закрытия в качестве оплаченных.|[Регистрация платежей и возвратов](payables-how-post-payments-refunds.md)|
| Использование функции на странице **Журнал платежей** для предложения оплат поставщикам в соответствии с выбранными критериями, такими как срок оплаты, доступность скидки и ваша ликвидность. |[Предлож. оплаты поставщикам](payables-how-suggest-vendor-payments.md) |
| Выпуск платежных документов для платежей поставщикам или возвратов клиентам в печатном виде или в электронном виде. Аннулируйте чеки перед учетом или после него. |[Совершение платежей с помощью платежных документов](payables-how-work-checks.md) |
|Выполнение электронных платежей согласно стандарту кредитового перевода SEPA в ЕС.|[Выполнение платежей с помощью расширения AMC Banking 365 Fundamentals или кредитного перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|
| Платите поставщику наличными или чеком, и учитывайте платеж при учете счета. |[Немедленное создание счетов покупки](finance-how-to-settle-purchase-invoices-promptly.md) |
| Убедитесь, что банк выполняет клиринг только проверенных платежных документов и сумм, отправив ему файл, содержащий сведения о поставщике, платежном документе и платеже. |[Экспорт файла Positive Pay](finance-how-positive-pay.md) |

## <a name="see-also"></a>См. также

[Управление кредиторской задолженностью](payables-manage-payables.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Управление дебиторской задолженностью](receivables-manage-receivables.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
