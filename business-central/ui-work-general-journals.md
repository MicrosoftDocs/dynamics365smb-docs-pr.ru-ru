---
title: "Использование финансовых журналов для учета непосредственно в ГК | Документы Майкрософт"
description: "Узнайте об использовании финансовых журналов для учета финансовых транзакций на счетах главной книги и других счетах, таких как банковские счета и счета поставщиков."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 02/23/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 090a0141583795757a0d59b358ba4d553100d976
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="working-with-general-journals"></a>Работа с финансовыми журналами
Большинство финансовых транзакций учитываются в главной книге с помощью отдельных бизнес-документов, например счетов покупки и заказов на продажу. Для бизнес-операций, которые не представлены документами в [!INCLUDE[d365fin](includes/d365fin_md.md)], например небольших расходов или наличных поступлений, можно создавать соответствующие транзакции путем учета строк журналов в окне **Финансовый журнал**. Дополнительные сведения см. в разделе [Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).

Например, можно учитывать личные средства, которые сотрудники расходуют на служебные цели, для последующей компенсации. Дополнительные сведения см. в разделе [Регистрация и возмещение расходов сотрудников](finance-how-record-reimburse-employee-expenses.md).

Финансовые журналы используются для учета финансовых транзакций непосредственно на счетах главной книги и других счетах, таких как банковские счета, счета клиентов, счета поставщиков и счета сотрудников. В результате учета в финансовом журнале всегда создаются операции по счетам главной книги. Это верно, даже если, к примеру, строка журнала учитывается в счете клиента, так как операция учитывается в счете дебиторской задолженности главной книги через учетную группу.

Вводимые в журналы сведения являются временными и, пока данные сведения находятся в журналах, они могут быть изменены. При учете журнала информация переносится в операции по отдельным счетам, где ее невозможно изменить. Однако можно отменить применение учтенных операций и учесть сторнирующие или исправляющие операции. Дополнительные сведения см. в разделе [Сторнирование учета](finance-how-reverse-journal-posting.md).

## <a name="using-journal-templates-and-batches"></a>Использование шаблонов и разделов журнала
Существует несколько шаблонов финансовых журналов. Каждый шаблон журнала представляется выделенным окном с определенными функциями и полями, которые нужны для поддержки этих функций, например окно **Журнал выверки платежей** для обработки банковских платежей и окно **Журнал платежей** для оплаты поставщикам или выплаты возмещения своим сотрудникам. Дополнительные сведения см. в разделах [Создание платежей](payables-make-payments.md) и [Выверка платежей клиентов вручную](receivables-how-apply-sales-transactions-manually.md).

Для каждого шаблона журнала вы можете настроить личный журнал в качестве раздела журнала. Например, вы можете определить собственный раздел для журнала платежей, задав собственный макет и параметры. Ниже приведен пример процедуры персонализации журнала.

> [!TIP]  
> Если установить флажок **Предлагаемая балансирующая сумма** в строке раздела в окне **Разделы финансового журнала**, то в поле **Сумма**, например в строках финансового журнала для документа с тем же номером, будет автоматически подставляться значение, балансирующее документ. Дополнительные сведения см. в разделе [Предложение значений в [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-let-system-suggest-values.md).

## <a name="understanding-main-accounts-and-balancing-accounts"></a>Сведения об основных счетах и балансирующих счетах
Если настроить для разделов журналов балансирующие счета по умолчанию на странице **Финансовые журналы**, балансирующий счет будет заполняться автоматически при заполнении поля **Номер счета**. В противном случае поля **Номер счета** и **Номер баланс. счета** необходимо заполнять вручную. На положительную сумму в поле **Сумма** дебетуется основной счет и кредитуется балансирующий. На отрицательную сумму кредитуется основной счет и дебетуется балансирующий.

> [!NOTE]  
>   НДС вычисляется отдельно для основного и балансирующего счетов, благодаря чему для них можно использовать разные процентные ставки НДС.

## <a name="working-with-recurring-journals"></a>Работа с типовыми журналами
Типовой журнал — это финансовый журнал со специальными полями для управления транзакциями, которые часто учитываются с небольшими изменениями или без таковых, такие как аренда, подписки, электричество и отопление. Эти поля для типовых транзакций помогают вести учет фиксированных и переменных сумм. Можно также указать автоматическое сторнирование операций на следующий день после даты учета. Можно также использовать ключи распределения для разделения повторяющихся операций среди различных счетов. Дополнительные сведения см. в разделе "Распределение повторяющихся сумм журналов на несколько счетов".

Благодаря типовому журналу операции, которые должны учитываться регулярно, необходимо вводить только один раз. Это значит, что счета, измерения, значения измерений и т.д. останутся в журнале после учета. При необходимости коррекцию можно делать при каждом учете.

### <a name="recurring-method-field"></a>Поле метода повторения
Это поле определяет, как поступить с суммой в строке журнала после учёта. Например, если вы будет использовать одну и ту же сумму каждый раз при учете строки, то после учета можно оставить сумму неизменной. Если вы хотите использовать в строке один и тот же текст и номер счета, а сумма будет отличаться при каждом учете, то вы можете удалить ее после учета.

| По | Ссылка |
| --- | --- |
|Фиксир.|Сумма в строке журнала сохраняется после учета.|
|Переменный|Сумма в строке журнала удаляется после учета.|
|Баланс|Учтённая сумма на счёте в строке будет распределена между счетами, определёнными для строки в таблице Фин. журнал - распределение. Таким образом, баланс на счёте будет установлен в 0. Не забудьте заполнить поле **Распределение (%)** в окне **Распределения**. Дополнительные сведения см. в разделе "Распределение повторяющихся сумм журналов на несколько счетов".|
|Сторнирование фиксированное|Сумма в строке журнала останется после учёта, а балансирующая операция будет учтена на следующий день.|
|Сторнирование переменное|Сумма в строке журнала будет удалена после учёта, а балансирующая операция будет учтена на следующий день.|
|Сторнирование - баланс|Учтённая сумма на счёте в строке будет распределена между счетами, определёнными для строки в окне **Распределения**. Баланс на счете будет установлен равным нулю, а балансирующая операция учитывается на следующий день.|

> [!NOTE]  
>  Поля НДС могут быть заполнены либо в строке типового журнала, либо в строке журнала распределения, но в обеих строках одновременно. Это значит, что они могут быть заполнены в окне **Распределения** только тогда, когда они не заполнены в типовом журнале.

### <a name="recurring-frequency-field"></a>Поле частоты повторения
Это поле определяет частоту учета операции в строке журнала. Это поле формулы даты, и его необходимо заполнить для строк типового журнала. Дополнительные сведения см. в разделе "Использование формул дат" статьи [Ввод данных](ui-enter-data.md).

#### <a name="examples"></a>Примеры
Если строка журнала должна учитывается ежемесячно, введите "1M." После каждого учёта дата в поле **Дата учета** будет обновляться на ту же дату следующего месяца.

В случае потребности учета операции в последний день каждого месяца можно проделать одно из следующего:

- Для учета первой операции в последний день месяца введите 1Д+1М-1Д (1 день + 1 месяц - 1 день). С помощью этой формулы дата учета вычисляется правильно независимо от количества дней в том или ином месяце.

- Для учета первой операции в произвольный день месяца, введите формулу 1М+ТМ. С помощью этой формулы дата учета будет после одного полного месяца + остающиеся дни текущего месяца.

### <a name="expiration-date-field"></a>Поле даты истечения срока действия
Это поле определяет дату последнего учета строки. Строка не будет учитываться после этой даты.

Преимущество использования этого поля состоит в том, что строка будет удалена из журнала немедленно, и всегда существует возможность заменить настоящую дату действия на более позднюю для последующего использования этой строки.

Если данное поле не заполнено, строка будет учитываться при каждом учете вплоть до ее удаления из журнала.

### <a name="allocating-recurring-journal-amounts-to-several-accounts"></a>Распределение повторяющихся сумм журналов на несколько счетов
В окне **Типовой финансовый журнал** можно выбрать действие **Распределения** для просмотра или управления порядком распределения сумм в строке типового журнала по нескольким счетам и измерениям. Обратите внимание, что функции распределения является строкой балансирующего счета по отношению к строке типового журнала.

Также как в типовом журнале, распределение следует вводить только один раз. Распределение остается в журнале распределения после учета, поэтому не требуется вводить суммы и распределения всякий раз при учете строки типового журнала.

Если метод повторения в типовом журнале определен как **Баланс** или **Сторнирование - баланс**, то программа будет игнорировать любые коды значений измерений в типовом журнале, если счет установлен равным нулю. Поэтому при распределении типовой строки по различным значениям измерений в окне **Распределения**, то будет создана только одна сторнирующая операция. Поэтому, если вы распределяете строку типового журнала, которая содержит код значения измерения, то не следует вводить тот же код в окне **Распределения**. Если сделать это, значения измерений будут неправильными.

####<a name="example-allocating-rent-payments-to-different-departments"></a>Пример. Распределение арендных платежей по различным подразделениям
Вам следует выплачивать арендную плату ежемесячно, поэтому сумма арендной платы вводится на счет кассы в строке типового журнала. В окне **Распределения** можно разделить расходы среди нескольких отделов (измерение отделов) в соответствии с количеством квадратных метров, занимаемых каждым отделом. Расчет основывается на проценте распределения по каждой строке. Можно ввести различные счета в различных строках распределения (если арендная плата тоже будет разделена по нескольким счетам) или можно ввести один и тот же счет, но с различными кодами значения измерения относительно измерения «Отдел» в каждой строке.


## <a name="working-with-standard-journals"></a>Работа со стандартными журналами
Когда созданы строки журнала, которые, возможно, впоследствии придется создавать заново, перед выполнением учета журнала можно сохранить эти строки как стандартный журнал. Эта функция применяется к журналам товаров и финансовым журналам.

> [!NOTE]  
>   описанная ниже процедура относится к журналу товаров, но эти сведения применимы и к финансовому журналу.

### <a name="to-save-a-standard-journal"></a>Сохранение стандартного журнала
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы товаров**, а затем выберите связанную ссылку.
2. Введите одну или несколько строках журнала.
3. Выберите строки журнала, которые нужно использовать повторно.
4. Выберите действие **Сохранить как стандартный журнал**.
5. В окне запроса **Сохранение как стандартный журнал товаров** необходимо определить новый или существующий стандартный журнал товаров, в котором должны быть сохранены выбранные строки:

    Если уже был создан один или несколько стандартных журналов товаров и нужно заменить какой-нибудь из них новым набором строк журнала товаров, можно выбрать в поле Код требуемый код.
6. Нажмите кнопку **ОК**, чтобы подтвердить, что вы хотите перезаписать существующий стандартный журнал товаров и заменить все его содержимое.
7. Выберите поле **Сохранить цену единицы**, если в поле **Цена единицы** нужно сохранять значения стандартного журнала товаров.
8. Выберите поле **Сохранить количество**, если программа должна сохранить значения в поле **Кол-во**.
9. Нажмите кнопку **ОК**, чтобы сохранить стандартный журнал товаров.

После сохранения стандартного журнала товаров на экране появляется окно Журнал товаров, которое позволяет выполнить учет журнала. Следует помнить, что этот журнал может быть легко восстановлен в следующий раз, когда понадобится учесть те же или аналогичные строки.

### <a name="to-reuse-a-standard-journal"></a>Повторное использование стандартного журнала
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журналы товаров**, а затем выберите связанную ссылку.
2. Выберите действие **Получить стандартные журналы**.

    Откроется окно Стандартные журналы товаров, содержащее коды и описания всех имеющихся стандартных журналов товаров.
3. Чтобы просмотреть стандартный журнал товаров перед его повторным использованием, выберите действие **Показать журнал**.

    Любые изменения, внесенные вами в стандартный журнал товаров, реализуются немедленно. Они сохранятся при следующем открытии или повторном использовании этого стандартного журнала товаров. Поэтому необходимо убедиться, что вносимое изменение достаточно важно для применения в общем случае. Если это не так, конкретные изменения в журнал товаров следует вносить после вставки строк стандартного журнала товаров. См. ниже шаг 4.
4. В окне **Стандартные журналы товаров** выберите стандартный журнал товаров, который нужно использовать повторно, и нажмите кнопку **ОК**.

    Строки, сохраненные как стандартный журнал товаров, подставляются в журнале товаров. Если в журнале товаров уже есть строки, то строки из стандартного журнала будут вставлены под существующими строками.

    Если в процессе выполнения функции **Сохранить как стандартный журнал товаров** не был установлен флажок **Сохранить цену единицы**, поле **Цена единицы** для строк, вставленных из стандартного журнала, автоматически заполняется текущим значением товара, скопированным из поля **Себестоимость единицы** карточки товара.

    > [!NOTE]  
    >   Если выбрано поле **Сохранить цену единицы** или **Сохранить количество**, перед выполнением учета журнала товаров нужно убедиться, что вставленные значения правильны для этой конкретной коррекции склада.

    Если вставленные строки журнала товаров содержат сохраненные цены единиц, которые учитывать не нужно, можно быстро исправить их на текущее значение для товара следующим образом.

6. Выберите строки журнала товара, которые требуется откорректировать, а затем выберите действие **Перерасчет цены единицы**. Поле Цена единицы обновится с учетом текущей себестоимости единицы товара.
7. Выберите действие **Учесть**.

## <a name="to-renumber-document-numbers-in-journals"></a>Перенумерация номеров документов в журналах
Чтобы убедиться в отсутствии ошибок учета из-за порядка следования номеров документов, можно использовать функцию **Перенумеровать номера документа** перед выполнением учета журнала.

Во всех журналах, которые основаны на финансовом журнале, поле **Номер документа** имеет возможность редактирования таким образом, чтобы можно было задать различные номера документа для различных строк журнала или того же номера документа для связанных строк журнала.

Если поле **Серии номеров** в разделе журнала заполнено, то функция учета в финансовых журналах требует, чтобы номер документа в индивидуальных или сгруппированных строках был в последовательном порядке. Чтобы убедиться в отсутствии ошибок учета из-за порядка следования номеров документов, можно использовать функцию **Перенумеровать номера документа** перед выполнением учета в журнале. Если соответствующие строки журнала сгруппированы по номеру документа до использования функции, они остаются сгруппированными, при этом им можно присвоить другой номер документа.

Эта функция также работает в отфильтрованных представлениях.

Любая перенумерация номеров документов будет учитывать связанные применения, например применение платежа, выполненное из документа в строке журнала к счету поставщика. Соответственно, могут быть обновлены поля **Код применения** и **Примен. к док. - номер** в затронутых операциях книги.

Следующая процедура основана на окне **Финансовый журнал**, но она применима ко всем другим журналам, которые основаны на финансовом журнале, например окно **Журнал платежей**.

1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Финансовые журналы**, а затем выберите связанную ссылку.
2. Когда вы будете готовы к учету журнала, выберите действие **Перенумеровать документы**.

Значение поля **Номер документа** при необходимости изменяется таким образом, чтобы номера документов в отдельных или сгруппированных строках журнала располагались в последовательном порядке. После того как документы перенумерованы, можно продолжить учет журнала.

## <a name="see-also"></a>См. также
[Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).  
[Сторнирование учета](finance-how-reverse-journal-posting.md)  
[Распределение затрат и дохода](year-allocate-costs-income.md)  
[Финансы](finance.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
