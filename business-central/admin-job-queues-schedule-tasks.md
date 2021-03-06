---
title: Планирование автоматического выполнения работ
description: Запланированные задания обрабатываются очередью работ. Эти работы выполняют отчеты и модули Codeunit. В настройках можно указать однократное или периодически повторяющееся выполнение работы.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 0f586898d65d4e51e48b0c12cf9bf2487d846b1c
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781240"
---
# <a name="use-job-queues-to-schedule-tasks"></a>Использование очередей работ для планирования задач

Очереди работ в [!INCLUDE[prod_short](includes/prod_short.md)] позволяют пользователям планировать и создавать определенные отчеты, а также запускать модули codeunit. В настройках можно указать однократное или периодически повторяющееся выполнение работы. Например, вы можете захотеть запускать отчет **Статистика продаж * менеджера** еженедельно, чтобы отслеживать продажи по продавцам каждую неделю, или вы можете запускать модуль codeunit **Делегировать запросы на утверждение** ежедневно, чтобы предотвратить накопление документов или блокировку рабочего иным образом.

На странице **Операции очереди работ** перечисляются все существующие работы. При добавлении новой записи очереди заданий, которую нужно запланировать, необходимо указать сведения о типе объекта, который должен запускаться, например отчет или кодовая единица,а также имя и код объекта, который необходимо запустить. Можно также добавлять параметры для определения поведения операции очереди заданий. Например, можно добавить параметр, чтобы только отправить учтенные заказы на продажу. У вас должны быть права на запуск указанного отчета или модуля codeunit, в противном случае при выполнении очереди работ будет возвращена ошибка.  
> [!IMPORTANT]  
> Если используется набор прав доступа SUPER, который поставляется с [!INCLUDE[prod_short](includes/prod_short.md)], данный пользователь и другие пользователи имеют права на запуск всех объектов в пределах лицензии. Этого все еще недостаточно для делегированного администратора или пользователей с лицензией на устройство, которые не могут создавать очереди заданий.

Очередь заданий может состоять из большого количества операций, представляющих собой задания, которыми управляет очередь и запускает их. Информация в записи определяет, какой отчет или модуль codeunit выполняется, как часто и когда запускается запись, в какой категории запускается задача и каким образом.  

После того как очереди заданий настроены и работают, статус может изменяться в пределах каждого повторяющегося периода, как указано ниже:

* **На удержании**  
* **Готово**  
* **В работе**  
* **Ошибка**  
* **Завершен**  

После успешного выполнения задания оно будет удалено из списка операций очереди заданий, если только это задание не является повторяющимся. Если это повторяющаяся работа, поле **Самая ранняя дата/время начала** показывает, когда ожидается следующий запуск задания.  

## <a name="to-view-status-or-errors-in-the-job-queue"></a>Просмотр состояния или ошибок в очереди работ

Данные, произведенные при выполнении очереди заданий, хранятся в базе данных, чтобы можно было устранить ошибки очереди работ.  
Для каждой записи очереди заданий вы можете просмотреть и изменить статус. При создании записи очереди работ она будет иметь статус **На удержании**. Можно установить состояние **Готово** и затем вернуть, например, состояние **На удержании**. В противном случае сведения о состоянии обновляются автоматически.

В следующей таблице описываются значения поля **Статус**.

| Статус | Описание |
|--|--|
| Готово | Показывает, что операция очереди работ готова к выполнению. |
| В работе | Показывает, что операция очереди работ не завершена. Это поле обновляется, когда выполняется очередь работ. |
| На удержании | По умолчанию. Отображает статус операции очереди заданий, когда она создается. Выберите действие **Установить статус Готово** для изменения статуса на **Готово**. Выберите действие **Поставить на удержание** или **Приостановить**, чтобы вернуть статус **На удержании**. |
| Ошибка | Показывает, что произошла ошибка. Выберите **Показать ошибку** для просмотра сообщения об ошибке. |
| Завершен | Показывает, что операция очереди работ завершена. |

### <a name="to-view-status-for-any-job"></a>Просмотр статуса любого задания
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Операции очереди работ**, затем выберите соответствующую ссылку.
2. На странице **Операции очереди работ**, выберите запись очереди заданий, затем выберите действие **Операции журнала**.  

> [!TIP]
> В [!INCLUDE [prod_short](includes/prod_short.md)] Online вы также можете просмотреть статус записей очереди заданий, используя Application Insights в Microsoft Azure. Дополнительные сведения см. в разделе [Анализ телеметрии трассировки жизненного цикла очереди заданий](/dynamics365/business-central/dev-itpro/administration/telemetry-job-queue-lifecycle-trace) в справке [!INCLUDE [prod_short](includes/prod_short.md)] для разработчиков и материалах для администрирования.

## <a name="the-my-job-queue-part"></a>Часть "Моя очередь работ"
Часть **Моя очередь работ** в вашем ролевом центре показывает операции очереди заданий, которые вы запустили, но они еще не завершены. По умолчанию часть не видна, поэтому ее следует добавить в ролевой центр. Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).  

В этой части отображается, какие документы с вашим кодом в поле **Код исполнителя** обрабатываются или помещены в очередь, включая те, которые связаны с фоновой обработкой. По этой части можно быстро понять, произошла ли ошибка при учете документа и есть ли ошибки в записи очереди заданий. Эта часть также позволяет отменить учет документа, если он не запущен.

### <a name="to-view-an-error-from-the-my-job-queue-part"></a>Просмотр ошибки из части "Моя очередь работ"
1. Для операции со статусом **Ошибка** выберите действие **Показать ошибку**.
2. Просмотрите сообщение об ошибке и устраните проблему.


## <a name="examples-of-what-can-be-scheduled-using-job-queue"></a>Примеры того, что можно запланировать с помощью очереди заданий

### <a name="schedule-reports"></a>Планирование отчетов

Можно запланировать выполнение отчета или пакетного задания на заданную дату и время. Запланированные отчеты и пакетные задания вводятся в очередь заданий и обрабатываются в запланированное время, как и другие задания. После выбора действия **Отправить** необходимо выбрать вариант **Запланировать**, а затем ввести такую информацию, как принтер, время и дата, а также повторение.  

Дополнительные сведения см. в разделе [Планирование выполнения отчета](ui-work-report.md#ScheduleReport)

### <a name="schedule-synchronization-between-prod_short-and-prod_short"></a>Планирование синхронизации между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)]

Если вы интегрировали [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE[prod_short](includes/cds_long_md.md)], вы можете использовать очередь заданий для планирования, если нужно синхронизировать записи, которые связаны между двумя бизнес-приложениями. В зависимости от направления и правил, которые вы определили для интеграции, задания синхронизации могут также создавать новые записи в целевом приложении, чтобы они соответствовали записям в источнике. Например, если продавец создает новый контакт в [!INCLUDE[crm_md](includes/crm_md.md)], задание синхронизации может создать этот же контакт для связанного продавца в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Планирование синхронизации между Business Central и Dynamics 365 Sales](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md).

### <a name="schedule-the-posting-of-sales-and-purchase-orders"></a>Планирование учета заказов на продажу и покупку

Очереди заданий — это эффективный инструмент для фонового планирования хода бизнес-процессов, например когда несколько пользователей пытаются выполнить учет заказов на продажу, но только один заказ может обрабатываться одновременно.  

Дополнительные сведения см. в разделе [Настройка фонового учета с очередями работ](ui-batch-posting.md#to-set-up-background-posting-with-job-queues)

## <a name="see-also"></a>См. также

[Администрация](admin-setup-and-administration.md)  
[Настройка Business Central](setup.md)  
[Изменение базовых настроек](ui-change-basic-settings.md)  
[Анализ телеметрии трассировки жизненного цикла очереди заданий](/dynamics365/business-central/dev-itpro/administration/telemetry-job-queue-lifecycle-trace)  


[!INCLUDE[footer-include](includes/footer-banner.md)]