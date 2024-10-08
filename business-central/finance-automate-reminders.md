---
title: Автоматизация напоминаний при сборе задолженностей
description: 'Как сэкономить время при сборе задолженностей за счет автоматизации процессов создания, выпуска и отправки напоминаний клиентам.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.search.keywords: 'collection, remindes'
ms.search.form: null
ms.date: 03/12/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="automate-reminders-in-collections"></a>Автоматизация напоминаний при сборе задолженностей

Увеличьте эффективность сбора задолженностей за счет автоматизации процесса создания, выпуска и отправки напоминаний вашим клиентам. Автоматизация может значительно сократить время, которое вы потратите на сбор задолженностей, повысить прозрачность процесса и дать вам возможность полностью контролировать каждый его этап.

На странице **Автоматизация напоминаний** вы определяете отдельные действия (шаги). Вы можете объединить шаги по созданию, выпуску и отправке напоминаний или создать отдельную автоматизацию для каждого шага, если это больше подходит для ваших процессов сбора задолженностей. Автоматизации основаны на условиях напоминания и уровнях напоминания. Чтобы узнать больше, перейдите в раздел [Настройка условий и уровней напоминаний](finance-setup-reminders.md). Вы можете установить фильтры для условий напоминаний для автоматизации в целом, а также установить фильтры для каждого действия в автоматизации. Вы также можете прикреплять неоплаченные счета к электронным письмам в виде PDF-файлов.

Автоматизация происходит через запись в очереди заданий. При настройке автоматизации используйте поле **Периодичность**, чтобы указать, как и когда она запускается. Если вы выберете **Вручную**, автоматизация запустится один раз при использовании действия **Запустить**. Вы также можете выбрать **Еженедельно**, **Ежемесячно** или **Пользовательский**, чтобы настроить более детальную периодичность. Если вы выберете **Пользовательский**, вам потребуется ввести формулу даты. Чтобы узнать больше о вводе формулы даты, перейдите в раздел [Использование формул даты](ui-enter-date-ranges.md#use-date-formulas). Если вы выберете вариант, отличный от **Вручную**, автоматизация будет работать до тех пор, пока вы не приостановите ее. Если вы хотите уточнить время запуска, используйте действие **Записи очереди заданий**, чтобы открыть страницу **Записи очереди заданий**, и настройте периодичность, например, ежедневно или определенный день недели.

## <a name="automate-the-reminders-flow"></a>Автоматизация потока напоминаний

В следующих разделах описывается, как настроить автоматическое создание, выпуск и отправку напоминаний.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Автоматизация напоминаний**, затем выберите связанную ссылку.
1. Выберите **Создать**, затем требуемым образом заполните поля на экспресс-вкладке **Общее**.
1. В поле **Фильтр условий напоминания** выберите условие или условия напоминания, для которых будет использоваться эта автоматизация.
1. В поле **Периодичность** выберите частоту запуска автоматизации.
1. На экспресс-вкладке **Действия** выберите **Создать**, затем выберите, будет ли система автоматизации создавать, выпускать или отправлять напоминания. Выберите **ОК**.
1. В зависимости от типа действия, которое выполняет автоматика, заполните необходимые поля на странице настройки. Чтобы узнать больше о настройках, перейдите в раздел [Настройки действий напоминаний](#settings-for-reminder-actions).
1. После настройки действий для автоматизации вы можете использовать действия **Переместить вверх** и **Переместить вниз** для настройки порядка, в котором они выполняются.

## <a name="settings-for-reminder-actions"></a>Настройки действий напоминаний

Параметры настройки для действий «Создать», «Выпустить» и «Отправить напоминание» различаются. В следующих разделах описано, как их использовать.

### <a name="create"></a>Создать

* Установите наивысший уровень во всех строках напоминаний.  
* Создайте напоминания для операций, находящихся на удержании. Например, этот параметр полезен, если у вас продолжается спор с клиентом и вы хотите, чтобы он увидел общую картину.
* Создавайте напоминания обо всех неоплаченных счетах, а не только о просроченных. В отчете в отдельных разделах отображаются просроченные счета и те, которые просто не оплачены, но не просрочены.
* Установите фильтры, чтобы сделать напоминание более конкретным.

### <a name="issue"></a>Выпустить

При выпуске напоминания в книге учета клиентов создаются записи, содержащие дату проводки и дату налогообложения. Используйте настройки на странице **Настройка выпуска напоминаний**, чтобы указать, следует ли заменять эту информацию в выпущенном напоминании информацией из созданного напоминания. Например, если вы создали напоминание вчера и выпустили его сегодня, срок выполнения сдвигается на один день.

### <a name="send"></a>Отправить

> [!NOTE]
> Автоматизация отправки требует, чтобы вы настроили адрес электронной почты в [!INCLUDE [prod_short](includes/prod_short.md)]. Чтобы узнать больше о настройке адреса электронной почты, перейдите в раздел [Настройка электронной почты](admin-how-setup-email.md).

Содержимое электронных писем, такое как тексты вложений, основной текст электронного письма и язык, определяется настройками условий напоминания. Чтобы узнать больше о настройках адреса электронной почты, перейдите в раздел [Настройка условий и уровней напоминаний](finance-setup-reminders.md).

Используйте настройки на странице **Настройка отправки напоминаний** для управления следующим:

* Общие параметры, такие как описание и количество отправок одного и того же напоминания.
* Настройки того, что включать в напоминание.
* Настройки для отслеживания напоминаний, которые вы отправляете путем создания взаимодействий, независимо от того, распечатываете ли вы напоминание или отправляете его по электронной почте, а также хотите ли вы прикреплять только просроченные счета, все счета или не прикреплять счета. 

## <a name="access-the-history-of-a-reminder"></a>Доступ к истории напоминания

[!INCLUDE [prod_short](includes/prod_short.md)] отслеживает каждый раз, когда запускается автоматизация. Вы можете получить доступ к истории, выбрав действие **Записи журнала**. Вы также можете использовать действие **Выпущенные напоминания**, чтобы получить доступ к списку отправленных вами напоминаний.

## <a name="handle-errors"></a>Обработка ошибок

На экспресс-вкладке **Действия** для каждого действия вы можете указать, хотите ли вы, чтобы автоматизация останавливалась, если в действии возникла ошибка. Если да, автоматизация не будет обрабатывать последующие действия. Чтобы включить или отключить эту функцию, используйте действия **Установить остановку при ошибке** или **Снять остановку при ошибке**.

## <a name="change-action-settings-for-an-automation"></a>Изменение настроек действий для автоматизации

Вы можете изменить настройки автоматизации в любое время. На экспресс-вкладке **Действия** выберите **Настройка**, затем внесите изменения.

## <a name="see-also"></a>См. также

[Настройка условий и уровней напоминаний](finance-setup-reminders.md)  
[Отправка напоминаний о задолженностях](receivables-send-reminders.md)  
