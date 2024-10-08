---
title: Сбор задолженностей
description: 'Узнайте, как напомнить своим клиентам о просроченных платежах. Отправьте выписку по клиенту, сделайте напоминание или отправьте процент-ноту.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.search.keywords: 'payment due, debt, overdue, fee, charge, reminder'
ms.search.form: '6, 25, 440, 443, 448, 452'
ms.date: 07/01/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="collect-outstanding-balances"></a>Сбор задолженностей

Управление расчетами с клиентами включает проверку своевременной оплаты причитающихся сумм. Если у клиентов есть просроченные платежи, можно начать отправлять им **отчеты по клиенту** в качестве напоминания. Кроме того, можно формировать напоминания.

Напоминания используются для уведомления клиентов о просроченных платежах. Также их можно использовать для вычисления финансовых расходов, таких как проценты или сборы, и их включения в напоминания. Используйте процент-ноты для записи в дебет клиентов процентов или сборов без напоминания им о просроченных суммах.

## <a name="statements"></a>Отчеты

Из карточки клиента можно создать выписку, содержащую транзакции этого клиента с вами. Затем вы можете создать PDF-файл и отправить его клиенту. В качестве альтернативы используйте **Отчет по клиенту**, чтобы отправить вашим клиентам обзор их бизнеса вместе с вами. 

> [!TIP]
> При необходимости вы можете отправить выписку в Excel для внесения изменений.  

### <a name="to-send-the-customer-statement-report"></a>Отправка отчета по клиенту.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 10.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Отчет по клиенту**, а затем выберите связанную ссылку.
2. Заполните соответствующим образом поля. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. В поле **Параметры вывода** выберите способ отправки отчета клиенту.

> [!NOTE]
> Если используется несколько валют, то отчет по клиенту всегда печатается в валюте клиента. Последняя дата в периоде отчете также используется как дата отчета и дата срока давности, если в отчет включается срок давности.

## <a name="reminders"></a>Напоминания

[!INCLUDE [receivables-reminders](includes/receivables-reminders.md)]

## <a name="finance-charges"></a>Процент-ноты

Если клиент не платит в установленный срок, вы можете автоматически рассчитать финансовые сборы и добавить их к просроченным суммам на счете клиента. Клиентов можно проинформировать о добавленных процентах путем отправки им процент-нот.  

> [!NOTE]  
> Процент-ноты могут использоваться для вычисления процентов и финансовых расходах, а также информирования о них клиентов без напоминания о просроченных платежах. Процент по просроченным платежам также можно вычислить при создании напоминаний.  

Перед созданием процент-нот необходимо настроить условия. Дополнительные сведения см. в разделе [Настройка процентных ставок](finance-setup-finance-charges.md).  

Можно вручную создать процент-ноту для отдельного клиента и автоматически заполнить строки. Также для создания процент-нот для всех или выбранных клиентов с просроченными задолженностями можно воспользоваться функцией **Создать процент-ноты**.  

После создания процент-нот их можно изменять. Текст, расположенный в начале и в конце процент-ноты, определяется процентными ставками, и его можно просмотреть в столбце **Описание** строк. Если в начале или конце текста автоматически была вставлена рассчитанная сумма, текст не будет скорректирован при удалении строк. В этом случае необходимо воспользоваться функцией **Обновить текст процент-ноты**.  

После создания процент-нот и внесения всех необходимых изменений можно либо напечатать тестовые отчеты, либо произвести учет процент-нот, обычно по электронной почте.

### <a name="to-create-a-finance-charge-memo-manually"></a>Создание процент-ноты вручную

Процент-нота аналогична счету. Можно заполнить заголовок вручную при автоматическом заполнении строк либо создать процент-ноты для всех клиентов автоматически.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 2.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Процент-ноты**, а затем выберите связанную ссылку.  
2. Выберите действие **Создать**, затем введите в поля требуемые данные.  
3. Выберите действие **Предложить строки процент-ноты**.
4. На странице **Предложить строки процент-ноты** настройте фильтр на экспресс-вкладке **Клиент - книга операций**, если требуется создавать процент-ноты только для конкретных операций.

    > [!NOTE]
    > Хотя они перечислены, выбор значений **Оплата** и **Кредит-нота** в фильтре **Тип документа** не будет иметь никакого эффекта, потому что функция **Предложить строки процент-ноты** обрабатывает только положительные суммы.
5. Нажмите кнопку **OK** для запуска пакетного задания.  

### <a name="to-update-finance-charge-memo-texts"></a>Обновление текстов процент-нот

В некоторых случаях вам может потребоваться изменить начальный и конечный текст, который вы настроили для условий финансового платежа. Если это сделать в тот момент, когда создана, но еще не учтена процент-нота, процент-ноты могут быть обновлены с учетом изменения текста.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 3.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Процент-нота**, а затем выберите связанную ссылку.  
2. откройте процент-ноту, в которой нужно изменить текст, а затем выберите действие **Обновить текст процент-ноты**.
3. На странице **Обновить текст процент-ноты** можно настроить фильтр, если требуется обновить несколько процент-нот.
4. Нажмите кнопку **ОК**, чтобы обновить начальный и конечный текст.  

### <a name="to-issue-finance-charge-memos"></a>Выдача процент-нот

После создания процент-нот и внесения всех необходимых изменений можно либо напечатать тестовые отчеты, либо выпустить процент-ноты.

При выпуске напоминания операции учитываются в соответствии со значениями параметров на странице **Процентные ставки**. Эти параметры определяет, учитываются ли проценты и/или дополнительные сборы на счете клиента и в главной книге. Параметры на странице **Учетные группы клиентов** определяют счета, на которых учитываются проценты или сборы.

По каждой учтенной клиентской операции в процент-ноте, создается операция на странице **Операции напоминания/процент-ноты**.

При наличии флажка в поле **Учет процентов** или в поле **Учет дополнительного сбора** страницы **Процентные ставки** также формируются следующие операции:

- одна операция на странице **Клиент - книга операций**;
- одна операция "расчеты с клиентом" на соответствующем счете ГК;
- одна операция "процент" и/или "дополнительная плата" на соответствующем счете ГК.

Кроме того, выпуск процент-ноты может привести к возникновению операций НДС.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать 4.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Процент-ноты**, а затем выберите связанную ссылку.
2. Выберите соответствующую процент-ноту, в затем выберите действие **Выпустить**.
3. На странице **Учет процент-нот** заполните требуемые поля.
4. Нажмите кнопку **ОК**

Финансовый меморандум либо распечатывается, либо отправляется на указанный адрес электронной почты в виде вложения в формате PDF.

### <a name="to-cancel-an-issued-finance-charge-memo"></a>Отмена выпущенной процент-ноты

Если финансовые платежные поручения были выданы по ошибке, вы можете отменить их до того, как они будут отправлены. Вы можете сделать это либо по одному, либо пакетом.

1. На странице **Выпущенные процент-ноты** выберите одну или несколько строк выпущенных процент-нот, которые вы хотите отменить, а затем выберите действие **Отмена**.
2. На странице **Отменить отправленные процент-ноты** заполните поля требуемым образом, а затем выберите кнопку **ОК**.

### <a name="to-view-reminder-and-finance-charge-entries"></a>Просмотр операций напоминаний и процент-нот

При выдаче напоминания на странице **Операции напоминания/процент-ноты** создается операция напоминания для каждой строки напоминания, содержащей операцию книги клиентов. Здесь можно будет просмотреть созданные операции напоминания для определенного клиента.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 5.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Клиенты**, а затем выберите связанную ссылку.  
2. Откройте соответствующую карточку клиента и выберите действие **Книга операций**.
3. На странице **Книга операций по клиентам** выделите строку с операцией книги, для которой требуется просмотреть операции напоминаний, а затем выберите действие **Операции напоминаний/процент-нот**.

## <a name="multiple-interest-rates"></a>Сложные процентные ставки

[!INCLUDE [multiple-interest-rates-def](includes/multiple-interest-rates-def.md)] Дополнительные сведения см. в разделе [Настройка нескольких процентных ставок](finance-how-to-set-up-multiple-interest-rates.md).  

## <a name="see-also"></a>См. также

[Настройка условий и уровней напоминаний](finance-setup-reminders.md)  
[Настройка процентных ставок](finance-setup-finance-charges.md)  
[Управление дебиторской задолженностью](receivables-manage-receivables.md)  
[Продажи](sales-manage-sales.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
