---
title: Синхронизация и интеграция данных | Документация Майкрософт
description: Синхронизация копирует данные между таблицами Microsoft Dataverse и записями Business Central и поддерживает актуальность данных в обеих системах.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'Dataverse, integration, sync, synchronize, mapping'
ms.date: 06/14/2021
ms.author: bholtorf
---

# <a name="synchronizing-data-in-business-central-with-microsoft-dataverse" />Синхронизация данных в Business Central с Microsoft Dataverse


При интеграции [!INCLUDE[prod_short](includes/cds_long_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)] можно решить, требуется ли синхронизировать данные в выбранных полях [!INCLUDE[prod_short](includes/prod_short.md)] (таких как клиенты, контакты и менеджеры по продаже) с эквивалентными строками в [!INCLUDE[prod_short](includes/cds_long_md.md)] (таких как организации, контакты и пользователи). В зависимости от типа строки, можно синхронизировать данные из [!INCLUDE[prod_short](includes/cds_long_md.md)] в [!INCLUDE[prod_short](includes/prod_short.md)] или наоборот. Дополнительные сведения см. в разделе [Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Синхронизация использует следующие элементы:

* Сопоставления таблиц интеграции
* Сопоставления полей интеграции
* Правила синхронизации
* Связанные записи

Если синхронизация настроена, можно связать записи [!INCLUDE[prod_short](includes/cds_long_md.md)] со строками [!INCLUDE[prod_short](includes/prod_short.md)], чтобы синхронизировать их данные. Можно запустить синхронизацию вручную или по расписанию. В следующей таблице приведен обзор способов синхронизации.  

|  Тип  |  Метод  |  Ссылка  |  
|--------|----------|-------|  
|Ручная синхронизация|Синхронизируйте строку за строкой.<br /><br /> Можно синхронизировать индивидуальные записи в [!INCLUDE[prod_short](includes/prod_short.md)], такие как клиент, с соответствующей строкой [!INCLUDE[prod_short](includes/cds_long_md.md)], такой как организация. Обычно так пользователи будут работать с данными [!INCLUDE[prod_short](includes/cds_long_md.md)] в [!INCLUDE[prod_short](includes/prod_short.md)].|[Связывание и синхронизация записей вручную](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Синхронизируйте на основе сопоставления таблиц.<br /><br /> Можно синхронизировать все записи в таблице [!INCLUDE[prod_short](includes/prod_short.md)] с таблицей [!INCLUDE[prod_short](includes/cds_long_md.md)].|[Синхронизация отдельных сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Синхронизируйте все измененные записи для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все записи, которые были изменены в таблицах [!INCLUDE[prod_short](includes/prod_short.md)] с момента последней синхронизации.|[Синхронизация всех измененных записей](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Полная синхронизации всех данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все данные в таблицах [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)], которые сопоставлены, и создать новые записи или строки в целевом решении для несвязанных записей в решении-источнике.<br /><br /> Полная синхронизация будет синхронизировать все данные и игнорировать связывание. Обычно полная синхронизация выполняется при настройке интеграции, и только одно из решений содержит данные. Полная синхронизации также может быть полезна в демонстрационной среде.|[Выполнение полной синхронизации](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Синхронизация по расписанию|Синхронизируйте все изменения данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE[prod_short](includes/cds_long_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий.|[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

> [!NOTE]
> Синхронизация между [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)] основана на запланированном выполнении записей очереди заданий и не гарантирует согласованность данных в реальном времени между двумя службами. Для согласованности данных в реальном времени вам следует изучить [Виртуальные таблицы Business Central](/dynamics365/business-central/dev-itpro/powerplatform/powerplat-overview) или API Business Central.   


## <a name="standard-table-mapping-for-synchronization" />Сопоставление стандартных таблиц для синхронизации
Таблицы в [!INCLUDE[prod_short](includes/cds_long_md.md)], например организации, интегрируются с эквивалентными типами таблиц в [!INCLUDE[prod_short](includes/prod_short.md)], например клиенты. Для работы с данными [!INCLUDE[prod_short](includes/cds_long_md.md)] нужно настроить ссылки, называемые связываниями, между таблицами в [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)].

В следующей таблице перечислено стандартное соответствие между таблицами в [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)].

> [!TIP]
> Вы можете сбросить изменения конфигурации, внесенные в таблицу интеграции и сопоставления полей, до значений по умолчанию, выбрав сопоставления, а затем выбрав **Использовать настройку синхронизации по умолчанию**.

| [!INCLUDE[prod_short](includes/prod_short.md)] | [!INCLUDE[prod_short](includes/cds_long_md.md)] | Направление синхронизации | Фильтр по умолчанию |
|---------------------------------------------|----------------------------------------------|---------------------------|----------------|
| Менеджер по продажам/закупкам | Пользователь | [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Фильтр контакта [!INCLUDE[prod_short](includes/cds_long_md.md)]: **Состояние** равно **Нет**, **Пользователь лицензирован** — **Да**, режим интеграции пользователя — **Нет** |
| Клиент | Организация | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Фильтр по счетам [!INCLUDE[prod_short](includes/cds_long_md.md)]: **тип связи** — **Клиент** и **статус** **Активно**. Фильтр [!INCLUDE[prod_short](includes/prod_short.md)]: **Заблокировано** пустое (Клиент не заблокирован). |
| Поставщик | Организация | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Фильтр по счетам [!INCLUDE[prod_short](includes/cds_long_md.md)]: **тип связи** — **Поставщик** и **статус** **Активно**. Фильтр [!INCLUDE[prod_short](includes/prod_short.md)]: **Заблокировано** пустое (Поставщик не заблокирован). |
| Контакт | Контакт | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)] -> [!INCLUDE[prod_short](includes/prod_short.md)] | Фильтр по контактам [!INCLUDE[prod_short](includes/prod_short.md)]: **тип** — **Человек** и контакт назначен организации. Фильтр по контактам [!INCLUDE[prod_short](includes/cds_long_md.md)]: контакт назначен организации, родительский тип клиента — **Клиент**. |
| Валюта | Валюта транзакции | [!INCLUDE[prod_short](includes/prod_short.md)] -> [!INCLUDE[prod_short](includes/cds_long_md.md)] |  |

> [!NOTE]
> Действия **Dataverse** не будут доступны на страницах, например, на странице "Карточка клиента", для записей, которые не соблюдают фильтр таблицы в сопоставлении таблицы интеграции.

### <a name="tip-for-admins-viewing-table-mappings" />Совет для администраторов: просмотр сопоставлений таблиц
Можно просмотреть сопоставления между таблицами в [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)] на странице **Сопоставления таблиц интеграции**, где можно также применять фильтры. Сопоставления определяются между полями в таблицах [!INCLUDE[prod_short](includes/prod_short.md)] и столбцами в таблицах [!INCLUDE[prod_short](includes/cds_long_md.md)] на странице **Сопоставление полей интеграции**, где можно добавить дополнительную логику сопоставления. Например, это может быть полезно в случае необходимости устранить проблему синхронизации.

## <a name="see-also" />См. также
[Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
