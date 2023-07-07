---
title: Настройка банковских счетов (содержит видео)
description: 'Узнайте, как банковские счета используются в Business Central и как вы можете провести выверку сумм с вашим банком.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'Yodlee, feed, stream'
ms.search.form: '370, 371, 372, 373, 375, 423, 424, 425, 426, 1240, 1280'
ms.date: 01/24/2022
ms.author: edupont
---
# <a name="set-up-bank-accounts"></a>Настройка банковских счетов

Банковские счета в [!INCLUDE[prod_short](includes/prod_short.md)] используются для того, чтобы отслеживать банковские транзакции. Счета могут быть деноминированы в местной валюте либо в иностранной валюте. После настройки банковских счетов можно использовать функцию «Печать платежей». Банковские счета включают дополнительные функции для [выверки платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md), [банковской выверки](bank-how-reconcile-bank-accounts-separately.md), а также импорта и экспорта банковских файлов. Банковские счета также могут быть включены в транзакции в общих журналах. Каждый банковский счет связан со счетом в плане счетов через назначенную группу разноски банковских счетов. Использование банковского счета в платежной транзакции автоматически операцию как на банковском счете, так и на связанном счете главной книги (ГК).  

Банковские счета работают по-разному в зависимости от того, указан ли код валюты:

- Если код валюты пуст

  Все транзакции по банковскому счету производятся в местной валюте (МВ) для текущей организации. Если транзакция выполняется по счету в другой валюте, суммы разносятся по счету в МВ на основе соответствующего обменного курса валюты. Все чеки, выпущенные с этого счета, должны быть выписаны в МВ. Если банковский счет используется в журнале, строка журнала автоматически унаследует пустой код валюты.  
  
- Указан код валюты

  Все транзакции по этому счету и всу выписанные с него чеки должны быть в той же валюте, которая указана в счете.

Вы можете сэкономить время на вводе данных, сделав банковский счет счетом по умолчанию для использования в валюте, указанной для счета. Если вы это сделаете, счет будет назначаться документам продаж и сервиса, в которых используется эта валюта. Чтобы сделать счет по умолчанию для торговых и сервисных документов, на странице **Карточка банковского счета** включите **Использовать по умолчанию для валюты**. При необходимости вы можете выбрать другой счет при работе с документом.

Банковский счет является неотъемлемой частью [!INCLUDE[prod_short](includes/prod_short.md)] и используется во многих других компонентах. На следующем рисунке показаны наиболее важные отношения:

![Иллюстрация отношений банковского счета.](media/Set-Up-Bank-Accounts/Bank_Account_Relations.png)

Как видно, создание банковского счета делает его доступным во всех местах, показанных выше; кроме того, он отражается в виде соответствующего счета ГК и на странице **Информация об организации**.

Банковский счет обычно контролируется ежедневно, чтобы гарантировать, что все новые платежи от клиентов регистрируются как можно быстрее. Это помогает обеспечить отражение фактического статуса клиента в [!INCLUDE[prod_short](includes/prod_short.md)]. Это дает продавцам, бухгалтерам и другим сотрудникам доступ к релевантной и актуальной информации, чтобы они не звонили лишний раз клиенту по поводу просроченных счетов или задержек поставок.  

![Иллюстрация банковского платежа.](media/Set-Up-Bank-Accounts/Bank-payment-flow.png)

Другая задача — импортировать платежи в валюте поставщика с реализованными курсами валют, чтобы убедиться, что фактический статус поставщиков актуален. Проще всего это сделать с помощью функциональности [выверки платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md). В **журнале выверки платежей** можно импортировать банковские транзакции прямо из приложения онлайн-банка и отправлять их более-менее автоматически. Журнал автоматически определяет и публикует следующее:  

- Прямые дебетовые платежи от клиентов  
- Оплата клиентов по отдельным счетам  
- Единовременные платежи от клиентов  
- Платежи клиентов в иностранной валюте  
- Платежи поставщикам  
- Платежи поставщикам в иностранной валюте  
- Периодические платежи поставщикам и подписки  
- Банковские сборы и проценты  

Выверка платежей обеспечивает значительную экономию времени при учете входящих и исходящих платежей. Однако транзакции по банковскому счету в [!INCLUDE[prod_short](includes/prod_short.md)] не считаются на 100% правильными до тех пор, пока вы не проведете банковскую выверку.  

Банковская выверка — это способ убедиться, что банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)] соответствует внешнему счету в банке.  

 ![Иллюстрация выверки банковского счета.](media/Set-Up-Bank-Accounts/BankReconciliation.png)

На приведенном выше рисунке левая сторона представляет банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)], а правая сторона представляет транзакции, импортированные из банка через приложение интернет-банка. На диаграмме посередине показаны транзакции с обеих сторон, что является банковской выверкой.

С банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)] большинство транзакций должно быть известно физическому банку. К немногим исключениям относятся следующие случаи:  

- Исправления размещены в [!INCLUDE[prod_short](includes/prod_short.md)]  
- Выпущенные чеки, которые еще не были обналичены 
- Платежи поставщикам, не утвержденные банком  

С физического счета в банке постоянно поступают транзакции, которые не были идентифицированы в журнале выверки платежей, например следующие:  

- Подписки новых поставщиков  
- Платежи клиентов без описания
- Банковские проценты
- Банковские комиссии
- Списания с кредитных карт, информация о которых еще не поступила

Чем лучше вам удается сопоставить информацию в журнале выверки платежей, тем больше транзакций учитывается автоматически, и тем проще становится периодическая банковская выверка.

Посмотрите видео ниже, чтобы узнать, каике основные шаги включает в себя создание банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)].

<br /><br />

> [!Video https://www.microsoft.com/videoplayer/embed/RE3Vhpl?rel=0]

> [!WARNING]
> Некоторые поля могут содержать конфиденциальные данные, например поля **Номер отделения банка**, **Номер банковского счета**, **Код SWIFT** и **Код IBAN**. Подробнее см. в статье [Мониторинг конфиденциальных полей](across-log-changes.md#monitoring-sensitive-fields).

## <a name="to-set-up-bank-accounts"></a>Настройка банковских счетов

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать 1.](media/ui-search/search_small.png "Что вы хотите сделать"), и введите **Банковские счета**, затем выберите связанную ссылку.
2. На странице **Банковские счета** выберите действие **Создать**.
3. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    Например, поле **Банк. счет - учетная группа** связывает банковский счет со счетом ГК в балансовом отчете. Подробнее см. в статье [Настройка учетных групп](finance-posting-groups.md).

> [!TIP]
> Некоторые поля скрыты, пока вы не выберете действие **Показать больше**, — как правило, потому, что они используются редко. Остальные нужно добавлять через персонализацию. Подробнее см. в статье [Персонализация рабочей области](ui-personalization-user.md).

Вы можете создать столько банковских счетов, сколько вам нужно для вашего бизнеса. Для каждого банковского счета необходимо указать информацию, позволяющую однозначно идентифицировать банковский счет. Эта информация включает в себя географический адрес банка, серии номеров для различных типов транзакций, таких как прямой дебет и кредитовые переводы, валюту, в которой указаны суммы, и информацию, которая используется для импорта банковских выписок. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
<!--
The following table explains key fields.

|Field|Description|  
|---------------------------------|---------------------------------------|  
|**General FastTab**||
|No.|Specifies the number of the bank account, according to the specified number series. If the number series allow manual numbering, any alphanumeric code up to 20 characters can be used.|
|Name|The Name of the bank holding the account.|
|Bank Branch No.|Typically used to identify the bank branch in domestic payments, it's very often considered a sensitive field. Learn more at [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Bank Account No.|Typically used to identify the bank account number in domestic payments, it's very often considered a sensitive field. Learn more at [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Balance|Shows the bank account balance in the account currency.|
|Balance (LCY)|Shows the bank account balance in the local currency (LCY).|
|Our Contact Code|Specifies a code to identify the employee responsible for this bank account. The employee must be created in the **Salesperson/Purchaser** table.|
|Blocked|Specifies the related record is blocked from being posted in transactions, for example the account is obsolete after a bank change.|
|SEPA Direct Debit Exp. Format|Specifies the single euro payments area (SEPA) format of the bank file to be exported when you choose **Create Direct Debit File** on the **Direct Debit Collect. Entries** page. Learn more at [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Credit Transfer Msg. Nos.|Specifies the number series for bank instruction messages created with the export file you create from the **Direct Debit Collect. Entries** page. Learn more at [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Direct Debit Msg. Nos.|Specifies the number series to be used on the direct debit file you export for a direct debit collection entry on the **Direct Debit Collect. Entries** page. Learn more at [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Creditor No.|Specifies your company as the creditor in connection with payment collection from customers using SEPA direct debit. Learn more at [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Bank Clearing Standard|The national bank names register used for the sender bank account.|
|Bank Clearing Code|Specifies the code for bank clearing required according to the format standard you selected in the **Bank Clearing Standard** field. The bank clearing code can be used as an alternative to SWIFT and IBAN to identify your bank as the sender of a bank transfer.|
|Last Date Modified|Date of the latest modification of the bank account.|
|**Payment Matching**||
|Disable Automatic Payment Matching|Specifies whether or not to disable automatic payment matching after importing bank transactions for this bank account. Learn more at [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|**Payment Match Tolerance**||
|Match Tolerance Type|Specifies the tolerance the automatic payment application function will use to apply the *Amount Incl. Tolerance Matched* rule for this bank account. Read more in [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|Match Tolerance Value|Specifies if the automatic payment application function will apply the *Amount Incl. Tolerance Matched* rule by percentage or amount. Learn more at [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|**Hidden Fields**||
|Search Name|Specifies an alternate name you can use to search for the record in question when you can't remember the value in the **Name** field.|
|Min. Balance|Specifies a minimum balance for the bank account. This field is for information purposes only.|
|Positive Pay Export Code|Specifies a code for the data exchange definition managing the export of positive-pay files. Learn more at [Export Positive Pay Files](finance-how-positive-pay.md).|
|**Communication FastTab**||
|Address|The address of the bank branch.|
|Address 2|An additional address field for the bank branch.|
|Post Code|The post code of the bank branch.|
|City|The city of the bank branch.|
|Country/Region Code|The country/region code of the bank branch.|
|Phone No.|The phone number of the bank branch.|
|Mobile Phone No.|The mobile phone number of the bank branch.|
|Contact|The main contact in the bank branch. Additional contacts can be created in the **Contacts** module.|
|Fax No.|The fax number of the bank branch.|
|Email|The email address of the bank branch.|
|Home Page|The home page address of the bank branch website.|
|**Posting FastTab**||
|Currency Code|Specifies the relevant currency code for the bank account. Applying a currency code to a bank account limits all transactions to only using the applied currency code. Leaving the currency code blank allows transactions in all currencies, however, the amount will eventually be converted to the LCY using the applied currency rate. Checks issued from this account follow the same rules.|
|Last Check No.|The number of the latest check issued from this account.|
|Transit No.|Specifies a bank identification number of your own choice.|
|Last Statement No.|The number of the latest bank reconciliation posted to this account. Learn more at [Reconcile Bank Accounts](bank-how-reconcile-bank-accounts-separately.md).|
|Last Payment Statement No.|The number of the latest payment reconciliation posted to this account. Learn more at [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|Last Bank Statement|The ending balance of the last bank statement. Learn more at [Reconcile Bank Accounts](bank-how-reconcile-bank-accounts-separately.md).|
|Bank Acc. Posting Group|Specifies a code for the bank account's posting group. The **Bank Acc. Posting Group** connects the bank account to the G/L account in the balance sheet.|
|**Transfer**||
|Transit No.|Specifies a bank identification number of your own choice.|
|SWIFT Code|Specifies the international bank identifier (SWIFT) code of the bank in which you have account. The SWIFT code is very often considered a sensitive field. Learn more at [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|IBAN|Specifies the bank account's international bank account number (IBAN). The IBAN code is very often considered a sensitive field. Learn more at [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Bank Statement Import Format|Specifies the format of the bank statement file imported into this bank account. This format is used in both the payment reconciliation journals and bank account reconciliations.|
|Payment Export Format|Specifies the format of the bank file that is exported when you choose **Export Payments to File** on the **Payment Journal** page.|
-->

## <a name="to-enter-an-opening-balance"></a>Ввод начального сальдо

Чтобы занести в поле **Сальдо** начальное сальдо, необходимо учесть в книге банковских счетов операцию на соответствующую сумму. Это можно сделать, выполнив выверку банковского счета. Подробнее см. в статье [Выверка банковских счетов](bank-how-reconcile-bank-accounts-separately.md).  
>
> Кроме того, можно реализовать задание начального сальдо в рамках общего создания данных в новых организациях с помощью мастера настройки **Миграция бизнес-данных**. Узнайте больше в разделе [Подготовьтесь к ведению бизнеса](ui-get-ready-business.md).  

> [!IMPORTANT]
> Не учитывайте начальное сальдо непосредственно в главной книге. Наличие на счете ГК операций, учтенных на нем напрямую, обычно приводит к тому, что вы не можете выверить банковский счет. С банковскими счетами в иностранной валюте такая практика приводит к накоплению разниц по мере учета все большего числа банковких выверок. Обычно вы учитываете начальное сальдо непосредственно на банковском счете, а затем эта сумма оказывается на счете ГК. Другой вариант — позднее сторнировать его со счета ГК, который вы используете для сальдирования начального сальдо главной книги. В обоих случаях необходимо сальдировать любой прямой учет на счете ГК до того, как вы начнете свою первую выверку банковских счетов &mdash; особенно если банковский счет открыт в иностранной валюте.

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Настройка банковского счета для импорта или экспорта банковских файлов

Поля на экспресс-вкладке **Перемещение** на странице **Карточка банковского счета** связаны с импортом и экспортом банковских файлов и выписок. Подробнее см. в статьях [Использование расширения AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) и [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 2.](media/ui-search/search_small.png "Что вы хотите сделать") и введите **Банковские счета**, затем выберите соответствующую ссылку.
2. Откройте карточку банковского счета, в которую будут импортироваться или с которой будут экспортироваться банковские файлы.
3. На экспресс-вкладке **Перемещение** заполните необходимые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> Различные службы экспорта файлов и их форматы требуют различных значений настройки на странице **Карточка банковского счета**. Вы получите сообщения о неверных или отсутствующих значениях настройки при попытке экспорта файла. Внимательно прочтите краткие описания полей или ознакомьтесь с соответствующими разделами с процедурами. Например, экспорт файла платежа для электронного платежа в Северной Америке (EFT) требует, чтобы поля **Номер последнего авизо предъявления к оплате** и **Номер транзитного счета** были заполнены. Подробнее см. в статье [Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file).

Поля на экспресс-вкладке **Транзит** на банковском счете служат разным целям в зависимости от того, является ли платеж входящим или исходящим.

На иллюстрации ниже показан маршрут входящих платежей (цифры в описании соответствуют цифрам на иллюстрации):

:::row:::
    :::column:::

1. Транзакции экспортируются с банковского счета в удобочитаемом формате CSV или в собственном формате банка.
2. *Определение обмена данными* сопоставляет информацию в файле с полями в [!INCLUDE[prod_short](includes/prod_short.md)]. Подробнее см. в статье [Настройка обмена данными](across-set-up-data-exchange.md)
3. *Настройка экспорта/импорта данных* определяет экспорт или импорт и связывается с определением обмена данными.
4. *Формат импорта банковских выписок* связывает настройку импорта с банковским счетом.
5. Платежи импортируются через страницу **Журнал выверки платежей** или **Выверка банковского счета**.

  :::column-end:::
  :::column:::

        ![Иллюстрация поступивших от банка платежей на банковские счета.](media/Set-Up-Bank-Accounts/payments-in-and-out-1.png)

  :::column-end:::
:::row-end:::

Входящие платежи всегда импортируются через страницу **Журнал выверки платежей** или непосредственно на страницу **Выверка банковского счета**. Напротив, исходящие платежи могут происходить из любого журнала платежей. Единственным условием является то, что поле **Разрешить экспорт платежей** необходимо выбрать в соответствующем пакете журнала платежей.

На иллюстрации ниже показан маршрут исходящих платежей (цифры в описании соответствуют цифрам на иллюстрации):

:::row:::
    :::column:::

6. Транзакции заполняют собой журнал платежей, подготовленный для экспорта платежей в файл.
7. *Формат импорта банковских выписок* связывает настройку импорта с банковским счетом.
8. *Настройка экспорта/импорта данных* определяет экспорт или импорт и связывается с определением обмена данными.
9. *Определение обмена данными* сопоставляет информацию в файле с полями в [!INCLUDE[prod_short](includes/prod_short.md)]. Подробнее см. в статье [Настройка обмена данными](across-set-up-data-exchange.md)
10. Платежи экспортируются из журнала платежей и импортируются на банковский счет.

  :::column-end:::
  :::column:::

        ![Иллюстрация платежей с банковских счетов, отправленных в банк.](media/Set-Up-Bank-Accounts/payments-in-and-out-2.png)

  :::column-end:::
:::row-end:::

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Настройка банковских счетов поставщиков для экспорта банковских файлов

Поля на экспресс-вкладке **Перемещение** на странице **Карточка банк. счета поставщика** связаны с экспортом банковских потоков и файлов. Подробнее см. в статьях [Использование расширения AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) и [Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file).

[!INCLUDE[purchase-vendor-bank-account](includes/purchase-vendor-bank-account.md)]

## <a name="changing-your-bank-account"></a>Изменение банковского счета

Если вы хотите использовать другой банковский счет для своей компании, вы должны создать новый банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)]. Мы рекомендуем вам не просто заменять информацию о счете, которую вы в настоящее время используете, потому что это может привести к неверным данным. Например, ваш начальный баланс может быть неправильным или ваш банковский поток может перестать работать правильно. Важно хранить текущий и новый счета отдельно.

После создания нового банковского счета необходимо также создать новую группу разноски банка и назначить ее новому счету главной книги. Вы можете снова использовать существующую учетную группу банка, и банковские транзакции будут разноситься на те же счета главной книги, что и транзакции по другим банковским счетам, для которых используется эта же учетная группа банка. Однако мы рекомендуем вам создать новую группу разноски банка и счет главной книги, чтобы упростить выверку.

> [!NOTE]
> Помните, что информация о банковском счете в открытых счетах-фактурах по-прежнему показывает исходный банковский счет. Соответственно, платежи, скорее всего, по-прежнему будут проводиться по этому счету. Мы рекомендуем вам оставить активными обе учетные записи в течение определенного периода времени после внесения изменений.

Чтобы получить более сжатое представление о ваших денежных счетах в финансовой отчетности, используйте счета **Сумма (от)** и **Сумма (до)** в плане счетов, строки **Группировка** в бухгалтерских или категории счетов ГК. Подробнее см. в разделе [Бизнес-аналитика и финансовая отчетность](bi.md).

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/cash-management-dynamics-365-business-central/)

## <a name="see-also"></a>См. также

[Настройка банковских операций](bank-setup-banking.md)  
[Настройка учетных групп](finance-posting-groups.md)  
[Выверка банковских счетов](bank-manage-bank-accounts.md)  
[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Прямой дебет SEPA в Business Central](finance-collect-payments-with-sepa-direct-debit.md)  
[Настройка банковского счета для прямого дебета SEPA](finance-collect-payments-with-sepa-direct-debit.md#to-set-up-your-bank-account-for-sepa-direct-debit)  
[Настройка банковского счета для кредитового перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-set-up-a-bank-account-for-sepa-credit-transfer)  
[Совершение платежей с помощью расширения AMC Banking 365 Fundamentals или кредитного перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)  
[Выверка платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Сведения о главной книге и плане счетов](finance-general-ledger.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
