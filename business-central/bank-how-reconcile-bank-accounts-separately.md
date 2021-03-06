---
title: Выверка банковских счетов | Microsoft Docs
description: Далее описывается процедура выверки стоимости запасов с главной книгой.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account balance, bank statement
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1049043da0fd4cd5db2dc76f41a3c3df0402bbfc
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5786811"
---
# <a name="reconcile-bank-accounts"></a>Выверка банковских счетов

Вы проводите выверку банковских счетов, чтобы убедиться, что ваши бизнес-операции и расходы правильно отражены в бухгалтерских книгах компании. Для этого вы сравниваете и сопоставляете записи на своих внутренних банковских счетах с банковскими операциями в вашем банке, а затем учитываете сальдо на своих внутренних банковских счетах, чтобы итоги были доступны финансовым менеджерам. Банковская выверка также является практическим способом выявления и устранения недостающих платежей и ошибок в бухгалтерском учете.

Ниже описано, как выполнить выверку банковских счетов на странице **Выверка банковских счетов**.

> [!TIP]
> Вы также можете выверять банковские счета на странице **Журнал выверки платежей** при обработке платежей. Если выбрать действие **Учесть платежи и выверить банковский счет**, все открытые операции книги банковских счетов, связанные с примененными операциями книг клиентов или поставщиков, будут закрыты. При этом автоматически выверяется банковский счет по платежам, которые учтены с использованием журнала. Дополнительные сведения см. в разделе [Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md).

> [!NOTE]  
> В версиях для Северной Америки проделать эту работу также можно на странице **Журнал банковской выверки**, которое лучше подходит для работы с платежными документами и депозитами, но в котором не предусмотрена возможность импорта файлов банковских выписок. Чтобы использовать эту страницу вместо страницы **Выверка банковского счета**, снимите флажок **Банковская выверка с автосопоставлением** на странице **Настройка ГК**. Дополнительные сведения см. в [Выверка банковских счетов](LocalFunctionality/UnitedStates/how-to-reconcile-bank-accounts.md) в "Локальная функциональность в США".

Строки на странице **Выверка банковского счета** разделены на две области. В области **Строки банковской выписки** показаны импортированные банковские транзакции или операции книги с неоплаченными платежами. В области **Книга операций по банку/кассе** показаны операции книги на внутреннем банковском счете.

Выверка банковских операций с внутренними банковскими записями называется *сопоставлением*. Можно выбрать выполнение соответствия автоматически с помощью функции **Совпадение автоматически**. Кроме того, можно выбрать строки вручную в обеих панелях для связывания каждой строки банковской выписки с одной или несколькими связанными операциями книги операций по банку/кассе, а затем использовать функцию **Совпадение вручную**. В строках с сопоставленными операциями установлен флажок **Применено**. Дополнительные сведения см. в разделе [Настройка правил для автоматического применения платежей](receivables-how-set-up-payment-application-rules.md).

> [!NOTE]  
> Если строки импорта банковских выписок относятся к операциям платежной книги, функции сопоставления использовать нельзя. Вместо этого необходимо выбрать действие **Применить операции** и выбрать соответствующую операцию в книге платежных документов для сопоставления строки банковской выписки.

Если значение в поле **Общее сальдо** в области **Строки банковской выписки** равняется значению поля **Сальдо для выверки** в области **Книга операций по банку/кассе**, вы можете выбрать действие **Учет**. Любые несопоставленные записи в книге банковских счетов останутся на странице, что указывает на некоторое расхождение, которое вы должны устранить в рамках выверки банковских счетов.

Любые строки, которые не могут быть сопоставлены (обозначены значением в поле **Разница**), останутся на странице **Выверка банковского счета** после учета. Они представляют собой несоответствие, которое вы должны устранить, прежде чем сможете завершить выверку банковского счета. Типичные бизнес-ситуации, которые могут вызвать расхождения:

| Разница | Причина | Решение |
|------------|--------|------------|
| Транзакция на внутреннем банковском счете отсутствует в банковской выписке. | Банковская транзакция не состоялась, хотя проводка была сделана в [!INCLUDE[prod_short](includes/prod_short.md)]. | Совершите недостающую денежную транзакцию (или попросите об этом дебитора), а затем повторно импортируйте файл банковской выписки или введите транзакцию вручную. |
| Транзакция по банковской выписке не существует в виде строки документа или журнала в [!INCLUDE[prod_short](includes/prod_short.md)]. | Банковская транзакция была совершена без соответствующей проводки в [!INCLUDE[prod_short](includes/prod_short.md)], например учета строки журнала для расходов. | Создайте и отсутствующую запись и выполните ее учет. Для получения информации о быстром способе инициировать эту операцию, см. [Создание отсутствующих операций книги для сопоставления с банковским транзакции](bank-how-reconcile-bank-accounts-separately.md#to-create-missing-ledger-entries-to-match-bank-statement-lines-with). |
| Транзакция на внутреннем банковском счете соответствует банковской транзакции, но некоторая информация слишком различается, что приводит к несоответствию. | Информация, такая как сумма или имя клиента, была введена по-разному при учете банковской или внутренней транзакции. | Проверьте эти информацию и вручную сопоставьте записи. При желании исправьте несоответствие информации. |

Вы должны устранить расхождения, например, путем создания отсутствующих записей и исправления несоответствующей информации, или путем проведения недостающих денежных операций, пока выверка банковского счета не будет завершена и учтена.

Область **Строки банковской выписки** на странице **Выверка банковского счета** можно заполнять следующими способами:

* Автоматически с помощью функции **Импорт выписки с банк. счета** для заполнения области **Строки банковской выписки** банковскими транзакциями в соответствии импортированным файлом или потоком, предоставленным банком.
* Вручную, с помощью функции **Предложить строки** для заполнения области **Строки банковской выписки** в соответствии со счетами [!INCLUDE[prod_short](includes/prod_short.md)] с неоплаченными платежами.

## <a name="to-fill-bank-reconciliation-lines-by-importing-a-bank-statement"></a>Заполнение строк банковской выверки путем импорта банковской выписки

Область **Строки банковской выписки** будет заполнена банковскими транзакциями в соответствии с импортированным файлом или потоком, предоставленным банком.

Чтобы включить импорт банковских выписок в электронном виде, необходимо сначала настроить и включить службу банковских выписок Envestnet Yodlee, а затем связать свои банковские счета с соответствующими счетами интернет-банка. Дополнительные сведения см. в разделе [Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md).  

> [!TIP]
> Вы также можете импортировать файлы банковских выписок в формате с разделением запятыми или точками с запятой (.CSV). Используйте мастер настройки **Настройка формата файла банковской выписки** для определения форматов импорта банковских выписок и их прикрепления к банковскому счету. Затем вы можете использовать эти форматы при импорте банковских выписок на странице **Выверка банковского счета**.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Выверка банковского счета**, затем выберите соответствующую ссылку.
2. Выберите действие **Создать**.
3. В поле **Номер банковского счета** выберите соответствующий банковский счет. Операции книги банковских счетов, существующие для банковского счета, будут отображаться в области **Книга операций по банку/кассе**.
4. В поле **Дата выписки** укажите дату выписки, полученной из банка.
5. В поле **Конечное сальдо выписки** укажите сальдо из банковской выписки.
6. При наличии файла банковской выписки, выберите действие **Импорт банковской выписки**.
7. Найдите файл, а затем нажмите кнопку **Открыть** для импорта банковских транзакций в область **Строки банковской выписки** на странице **Выверка банковского счета**.

## <a name="to-fill-bank-reconciliation-lines-with-the-suggest-lines-function"></a>Заполнение строки банковской выверки с помощью функции предложения строк

Область **Строки банковской выписки** будет заполнена в соответствии со счетами в [!INCLUDE[prod_short](includes/prod_short.md)], которые имеют непогашенные платежи.  

1. На странице **Выверка банковского счета** выберите действие **Предложить строки**.
2. В поле **Дата начала** укажите самую раннюю дату учета для выверяемых операций книги.
3. В поле **Дата окончания** укажите самую позднюю дату учета для выверяемых операций книги.
4. Установите флажок **Включать платежные документы**, чтобы предложить операции книги платежных документов вместо соответствующих операций книги банковских счетов.
5. Нажмите кнопку **ОК**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-automatically"></a>Автоматическое сопоставление строк банковских выписок с операциями книги банковских счетов

На странице **Выверка банковского счета** предусмотрена функция автоматического сопоставления на основании совпадения текста в строке банковской выписки (в левой области) с текстом в одной или нескольких операций книги банковских счетов (в правой области). Помните, что вы можете изменять предлагаемые автоматические сопоставления платежей или не использовать их вовсе. Дополнительные сведения см. в разделе [Сопоставление строк банковских выписок с операциями книги банковских счетов вручную](bank-how-reconcile-bank-accounts-separately.md#to-match-bank-statement-lines-with-bank-account-ledger-entries-manually).

1. На странице **Выверка банковского счета** выберите **Определять соответствие автоматически**. Откроется страница **Сопоставить банковские операции**.
2. В окне **Отклонение даты транзакции (дни)** укажите период в днях до и после даты учета операции по банковскому счету, в пределах которого функция будет искать соответствующие даты транзакций в банковской выписке.

    Если ввести значение 0 или поле остается пустым, то функция **Сопоставлять автоматически** будет искать даты транзакции, совпадающие с датой учета операции книги банковских счетов.
3. Нажмите кнопку **ОК**.

    Все строки банковских выписок и операций книги банковских счетов, которые можно сопоставить, становятся зелеными, и устанавливается флажок **Применено**.
4. Чтобы удалить сопоставление, выберите строку банковской выписки и выберите действие **Удалить соответствие**.

## <a name="to-match-bank-statement-lines-with-bank-account-ledger-entries-manually"></a>Сопоставление строк банковских выписок с операциями книги банковских счетов вручную

1. На странице **Выверка банковского счета** выберите непримененную строку в области **Строки банковской выписки**.
2. В области **Книга операций по банку/кассе** выберите одну или несколько операций книги банковских счетов, которые можно сопоставить с выделенной строкой банковской выписки. Чтобы выделить несколько строк, нажмите и удерживайте клавишу CTRL.
3. Выберите действие **Определить соответствие вручную**.

    Шрифт выбранной строки банковской выписки и выбранных операций книги платежей становится зеленым, и устанавливается флажок **Применено** в правой панели.
4. Повторите шаги с 1 по 3 для всех строк банковских выписок, которые не совпадают.
5. Чтобы удалить сопоставление, выберите строку банковской выписки и выберите действие **Удалить соответствие**.

## <a name="to-create-missing-ledger-entries-to-match-bank-statement-lines-with"></a>Создание отсутствующих операций книги для сопоставления со строками банковской выписки

Иногда банковская выписка содержит суммы начисленных процентов или взысканных комиссий. Такие строки банковской выписки не удается сопоставить из-за отсутствия соответствующих операций книги в [!INCLUDE[prod_short](includes/prod_short.md)]. Затем нужно учесть строку журнала для каждой транзакции, чтобы создать соответствующую операцию книги, которую можно сопоставить.

1. На странице **Выверка банковского счета** выберите действие **Переместить в финансовый журнал**.  
2. На странице **Перемещ. банк. выверки в фин. журнал** укажите, какую главную книгу требуется использовать, затем нажмите кнопку **ОК**.

    Откроется страница **Финансовый журнал**, содержащая новые строки журнала для всех строк банковской выписки с недостающими операциями книги.
3. Заполните строки журнала соответствующими сведениями, например укажите балансирующий счет. Дополнительные сведения см. в разделе [Работа с финансовыми журналами](ui-work-general-journals.md).  
4. Чтобы проверить результат работы перед его учетом, выберите действие **Тестовый отчет**. Откроется отчет **Выписка по банковскому счету**, содержащий те же поля, что и в заголовке страницы **Выверка банковского счета**.
5. Выберите действие **Учет**.

    После учета операции перейдите к сопоставлению строки банковской выписки.
6. Обновите или заново откройте страницу **Выверка банковского счета**. В области **Книга операций по банку/кассе** появится новая операция книги.
7. Сопоставьте строку банковской выписки с операцией книги банковских счетов вручную или автоматически.

## <a name="undo-a-bank-account-reconciliation"></a>Отмена выверки банковского счета
Если вы обнаружите ошибку в разнесенной выверке банка, вы можете использовать действие **Отмена** на странице **Выписка по банковскому счету**, чтобы исправить ошибку. Когда вы отменяете разнесенную банковскую выверку, записи перемещаются на страницу **Выверка банка** и помечаются как **Открыто**, что означает, что они не выверены. Затем вы можете исправить банковскую выверку и снова разнести ее.

> [!NOTE]
> В версии для Северной Америки, чтобы использовать функцию отмены для разнесенных банковских выверок и банковских выписок, необходимо включить параметр **Выверка банка с автосопоставлением** на странице **Настройка главной книги**. Функция отмены недоступна для выписок по счету, разнесенных из таблиц выверки банковских счетов.

### <a name="reusing-the-bank-statement-number"></a>Повторное использование номера банковской выписки
Номер банковской выписки, используемый для новой банковской выверки, берется из банковского счета, как и последняя выписка сальдо. Вы можете изменить эти значения перед началом новой банковской выверки. Однако при создании новой банковской выверки [!INCLUDE[d365fin](includes/d365fin_md.md)] проверяет, присвоен ли уже номер выписки проведенной выписке по счету. Если номер уже используется, но вы хотите, чтобы он использовался в новой банковской выписке, вы можете использовать действие **Изменить номер выписки** на странице **Выверка банковского счета**.

### <a name="examples"></a>Примеры
Ниже приведены несколько примеров того, как исправить ошибку в проведенной выверке банка с использованием или без использования того же номера выписки.

#### <a name="example-1"></a>Пример 1
Вы выполнили выверку банковских счетов за январь, февраль и март. Номер банковской выписки за март был 100. Позже вы обнаружили, что март включал только записи до 30-го числа, что означает, что записи за 31-е число отсутствуют. Итак, вам нужно переделать банковскую выверку за март. В этом случае мы откроем страницу **Выписка по банковскому счету**, выберем выписку за март, затем выберем **Отмена**. 

Новой банковской выверке присвоен номер выписки 101. Чтобы переназначить номер 100, выберите **Изменить № выписки** и введите **100**. 

> [!TIP]
> Не забудьте установить соответствующую дату окончания выписки (в данном примере это 31 марта) и отредактировать поле **Сальдо последней выписки**. 

#### <a name="example-2"></a>Пример 2
Вы выполнили выверку банковских счетов за январь, февраль, июнь и июль. Вы обнаружили, что февраль был неправильным. Предположим, это эта выписка имела номер 100. Как и в примере 1, вы используете действия "Отмена" и "Изменить № выписки", чтобы изменить номер выписки, как в примере №1 выше, и теперь вы можете повторить выверку банковского счета за февраль.  

После разноски исправленной банковской выверки за февраль на соответствующей карточке банковского счета в поле **Номер посл. выписки** отображается значение **100**, а в поле **Сальдо последней выписки** отображается конечное сальдо для февральской выписки. 

Если вы выполните следующую банковскую выверку за март, [!INCLUDE[d365fin](includes/d365fin_md.md)] присвоит 101 как номер выписки и даст ей правильное **Сальдо последней выписки**.

Если вы выполните следующую выверку банковского счета за август, подумайте об изменении значений в полях **Номер посл. выписки** и **Сальдо последней выписки** на карточке **Банковский счет** перед созданием следующей банковской выверки, или используйте действие "Изменить № выписки", а также измените значение в поле "Сальдо последней выписки" на странице банковской выверки.

> [!NOTE]
> Номер выписки важен, когда вы выполняете банковские выверки с импортированными файлами CAMT, которые содержат номера выписок, или когда вы проводите выверку на основе распечатанных банковских выписок. Если вы просто загружаете ряд банковских операций из своего онлайн-банка, номер выписки обычно не имеет значения. 
>
>Сальдо последней выписки хранится на банковском счете, чтобы свести к минимуму ошибки при выполнении банковских выверок, но его также можно редактировать, что позволяет выполнять банковские выверки в любом порядке. Это также означает, что если вы отмените выписку по счету, новое конечное сальдо может не быть сальдо последней выписки в следующей выписке по счету. Нет функции, которая позволяла бы перемещать сальдо вперед для всех последующих выписок по счету, поэтому помните об этом при использовании отмены. 

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/bank-reconciliation-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Выверка банковских счетов](bank-manage-bank-accounts.md)  
[Автоматическое применение платежей и выверка банковских счетов](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Настройка банковских операций](bank-setup-banking.md)  
[Настройка правил для автоматического применения платежей](receivables-how-set-up-payment-application-rules.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]