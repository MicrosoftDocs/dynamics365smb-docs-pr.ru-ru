---
title: Настройка банковских счетов (содержит видео)
description: Узнайте, как банковские счета используются в Business Central и как вы можете провести выверку сумм с вашим банком.
author: bholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Yodlee, feed, stream
ms.search.form: 370, 371, 372, 373, 375, 423, 424, 425, 426, 1240, 1280
ms.date: 01/24/2022
ms.author: edupont
ms.openlocfilehash: 49ddd48a03c8abe9ea9b396bebc4328e2be30104
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8143742"
---
# <a name="set-up-bank-accounts"></a>Настройка банковских счетов

Банковские счета в [!INCLUDE[prod_short](includes/prod_short.md)] используются для того, чтобы отслеживать банковские транзакции. Счета могут быть деноминированы в локальной валюте, либо в иностранной валюте. После настройки банковских счетов можно использовать функцию «Печать платежей». Банковские счета включают дополнительные функции для [выверки платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md), [банковской выверки](bank-how-reconcile-bank-accounts-separately.md) и импорта и экспорта банковских файлов. Банковские счета также могут быть включены в транзакции в общих журналах. Каждый банковский счет связан со счетом в плане счетов через назначенную группу разноски банковских счетов. Использование банковского счета в платежной транзакции автоматически создает запись как для банковского счета, так и для связанного с ним счета ГК.  

Банковские счета работают по-разному в зависимости от того, указан ли код валюты:

- Код валюты пуст

  Все транзакции по банковскому счету будут производиться в местной валюте (МВ) для текущей компании. Если транзакция выполняется по счету в другой валюте, суммы разносятся по счету в МВ на основе соответствующего обменного курса валюты. Все чеки, выпущенные с этого счета, должны быть выписаны в МВ. Если банковский счет используется в журнале, строка журнала автоматически унаследует пустой код валюты.  
- Указан код валюты

  Все транзакции, которые производятся на этом счете, должны быть в той же валюте, которая указана в счете. Все чеки, выпущенные с этого счета, также должны иметь эту валюту.  

Банковский счет является неотъемлемой частью [!INCLUDE[prod_short](includes/prod_short.md)] и используется во многих других возможностях. На следующем рисунке показаны наиболее важные отношения:

![Иллюстрация отношений банковского счета.](media/Set-Up-Bank-Accounts/Bank_Account_Relations.png)

Это означает, что создание банковского счета делает его доступным во всех местах, показанных выше, а также зеркальным отображением для соответствующего счета ГК и на странице **Информация о компании**.

Банковский счет обычно контролируется ежедневно, чтобы гарантировать, что все новые платежи от клиентов регистрируются как можно быстрее. Это помогает убедиться, что фактический статус клиентов отражается в [!INCLUDE[prod_short](includes/prod_short.md)], чтобы продавцы, бухгалтеры и другие сотрудники имели доступ к актуальной информации. Таким образом они избегают ненужных звонков клиенту по поводу просроченных счетов или задержки доставки.  

![Иллюстрация банковского платежа.](media/Set-Up-Bank-Accounts/Bank-payment-flow.png)

Другая задача — импортировать платежи в валюте поставщика с реализованными курсами валют, чтобы убедиться, что фактический статус поставщиков актуален. Самый простой способ убедиться, что банковский счет обновлен, — это использовать возможность [выверка платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md). В **журнале выверки платежей** можно импортировать банковские транзакции прямо из приложения онлайн-банка и отправлять их более-менее автоматически. Журнал автоматически определяет и публикует следующее:  

- Прямые дебетовые платежи от клиентов  
- Оплата клиентов по отдельным счетам  
- Единовременные платежи от клиентов  
- Платежи клиентов в иностранной валюте  
- Платежи поставщикам  
- Платежи поставщикам в иностранной валюте  
- Периодические платежи поставщикам и подписки  
- Банковские сборы и проценты  

Выверка платежей обеспечивает значительную экономию времени при разноске входящих и исходящих платежей. Однако операции по банковскому счету в [!INCLUDE[prod_short](includes/prod_short.md)] не считаются на 100% правильным до тех пор, пока вы не проведете банковскую выверку.  

Банковская выверка — это способ убедиться, что банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)] соответствует внешнему счету в банке.  

 ![Иллюстрация выверки банковского счета.](media/Set-Up-Bank-Accounts/BankReconciliation.png)

На приведенном выше рисунке левая сторона представляет банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)], а правая сторона представляет транзакции, импортированные из банка через приложение онлайн-банка. На диаграмме посередине показаны транзакции с обеих сторон, что является банковской выверкой.

С банковского счета в [!INCLUDE[prod_short](includes/prod_short.md)] большинство транзакций должно быть известно физическому банку. Единственные исключения включают следующие случаи:  

- Исправления размещены в [!INCLUDE[prod_short](includes/prod_short.md)]  
- Выпущенные чеки, которые еще не были обналичены  
- Платежи поставщикам, не утвержденные банком  

С физического счета в банке постоянно поступают неизвестные транзакции, которые не были идентифицированы в журнале выверки платежей, например следующие:  

- Подписки новых поставщиков  
- Платежи клиентов без описания
- Банковские проценты
- Банковские сборы
- Платежи по кредитной карте, о которых еще не сообщалось

Чем точнее отображается информация о сопоставлении, которую вы вводите в журнале выверки платежей, тем больше транзакций проводится автоматически и тем проще становится периодическая банковская выверка.

<br><br>

> [!Video https://www.microsoft.com/videoplayer/embed/RE3Vhpl?rel=0]

<br><br>

> [!WARNING]
> Некоторые поля могут содержать конфиденциальные данные, например поля **Номер отделения банка**, **Номер банковского счета**, **Код SWIFT** и **Код IBAN**. Для получения дополнительной информации см. [Мониторинг конфиденциальных полей](across-log-changes.md#monitoring-sensitive-fields).

## <a name="to-set-up-bank-accounts"></a>Настройка банковских счетов

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Банковские счета**, а затем выберите связанную ссылку.
2. На странице **Банковские счета** выберите действие **Создать**.
3. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    Например, поле **Банк. счет - учетная группа** связывает банковский счет со счетом ГК в балансовом отчете. Дополнительные сведения см. в разделе [Настройка учетных групп](finance-posting-groups.md).

> [!TIP]
> Некоторые поля скрыты, пока вы не выберете действие **Показать больше**, как правило, потому, что они используются редко. Остальные нужно добавлять через персонализацию. Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).

Вы можете создать столько банковских счетов, сколько вам нужно для вашего бизнеса. Для каждого банковского счета необходимо указать информацию, позволяющую однозначно идентифицировать банковский счет. Эта информация включает в себя географический адрес банка, серии номеров для различных типов транзакций, таких как прямой дебет и кредитовые переводы, валюту, в которой указаны суммы, и информацию, которая используется для импорта банковских выписок. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
<!--
The following table explains key fields.

|Field|Description|  
|---------------------------------|---------------------------------------|  
|**General FastTab**||
|No.|Specifies the number of the bank account, according to the specified number series. If the number series allow manual numbering, any alphanumeric code up to 20 characters can be used.|
|Name|The Name of the bank holding the bank account.|
|Bank Branch No.|The Bank Branch No. is usually used to identify the bank branch in domestic payments. The Bank Branch No. is very often considered a sensitive field. Read more about [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Bank Account No.|Bank Account No. is usually used to identify the bank account no. in domestic payments. The Bank Account No. is very often considered a sensitive field. Read more about [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Balance|Shows the Balance of the bank account in the account currency.|
|Balance (LCY)|Shows the Balance of the bank account in the local currency (LCY).|
|Our Contact Code|Specifies a code to specify the employee who is responsible for this bank account. The employee must be created in the **Salesperson/Purchaser** table.|
|Blocked|Specifies that the related record is blocked from being posted in transactions, for example the account is obsolete after a bank change.|
|SEPA Direct Debit Exp. Format|Specifies the SEPA format of the bank file that will be exported when you choose the **Create Direct Debit File** button in the **Direct Debit Collect. Entries** window. Read more in [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Credit Transfer Msg. Nos.|Specifies the number series for bank instruction messages that are created with the export file that you create from the Direct Debit Collect. Entries window. Read more in [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Direct Debit Msg. Nos.|Specifies the number series that will be used on the direct debit file that you export for a direct-debit collection entry in the Direct Debit Collect. Entries window. Read more in [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Creditor No.|Specifies your company as the creditor in connection with payment collection from customers using SEPA Direct Debit. Read more in [SEPA Direct Debit in Business Central](finance-collect-payments-with-sepa-direct-debit.md).|
|Bank Clearing Standard|The national bank names register used for the sender bank account.|
|Bank Clearing Code|Specifies the code for bank clearing that is required according to the format standard that you selected in the Bank Clearing Standard field. The bank clearing code can be used as an alternative to SWIFT and IBAN to identify your bank as sender of a bank transfer.|
|Last Date Modified|Date of the latest modification of the bank account.|
|**Payment Matching**||
|Disable Automatic Payment Matching|Specifies whether to disable automatic payment matching after importing bank transactions for this bank account. Read more in [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|**Payment Match Tolerance**||
|Match Tolerance Type|Specifies by which tolerance the automatic payment application function will apply the Amount Incl. Tolerance Matched rule for this bank account. Read more in [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|Match Tolerance Value|Specifies if the automatic payment application function will apply the Amount Incl. Tolerance Matched rule by Percentage or Amount. Read more in [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|**Hidden Fields**||
|Search Name|Specifies an alternate name that you can use to search for the record in question when you cannot remember the value in the Name field.|
|Min. Balance|Specifies a minimum balance for the bank account. This field is for information purposes only.|
|Positive Pay Export Code|Specifies a code for the data exchange definition that manages the export of positive-pay files. Read more in [Export Positive Pay Files](finance-how-positive-pay.md).|
|**Communication FastTab**||
|Address|The address of the bank branch.|
|Address 2|An additional address field for the bank branch.|
|Post Code|The post code of the bank branch.|
|City|The city of the bank branch.|
|Country/Region Code|The Country/Region Code of the bank branch.|
|Phone No.|The Phone No. of the bank branch.|
|Mobile Phone No.|The Mobile Phone No. of the bank branch.|
|Contact|The main contact in the bank branch. Additional contacts can be created in the Contacts module.|
|Fax No.|The Fax No. of the bank branch.|
|Email|The Email of the bank branch.|
|Home Page|The Home Page of the bank branch.|
|**Posting FastTab**||
|Currency Code|Specifies the relevant currency code for the bank account. Applying a currency code to a bank account will limit all transactions to only use the applied currency code. Leaving the currency code blank will allow transactions in all currencies, however, the amount will be converted to the local currency (LCY) using the applied currency rate. Checks issued from this account will also follow the same rules.|
|Last Check No.|The number of the latest check issued from this account.|
|Transit No.|Specifies a bank identification number of your own choice.|
|Last Statement No.|The number of the latest bank reconciliation posted to this account. Read more in [Reconcile Bank Accounts](bank-how-reconcile-bank-accounts-separately.md).|
|Last Payment Statement No.|The number of the latest payment reconciliation posted to this account. Read more in [Payment Reconciliation](receivables-apply-payments-auto-reconcile-bank-accounts.md).|
|Last Bank Statement|The ending-balance of the last bank statement. Read more in [Reconcile Bank Accounts](bank-how-reconcile-bank-accounts-separately.md).|
|Bank Acc. Posting Group|Specifies a code for the bank account posting group for the bank account. The Bank Acc. Posting Group connects the bank account to the G/L Account in the balance sheet.|
|**Transfer**||
|Transit No.|Specifies a bank identification number of your own choice.|
|SWIFT Code|Specifies the international bank identifier code (SWIFT) of the bank where you have the account. The SWIFT Code is very often considered a sensitive field. Read more about [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|IBAN|Specifies the bank account's international bank account number. The IBAN Code is very often considered a sensitive field. Read more about [Monitoring Sensitive Fields](across-log-changes.md#monitoring-sensitive-fields).|
|Bank Statement Import Format|Specifies the format of the bank statement file that can be imported into this bank account. The format is being used in both the payment reconciliation journals and the bank account reconciliations.|
|Payment Export Format|Specifies the format of the bank file that will be exported when you choose the Export Payments to File button in the Payment Journal window.|
-->
> [!NOTE]
> Чтобы занести в поле **Сальдо** начальное сальдо, необходимо учесть в книге банковских счетов операцию на соответствующую сумму. Это можно сделать, выполнив выверку банковского счета. Дополнительные сведения см. в разделе [Выверка банковских счетов](bank-how-reconcile-bank-accounts-separately.md).  
>
> Кроме того, можно реализовать начальное сальдо как часть общего создания данных в новых организациях с помощью мастера настройки **Миграция бизнес-данных**. Дополнительные сведения см. в разделе [Подготовьтесь к ведению бизнеса](ui-get-ready-business.md).  

> [!IMPORTANT]
> Важно, чтобы вы не проводили начальное сальдо непосредственно в главную книгу. Наличие записей на счете ГК, проводящихся непосредственно по счету ГК, обычно приводит к тому, что вы не сможете выверить банковский счет или, в случае банковских счетов в иностранной валюте, приводит к накоплению разниц по мере проводки дополнительных банковских выверок. Часто вы проводите начальное сальдо непосредственно по банковскому счету, а затем сумма оказывается на счете ГК. В качестве альтернативы вы сторнируете его позже по назначенному счету ГК, который вы использовали для балансирования начального баланса главной книги. В обоих случаях вы должны сбалансировать любую прямую проводку по счету ГК до того, как начнете свою первую выверку банковских счетов, особенно если банковский счет открыт в иностранной валюте.  

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Настройка банковского счета для импорта или экспорта банковских файлов

Поля на экспресс-вкладке **Перемещение** на странице **Карточка банковского счета** связаны с импортом и экспортом банковских файлов и выписок. Для получения дополнительной информации см. разделы [Использование расширения AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) и [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Банковские счета**, а затем выберите связанную ссылку.
2. Откройте карточку банковского счета, в которую будут импортироваться или экспортироваться банковские файлы.
3. На экспресс-вкладке **Перемещение** заполните необходимые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
> Различные службы экспорта файлов и их форматы требуют различных значений настройки на странице **Карточка банковского счета**. Вы получите сообщения о неверных или отсутствующих значениях настройки при попытке экспорта файла. Поэтому внимательно прочтите краткие описания полей или ознакомьтесь с соответствующими разделами с процедурами. Например, экспорт файла платежа для электронного платежа в Северной Америке (EFT) требует, чтобы поля **Номер последнего авизо предъявления к оплате** и **Номер транзитного счета** были заполнены. Дополнительные сведения см. в разделе [Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file).

Поля на экспресс-вкладке **Транзит** на банковском счете служат разным целям в зависимости от того, является ли платеж входящим или исходящим.

На иллюстрации показан маршрут входящих платежей:

:::row:::
    :::column:::
        1. Транзакции экспортируются с банковского счета в удобочитаемом формате CSV или в собственном формате банка.
        <br><br>
2. *Определение обмена данными* сопоставляет информацию в файле с полями в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения даны в разделе [Настройка обмена данными](across-set-up-data-exchange.md)
<br><br>
3. *Настройка экспорта/импорта данных* определяет экспорт или импорт и ссылается на определение обмена данными.
<br><br>
4. *Формат импорта банковских выписок* связывает настройку импорта с банковским счетом.
<br><br>
5. Платежи импортируются через страницу **Журнал выверки платежей** или **Выверка банковского счета**.
    :::column-end:::
    :::column:::
        ![Иллюстрация поступивших от банка платежей на банковские счета.](media/Set-Up-Bank-Accounts/payments-in-and-out-1.png)
    :::column-end:::
:::row-end:::

Входящие платежи всегда импортируются через страницу **Журнал выверки платежей** или непосредственно на странице **Выверка банковского счета**. Напротив, исходящие платежи могут происходить из любого журнала платежей. Единственным условием является то, что поле **Разрешить экспорт платежей** необходимо выбрать в соответствующем пакете журнала платежей.

На иллюстрации показан маршрут исходящих платежей:

:::row:::
    :::column:::
        6. Проводки, занесенные в журнал платежей, подготовленный для экспорта платежей в файл.
        <br><br>
        7. *Формат импорта банковских выписок* связывает настройку импорта с банковским счетом
        <br><br>
        8. *Настройка экспорта/импорта данных* определяет экспорт или импорт и связывается с определением обмена данными.
        <br><br>
        9. *Определение обмена данными* сопоставляет информацию в файле с полями в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения даны в разделе [Настройка обмена данными](across-set-up-data-exchange.md)
        <br><br>
        10. Платежи экспортируются из журнала платежей и импортируются на банковский счет.
    :::column-end:::
    :::column:::
        ![Иллюстрация платежей с банковских счетов, отправленных в банк.](media/Set-Up-Bank-Accounts/payments-in-and-out-2.png)
    :::column-end:::
:::row-end:::

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Настройка банковских счетов поставщиков для экспорта банковских файлов

Поля на экспресс-вкладке **Перемещение** на странице **Карточка банк. счета поставщика** связаны с экспортом банковских файлов и выписок. Для получения дополнительной информации см. разделы [Использование расширения AMC Banking 365 Fundamentals](ui-extensions-amc-banking.md) и [Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file).

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Поставщики**, а затем выберите связанную ссылку.
2. Откройте карточку поставщика, на банковских счет которого будут экспортироваться банковские файлы платежей.
3. Выберите действие **Банковские счета**.
4. Из **Список банковских счетов поставщика** выберите соответствующий банковский счет или добавьте новый банковский счет.  
5. На странице **Карточка банк. счета поставщика** на экспресс-вкладке **Перемещение** заполните требуемые поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!WARNING]
> Некоторые поля в банковском счете поставщика могут содержать конфиденциальные данные, например поля **Номер отделения банка**, **Номер банковского счета**, **Код SWIFT** и **Код IBAN**. Для получения дополнительной информации прочитайте [Мониторинг конфиденциальных полей](across-log-changes.md#monitoring-sensitive-fields).

## <a name="changing-your-bank-account"></a>Изменение банковского счета

Если вы хотите использовать другой банковский счет для своей компании, вы должны создать новый банковский счет в [!INCLUDE[prod_short](includes/prod_short.md)]. Мы рекомендуем вам не просто заменять информацию о счете, которую вы в настоящее время используете, потому что это может привести к неверным данным. Например, ваш начальный баланс может быть неправильным или ваш банковский поток может перестать работать правильно. Важно хранить текущий и новый счета отдельно.

После создания нового банковского счета необходимо также создать новую группу разноски банка и назначить ее новому счету главной книги. Вы можете повторно использовать существующую группу разноски банка, и банковские операции будут разноситься на те же счета главной книги, что и другие банковские счета, которые разделяют группу разноски банка. Однако мы рекомендуем вам создать новую группу разноски банка и счет главной книги, чтобы упростить выверку.

> [!NOTE]
> Помните, что информация о банковском счете в открытых счетах-фактурах по-прежнему показывает исходный банковский счет. Соответственно, платежи, скорее всего, по-прежнему будут проводиться по этому счету. Мы рекомендуем вам оставить активными обе учетные записи в течение определенного периода времени после внесения изменений.

Чтобы получить более сжатое представление о ваших денежных счетах в финансовой отчетности, используйте счета **Сумма (от)** и **Сумма (до)** в вашем плане счетов, строки **Группировка** в финансовых отчетах или категории счетов ГК. Для получения дополнительной информации прочитайте раздел [Бизнес-аналитика и Financial Reporting](bi.md).

## <a name="see-also"></a>См. также

[Настройка банковских операций](bank-setup-banking.md)  
[Настройка учетных групп](finance-posting-groups.md)  
[Выверка банковских счетов](bank-manage-bank-accounts.md)  
[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)  
[Прямой дебет SEPA в Business Central](finance-collect-payments-with-sepa-direct-debit.md)  
[Настройка банковского счета для прямого дебета SEPA](finance-collect-payments-with-sepa-direct-debit.md#to-set-up-your-bank-account-for-sepa-direct-debit)  
[Настройка банковского счета для кредитового перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#to-set-up-a-bank-account-for-sepa-credit-transfer)  
[Выполнение платежей с помощью расширения AMC Banking 365 Fundamentals или кредитного перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)  
[Выверка платежей](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Сведения о главной книге и плане счетов](finance-general-ledger.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
