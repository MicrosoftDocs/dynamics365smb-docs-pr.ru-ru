---
title: Синхронизация Business Central и Common Data Service | Документы Майкрософт
description: Узнайте о синхронизации данных между Business Central и Common Data Service.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 2f1b79cdf04075159b5e464e384bace89d9f933c
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917805"
---
# <a name="scheduling-a-synchronization-between-business-central-and-common-data-service"></a>Планирование синхронизации между Business Central и Common Data Service

Можно синхронизировать [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[cds_long_md](includes/cds_long_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий. Задания синхронизации выполнят синхронизацию данных в записях [!INCLUDE[d365fin](includes/d365fin_md.md)] и записях [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые ранее были связаны. Или для записей, которые еще не связаны, в зависимости от направления синхронизации и правил, задания синхронизации могут создать и связать новые записи в целевой системе. 

Имеется несколько заданий синхронизации, которые доступны в готовом виде. Задания выполняются в следующем порядке во избежание зависимостей связывания между объектами. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](/dynamics365/business-central/admin-job-queues-schedule-tasks.md).

1. Задание синхронизации "ВАЛЮТА — Common Data Service".
2. Задание синхронизации "ПОСТАВЩИК — Common Data Service".
3. Задание синхронизации "КОНТАКТ — Common Data Service".
4. Задание синхронизации "КЛИЕНТ — Common Data Service".
5. Задание синхронизации "ПРОДАВЦЫ — Common Data Service".

Задания можно просмотреть на странице **Операции очереди работ**. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md).

## <a name="default-synchronization-job-queue-entries"></a>Операции очереди заданий синхронизации по умолчанию

В следующей таблице описываются задания синхронизации по умолчанию для [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  

| Операция очереди работ | Описание | Направление | Сопоставление таблиц интеграции | Частота синхронизации по умолчанию (мин) | Время бездействия по умолчанию (мин) |
|--|--|--|--|--|--|--|
| Задание синхронизации КОНТАКТ — Common Data Service | Синхронизирует контакты [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с контактами [!INCLUDE[d365fin](includes/d365fin_md.md)]. | Двунаправленная | КОНТАКТ | 30 | 720 <br>(12 часов) |
| Задание синхронизации ВАЛЮТА — Common Data Service | Синхронизирует валюты транзакций [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с валютами [!INCLUDE[d365fin](includes/d365fin_md.md)]. | Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] | ВАЛЮТА | 30 | 720 <br> (12 ч.) |
| Задание синхронизации КЛИЕНТ — Common Data Service | Синхронизирует организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с клиентами [!INCLUDE[d365fin](includes/d365fin_md.md)]. | Двунаправленная | КЛИЕНТ | 30 | 720<br> (12 ч.) |
| Задание синхронизации "ПОСТАВЩИК — Common Data Service" | Синхронизирует организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с клиентами [!INCLUDE[d365fin](includes/d365fin_md.md)]. | Двунаправленная | ПОСТАВЩИК | 30 | 720<br> (12 ч.) |
| Задание синхронизации "ПРОДАВЦЫ — Common Data Service" | Синхронизирует продавцов [!INCLUDE[d365fin](includes/d365fin_md.md)] с пользователями [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. | Из [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)] | ПРОДАВЦЫ | 30 | 1440<br> (24 ч.) |

## <a name="synchronization-process"></a>Процесс синхронизации

Каждая операция очереди заданий синхронизации использует соответствующее сопоставление таблицы интеграции, задающее таблицу [!INCLUDE[d365fin](includes/d365fin_md.md)] и объект [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые должны быть синхронизированы. Сопоставления таблиц также включают ряд настроек, управляющих записями в таблице [!INCLUDE[d365fin](includes/d365fin_md.md)] и объекте [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которые должны быть синхронизированы.  

Чтобы синхронизировать данные, записи объекта [!INCLUDE[cds_long_md](includes/cds_long_md.md)] должны быть связаны с записями [!INCLUDE[d365fin](includes/d365fin_md.md)]. Например, клиент [!INCLUDE[d365fin](includes/d365fin_md.md)] должен быть связан с организацией [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Связи можно настроить вручную перед выполнением заданий синхронизации или позволить заданиям синхронизации автоматически настроить связи. В следующем списке указан способ синхронизации данных между Common Data Service и [!INCLUDE[d365fin](includes/d365fin_md.md)] при использовании операций очереди заданий синхронизации. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md).

- Флажок **Синхр. только связанные записи** флажок контролирует, создаются ли новые записи при синхронизации. По умолчанию флажок установлен, что означает, что будут синхронизированы только связанные записи. При сопоставлении таблицы интеграции можно изменить сопоставление таблицы между операцией [!INCLUDE[cds_long_md](includes/cds_long_md.md)] и таблицей [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы задания синхронизации интеграции создавали новые записи в целевой базе данных для каждой записи в исходной базе, которая не связана. Дополнительные сведения см. в разделе [Создание новых записей](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).

    **Пример** Если вы снимите флажок **Синхр. только связанные записи**, то при синхронизации клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] с организациями в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] для каждого клиента в [!INCLUDE[d365fin](includes/d365fin_md.md)] создается и автоматически связывается новая организация. Кроме того, поскольку синхронизация в этом случае является двунаправленной, новый клиент создается и связывается для каждой организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)], которая еще не связана.  

    > [!NOTE]  
    > Имеются правила и фильтры, которые определяют, какие данные синхронизируются. Для получения дополнительной информации см. [Правила синхронизации](admin-synchronizing-business-central-and-sales.md).

- Когда новые записи создаются в [!INCLUDE[d365fin](includes/d365fin_md.md)], записи используют шаблон, определенный для сопоставления таблиц интеграции, или шаблон по умолчанию, доступный для этого типа записей. Поля заполняются данными из [!INCLUDE[d365fin](includes/d365fin_md.md)] или [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в зависимости от направления синхронизации. Дополнительные сведения см. в разделе [Изменение сопоставлений таблицы для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md).  

- При последующих синхронизациях обновляются только те записи, которые были изменены или добавлены после последнего успешного задания синхронизации.  

     Новые записи в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] добавляются в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если данные в полях в записях [!INCLUDE[cds_long_md](includes/cds_long_md.md)] изменены, данные копируются в соответствующее поле в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

- При двунаправленной синхронизации задание выполняет синхронизацию из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[cds_long_md](includes/cds_long_md.md)], а затем из [!INCLUDE[cds_long_md](includes/cds_long_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="about-inactivity-timeouts"></a>О таймаутах неактивности

Некоторые операции очереди работ, например те, которые планируют синхронизацию между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[cds_long_md](includes/cds_long_md.md)], используют поле **Таймаут неактивности** карточки операции очереди работ, чтобы предотвратить ненужный запуск очереди работ.  

:::image type="content" source="media/on-hold-with-inactivity-timeout.png" alt-text="Блок-схема, когда операции очереди работ приостанавливаются из-за неактивности.":::

Если значение в этом поле не равно нулю и очередь заданий не обнаружила изменений во время последнего запуска, [!INCLUDE[d365fin](includes/d365fin_md.md)] приостанавливает операцию очереди работ. Когда это происходит, поле **Статус очереди работ** содержит значение **На удержании из-за неактивности**, а [!INCLUDE[d365fin](includes/d365fin_md.md)] ждет в течение периода времени, указанного в поле **Таймаут неактивности**, после чего снова запускает очередь работ.  

Например, по умолчанию операция очереди работ CURRENCY, которая синхронизирует валюты в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] с обменными курсами в [!INCLUDE[d365fin](includes/d365fin_md.md)], будет искать изменения обменных курсов каждые 30 минут. Если никаких изменений не найдено, [!INCLUDE[d365fin](includes/d365fin_md.md)] переводит операцию очереди работу CURRENCY на удержание на 720 минут (шесть часов). Если обменный курс изменяется в [!INCLUDE[d365fin](includes/d365fin_md.md)], пока операция очереди работ находится на удержании, [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически заново активирует операцию очереди работ и перезапускает очередь работ. 

> [!Note]
> [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически активирует операции очереди работ, которые находятся на удержании только тогда, когда в [!INCLUDE[d365fin](includes/d365fin_md.md)] происходят изменения. Изменения в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] не активируют операции очереди работ.

## <a name="to-view-the-synchronization-job-log"></a>Просмотр журнала заданий синхронизации

1. Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Журнал синхронизации интеграции**, а затем выберите связанную ссылку.
2. Если при выполнении задания синхронизации произошла одна или несколько ошибок, количество ошибок отображается в столбце **Ошибки**. Для просмотра ошибок по заданию выберите номер.  

    > [!TIP]  
    > Можно просмотреть все ошибки задания синхронизации, открыв журнал ошибок задания синхронизации вручную.

## <a name="to-view-the-synchronization-job-log-from-the-table-mappings"></a>Просмотр журнала заданий синхронизации из сопоставлений таблиц

1. Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Сопоставления таблиц интеграции**, а затем выберите связанную ссылку.
2. На странице **Сопоставления таблиц интеграции** выберите запись, затем выберите **Журнал заданий синхронизации интеграции**.  

## <a name="to-view-the-synchronization-error-log"></a>Просмотр журнала ошибок синхронизации

- Выберите значок :::image type="icon" source="media/ui-search/search_small.png" border="false":::, введите **Ошибки синхронизации интеграции**, а затем выберите связанную ссылку.

## <a name="see-also"></a>См. также

[Синхронизация данных в Business Central и [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Ручная синхронизация сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md)  
[Планирование синхронизации между Business Central и [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
[Об интеграции Dynamics 365 Business Central с [!INCLUDE[cds_long_md](includes/cds_long_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md)  
