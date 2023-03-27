---
title: Синхронизация Business Central и Dataverse
description: Узнайте о синхронизации данных между Business Central и Dataverse.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'sales, crm, integration, sync, synchronize'
ms.date: 06/14/2021
ms.author: bholtorf
---

# Планирование синхронизации между Business Central и Dataverse


Можно синхронизировать [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE[cds_long_md](includes/cds_long_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий. Задания синхронизации выполнят синхронизацию данных в записях [!INCLUDE[prod_short](includes/prod_short.md)] и записях [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые ранее были связаны. Или для записей, которые еще не связаны, в зависимости от направления синхронизации и правил, задания синхронизации могут создать и связать новые записи в целевой системе. 

Имеется несколько заданий синхронизации, которые доступны в готовом виде. Задания выполняются в следующем порядке во избежание зависимостей связывания между таблицами. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).

1. Задание синхронизации "ВАЛЮТА — Common Data Service".
2. Задание синхронизации "ПОСТАВЩИК — Common Data Service".
3. Задание синхронизации "КОНТАКТ — Common Data Service".
4. Задание синхронизации "КЛИЕНТ — Common Data Service".
5. Задание синхронизации "ПРОДАВЦЫ — Common Data Service".

Задания можно просмотреть на странице **Операции очереди работ**. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).

## Операции очереди заданий синхронизации по умолчанию

В следующей таблице описываются задания синхронизации по умолчанию для [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  

| Операция очереди работ | Описание | Направление | Сопоставление таблиц интеграции | Частота синхронизации по умолчанию (мин) | Время бездействия по умолчанию (мин) |
|--|--|--|--|--|--|--|
| Задание синхронизации КОНТАКТ — Common Data Service | Синхронизирует контакты [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с контактами [!INCLUDE[prod_short](includes/prod_short.md)]. | Двунаправленная | КОНТАКТ | 30 | 720 <br>(12 часов) |
| Задание синхронизации ВАЛЮТА — Common Data Service | Синхронизирует валюты транзакций [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с валютами [!INCLUDE[prod_short](includes/prod_short.md)]. | Из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] | ВАЛЮТА | 30 | 720 <br> (12 ч.) |
| Задание синхронизации КЛИЕНТ — Common Data Service | Синхронизирует организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с клиентами [!INCLUDE[prod_short](includes/prod_short.md)]. | Двунаправленная | КЛИЕНТ | 30 | 720<br> (12 ч.) |
| Задание синхронизации "ПОСТАВЩИК — Common Data Service" | Синхронизирует организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с клиентами [!INCLUDE[prod_short](includes/prod_short.md)]. | Двунаправленная | ПОСТАВЩИК | 30 | 720<br> (12 ч.) |
| Задание синхронизации "ПРОДАВЦЫ — Common Data Service" | Синхронизирует продавцов [!INCLUDE[prod_short](includes/prod_short.md)] с пользователями [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. | Из [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в [!INCLUDE[prod_short](includes/prod_short.md)] | ПРОДАВЦЫ | 30 | 1440<br> (24 ч.) |

## Процесс синхронизации

Каждая операция очереди заданий синхронизации использует соответствующее сопоставление таблицы интеграции, задающее таблицу [!INCLUDE[prod_short](includes/prod_short.md)] и таблицу [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые должны быть синхронизированы. Сопоставления таблиц также включают ряд настроек, управляющих записями в таблице [!INCLUDE[prod_short](includes/prod_short.md)] и таблице [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые должны быть синхронизированы.  

Чтобы синхронизировать данные, записи таблицы [!INCLUDE[cds_long_md](includes/cds_long_md.md)] должны быть связаны с записями [!INCLUDE[prod_short](includes/prod_short.md)]. Например, клиент [!INCLUDE[prod_short](includes/prod_short.md)] должен быть связан с организацией [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Связи можно настроить вручную перед выполнением заданий синхронизации или позволить заданиям синхронизации автоматически настроить связи. В следующем списке указан способ синхронизации данных между [!INCLUDE[cds_long_md](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)] при использовании операций очереди заданий синхронизации. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md).

- Флажок **Синхр. только связанные записи** флажок контролирует, создаются ли новые записи при синхронизации. По умолчанию флажок установлен, что означает, что будут синхронизированы только связанные записи. При сопоставлении таблицы интеграции можно изменить сопоставление таблицы между таблицей [!INCLUDE[cds_long_md](includes/cds_long_md.md)] и таблицей [!INCLUDE[prod_short](includes/prod_short.md)], чтобы задания синхронизации интеграции создавали новые записи в целевой базе данных для каждой строки в исходной базе, которая не связана. Дополнительные сведения см. в разделе [Создание новых записей](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).

    **Пример** Если вы снимите флажок **Синхр. только связанные записи**, то при синхронизации клиентов в [!INCLUDE[prod_short](includes/prod_short.md)] с организациями в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] для каждого клиента в [!INCLUDE[prod_short](includes/prod_short.md)] создается и автоматически связывается новая организация. Кроме того, поскольку синхронизация в этом случае является двунаправленной, новый клиент создается и связывается для каждой организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которая еще не связана.  

    > [!NOTE]  
    > Имеются правила и фильтры, которые определяют, какие данные синхронизируются. Для получения дополнительной информации см. [Правила синхронизации](admin-synchronizing-business-central-and-sales.md).

- Когда новые записи создаются в [!INCLUDE[prod_short](includes/prod_short.md)], записи используют шаблон, определенный для сопоставления таблиц интеграции, или шаблон по умолчанию, доступный для этого типа строки. Поля заполняются данными из [!INCLUDE[prod_short](includes/prod_short.md)] или [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в зависимости от направления синхронизации. Дополнительные сведения см. в разделе [Изменение сопоставлений таблицы для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md).  

- При последующих синхронизациях обновляются только те записи, которые были изменены или добавлены после последнего успешного задания синхронизации для таблицы.  

     Новые записи в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] добавляются в [!INCLUDE[prod_short](includes/prod_short.md)]. Если данные в полях в записях [!INCLUDE[cds_long_md](includes/cds_long_md.md)] изменены, данные копируются в соответствующее поле в [!INCLUDE[prod_short](includes/prod_short.md)].  

- При двунаправленной синхронизации задание выполняет синхронизацию из [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[cds_long_md](includes/cds_long_md.md)], а затем из [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в [!INCLUDE[prod_short](includes/prod_short.md)].

## О таймаутах неактивности
Некоторые операции очереди работ, например те, которые планируют синхронизацию между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[cds_long_md](includes/cds_long_md.md)], используют поле **Таймаут неактивности** на странице операции очереди работ, чтобы предотвратить ненужный запуск очереди работ.  

:::image type="content" source="media/on-hold-with-inactivity-timeout.png" alt-text="Блок-схема, когда операции очереди работ приостанавливаются из-за неактивности.":::

Если значение в этом поле не равно нулю и очередь заданий не обнаружила изменений во время последнего запуска, [!INCLUDE[prod_short](includes/prod_short.md)] приостанавливает операцию очереди работ. Когда это происходит, поле **Статус очереди работ** содержит значение **На удержании из-за неактивности**, а [!INCLUDE[prod_short](includes/prod_short.md)] ждет в течение периода времени, указанного в поле **Таймаут неактивности**, после чего снова запускает очередь работ.  

Например, по умолчанию операция очереди работ CURRENCY, которая синхронизирует валюты в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с обменными курсами в [!INCLUDE[prod_short](includes/prod_short.md)], будет искать изменения обменных курсов каждые 30 минут. Если никаких изменений не найдено, [!INCLUDE[prod_short](includes/prod_short.md)] переводит операцию очереди работу CURRENCY на удержание на 720 минут (двенадцать часов). Если обменный курс изменяется в [!INCLUDE[prod_short](includes/prod_short.md)], пока операция очереди работ находится на удержании, [!INCLUDE[prod_short](includes/prod_short.md)] автоматически заново активирует операцию очереди работ и перезапускает очередь работ. 

> [!Note]
> [!INCLUDE[prod_short](includes/prod_short.md)] автоматически активирует операции очереди работ, которые находятся на удержании только тогда, когда в [!INCLUDE[prod_short](includes/prod_short.md)] происходят изменения. Изменения в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] не активируют операции очереди работ.

## Просмотр журнала заданий синхронизации

1. Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Журнал синхронизации интеграции**, а затем выберите связанную ссылку.
2. Если при выполнении задания синхронизации произошла одна или несколько ошибок, количество ошибок отображается в столбце **Ошибки**. Для просмотра ошибок по заданию выберите номер.  

    > [!TIP]  
    > Можно просмотреть все ошибки задания синхронизации, открыв журнал ошибок задания синхронизации вручную.

## Просмотр журнала заданий синхронизации из сопоставлений таблиц

1. Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Сопоставления таблиц интеграции**, а затем выберите связанную ссылку.
2. На странице **Сопоставления таблиц интеграции** выберите запись, затем выберите **Журнал заданий синхронизации интеграции**.  

## Просмотр журнала ошибок синхронизации

- Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Ошибки синхронизации интеграции**, а затем выберите связанную ссылку.

## См. также

[Синхронизация данных в Business Central и [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Ручная синхронизация сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md)  
[Планирование синхронизации между Business Central и [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
[Об интеграции Dynamics 365 Business Central с [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
