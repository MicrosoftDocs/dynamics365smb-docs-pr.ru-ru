---
title: Синхронизация и интеграция данных | Документация Майкрософт
description: Синхронизация копирует данные между объектами Common Data Service и записями Business Central и поддерживает актуальность данных в обеих системах.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 9d3f4e86a0da5c26a84ca79b1712f2f240e347a2
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922446"
---
# <a name="synchronizing-data-in-business-central-with-common-data-service"></a>Синхронизация данных в Business Central с Common Data Service

При интеграции [!INCLUDE[d365fin](includes/cds_long_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)] можно решить, требуется ли синхронизировать данные в выбранных полях записей [!INCLUDE[d365fin](includes/d365fin_md.md)] (таких как клиенты, контакты и менеджеры по продаже) с эквивалентными записями в [!INCLUDE[d365fin](includes/cds_long_md.md)] (таких как организации, контакты и пользователи). В зависимости от типа записи, можно синхронизировать данные из [!INCLUDE[d365fin](includes/cds_long_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)] или наоборот. Дополнительные сведения см. в разделе [Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Синхронизация использует следующие элементы:

* Сопоставления таблиц интеграции
* Сопоставления полей интеграции
* Правила синхронизации
* Связанные записи

Если синхронизация настроена, можно связать записи [!INCLUDE[d365fin](includes/cds_long_md.md)] с записями [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы синхронизировать их данные. Можно запустить синхронизацию вручную или по расписанию. В следующей таблице приведен обзор способов синхронизации записей.  

|  Тип  |  Метод  |  Ссылка  |  
|--------|----------|-------|  
|Ручная синхронизация|Синхронизируйте запись за записью.<br /><br /> Можно синхронизировать индивидуальные записи в [!INCLUDE[d365fin](includes/d365fin_md.md)], такие как клиент, с соответствующей записью [!INCLUDE[d365fin](includes/cds_long_md.md)], такой как организация. Обычно так пользователи будут работать с данными [!INCLUDE[d365fin](includes/cds_long_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Связывание и синхронизация записей вручную](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Синхронизируйте на основе сопоставления таблиц.<br /><br /> Можно синхронизировать все записи в таблице [!INCLUDE[d365fin](includes/d365fin_md.md)] с объектом [!INCLUDE[d365fin](includes/cds_long_md.md)].|[Синхронизация отдельных сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Синхронизируйте все измененные записи для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все записи, которые были изменены в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] с момента последней синхронизации.|[Синхронизация всех измененных записей](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Полная синхронизации всех данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все данные в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] и объектах [!INCLUDE[d365fin](includes/cds_long_md.md)], которые сопоставлены, и создать новые записи в целевом решении для несвязанных записей в решении-источнике.<br /><br /> Полная синхронизация будет синхронизировать все данные и игнорировать связывание. Обычно полная синхронизация выполняется при настройке интеграции, и только одно из решений содержит данные. Полная синхронизации также может быть полезна в демонстрационной среде.|[Выполнение полной синхронизации](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Синхронизация по расписанию|Синхронизируйте все изменения данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[d365fin](includes/cds_long_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий.|[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

## <a name="standard-entity-mapping-for-synchronization"></a>Сопоставление стандартных объектов для синхронизации
Объекты в [!INCLUDE[d365fin](includes/cds_long_md.md)], например организации, интегрируются с эквивалентными типами объектов в [!INCLUDE[d365fin](includes/d365fin_md.md)], например клиенты. Для работы с данными [!INCLUDE[d365fin](includes/cds_long_md.md)] нужно настроить ссылки, называемые связываниями, между объектами в [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].

В следующей таблице перечислено стандартное соответствие между объектами в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)], которое предоставляет [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!TIP]
> Вы можете сбросить изменения конфигурации, внесенные в таблицу интеграции и сопоставления полей, до значений по умолчанию, выбрав сопоставления, а затем выбрав **Использовать настройку синхронизации по умолчанию**.

| [!INCLUDE[d365fin](includes/d365fin_md.md)] | [!INCLUDE[d365fin](includes/cds_long_md.md)] | Направление синхронизации | Фильтр по умолчанию |
|---------------------------------------------|----------------------------------------------|---------------------------|----------------|
| Менеджер по продажам/закупкам | Пользователь | [!INCLUDE[d365fin](includes/cds_long_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Фильтр контакта [!INCLUDE[d365fin](includes/cds_long_md.md)]: **Состояние** равно **Нет**, **Пользователь лицензирован** — **Да**, режим интеграции пользователя — **Нет** |
| Клиент | Организация | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Фильтр по счетам [!INCLUDE[d365fin](includes/cds_long_md.md)]: **тип связи** — **Клиент** и **статус** **Активно**. Фильтр [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Заблокировано** пустое (Клиент не заблокирован). |
| Поставщик | Организация | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Фильтр по счетам [!INCLUDE[d365fin](includes/cds_long_md.md)]: **тип связи** — **Поставщик** и **статус** **Активно**. Фильтр [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Заблокировано** пустое (Поставщик не заблокирован). |
| Контакт | Контакт | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Фильтр по контактам [!INCLUDE[d365fin](includes/d365fin_md.md)]: **тип** — **Человек** и контакт назначен организации. Фильтр по контактам [!INCLUDE[d365fin](includes/cds_long_md.md)]: контакт назначен организации, родительский тип клиента — **Организация**. |
| Валюта | Валюта транзакции | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[d365fin](includes/cds_long_md.md)] |  |


### <a name="tip-for-admins-viewing-entity-mappings"></a>Совет для администраторов: просмотр сопоставлений объектов
Можно просмотреть сопоставления между объектами в [!INCLUDE[d365fin](includes/cds_long_md.md)] и таблицами в [!INCLUDE[d365fin](includes/d365fin_md.md)] на странице **Сопоставления таблиц интеграции**, гте можно также применять фильтры. Сопоставления определяются между полями в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] и полями в объектах [!INCLUDE[d365fin](includes/cds_long_md.md)] на странице **Сопоставление полей интеграции**, где можно добавить дополнительную логику сопоставления. Например, это может быть полезно в случае необходимости устранить проблему синхронизации.

## <a name="see-also"></a>См. также  
[Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)
