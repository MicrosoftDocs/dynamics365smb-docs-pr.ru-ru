---
title: Синхронизация и интеграция данных | Документы Майкрософт
description: Синхронизация копирует данные между записями Dynamics 365 for Sales и записями Business Central и поддерживает актуальность данных в обеих системах.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: e52010384de83d95011cb29a88cad17a5eba817c
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "940300"
---
# <a name="synchronizing-data-in-business-central-and-dynamics-365-for-sales"></a>Синхронизация данных в Business Central и Dynamics 365 for Sales
При интеграции [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)] можно решить, требуется ли синхронизировать данные в выбранных полях записей [!INCLUDE[d365fin](includes/d365fin_md.md)] (таких как клиенты, контакты и менеджеры по продаже) с эквивалентными записями в [!INCLUDE[d365fin](includes/d365fin_md.md)] (таких как организации, контакты и пользователи). В зависимости от типа записи, можно синхронизировать данные из [!INCLUDE[crm_md](includes/crm_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)] или наоборот. Дополнительные сведения см. в разделе [Интеграция с Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md).  

Синхронизация использует следующие элементы:

* Сопоставления таблиц интеграции
* Сопоставления полей интеграции
* Правила синхронизации
* Связанные записи

Если синхронизация настроена, можно связать записи [!INCLUDE[crm_md](includes/crm_md.md)] с записями [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы синхронизировать их данные. Можно запустить синхронизацию вручную или по расписанию. В следующей таблице приведен обзор способов синхронизации записей.  

|  Тип  |  Метод  |  Ссылка  |  
|--------|----------|-------|  
|Ручная синхронизация|Синхронизируйте запись за записью.<br /><br /> Можно синхронизировать индивидуальные записи в [!INCLUDE[d365fin](includes/d365fin_md.md)], такие как клиент, с соответствующей записью [!INCLUDE[crm_md](includes/crm_md.md)], такой как организация. Обычно так пользователи будут работать с данными [!INCLUDE[crm_md](includes/crm_md.md)] в [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Связывание и синхронизация записей вручную](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
|  |Синхронизируйте на основе сопоставления таблиц.<br /><br /> Можно синхронизировать все записи в таблице [!INCLUDE[d365fin](includes/d365fin_md.md)] с объектом [!INCLUDE[crm_md](includes/crm_md.md)].|[Синхронизация отдельных сопоставлений таблиц](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings)|  
||Синхронизируйте все измененные записи для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все записи, которые были изменены в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] с момента последней синхронизации.|[Синхронизация всех измененных записей](admin-manual-synchronization-of-table-mappings.md#synchronizing-all-modified-records)|
||Полная синхронизации всех данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать все данные в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] и объектах [!INCLUDE[crm_md](includes/crm_md.md)], которые сопоставлены, и создать новые записи в целевом решении для несвязанных записей в решении-источнике.<br /><br /> Полная синхронизация будет синхронизировать все данные и игнорировать связывание. Обычно полная синхронизация выполняется при настройке интеграции, и только одно из решений содержит данные. Полная синхронизации также может быть полезна в демонстрационной среде.|[Выполнение полной синхронизации](admin-manual-synchronization-of-table-mappings.md#run-a-full-synchronization)|  
|Синхронизация по расписанию|Синхронизируйте все изменения данных для всех сопоставлений таблиц.<br /><br /> Можно синхронизировать [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] для запланированных интервалов путем настройки заданий в очереди заданий.|[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)|  

## <a name="standard-sales-entity-mapping-for-synchronization"></a>Сопоставление стандартных объектов Sales для синхронизации
Объекты в [!INCLUDE[crm_md](includes/crm_md.md)], например организации, интегрируются с эквивалентными типами объектов в [!INCLUDE[d365fin](includes/d365fin_md.md)], например клиенты. Для работы с данными [!INCLUDE[crm_md](includes/crm_md.md)] нужно настроить ссылки, называемые связываниями, между объектами в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].

В следующей таблице перечислено стандартное соответствие между объектами в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], которое предоставляет [!INCLUDE[d365fin](includes/d365fin_md.md)].

|[!INCLUDE[d365fin](includes/d365fin_md.md)]|[!INCLUDE[crm_md](includes/crm_md.md)]|Направление синхронизации|Фильтр по умолчанию|
|-------------------------------------------|-----|-------------------------|--------------|
|Менеджер по продажам/закупкам|Пользователь|[!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Фильтр контакта Sales: **Состояние** равно **Нет**, **Пользователь лицензирован** — **Да**, режим интеграции пользователя — **Нет**|
|Клиент|Организация|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Фильтр организации Sales: **Тип отношения** — **Клиент**, **Состояние** — **Активно**.|
|Контакт|Контакт|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Фильтр контактов [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Тип** равен **Человек** и контакт назначен компании. Фильтр по контактам Sales: контакт назначен организации, родительский тип клиента — **Организация**.|
|Валюта|Валюта транзакции|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Единица измерения|Группа единиц|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Товар|Продукт|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Тип контактов Sales: **Тип продукта** — **Товарный запас**|
|Ресурс|Продукт|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]|Тип контактов Sales: **Тип продукта** — **Услуги**|
|Ценовая группа клиента|Прайс-лист|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Цена продажи|Прайс-лист на продукцию|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]|Фильтр контактов [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Код продажи** не пустой, **Тип продажи** — **Ценовая группа клиента**|
|Возможность|Возможность|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]| |
|Заголовок счета продажи|Счет|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Строка счета продажи|Продукт счета|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]| |
|Заголовок заказа на продажу|Заказ на продажу|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)]|Фильтр заголовков продаж [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Тип документа** — Заказ, **Статус** — Выпущено|
|Примечания заказа на продажу|Примечания заказа на продажу|[!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)]| |

### <a name="tip-for-admins-viewing-entity-mappings"></a>Совет для администраторов: просмотр сопоставлений объектов
Можно просмотреть сопоставления между объектами в [!INCLUDE[crm_md](includes/crm_md.md)] и таблицами в [!INCLUDE[d365fin](includes/d365fin_md.md)] на странице **Сопоставления таблиц интеграции**, гте можно также применять фильтры. Сопоставления определяются между полями в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] и полями в объектах [!INCLUDE[crm_md](includes/crm_md.md)] на странице **Сопоставление полей интеграции**, где можно добавить дополнительную логику сопоставления. Например, это может быть полезно в случае необходимости устранить проблему синхронизации.

### <a name="tip-for-developers-mapping-fields-in-business-central-to-the-option-sets-in-sales"></a>Совет для разработчиков: сопоставление полей в Business Central наборам параметров в Sales
Если вы разработчик и хотите добавить параметры в наборы параметров в [!INCLUDE[crm_md](includes/crm_md.md)], необходимо знать следующее. В [!INCLUDE[d365fin](includes/d365fin_md.md)] имеются три таблицы, которые сопоставляются полям параметров объекта **Организация** в [!INCLUDE[crm_md](includes/crm_md.md)]. Записи в таблицах, которые не связаны с параметрами в [!INCLUDE[crm_md](includes/crm_md.md)], не будут синхронизированы. Это означает, что поле **Параметр** останется пустым в [!INCLUDE[crm_md](includes/crm_md.md)].

В следующей таблице показаны сопоставления таблиц [!INCLUDE[d365fin](includes/d365fin_md.md)] для поля **Параметр** в объекте **Организация** в [!INCLUDE[crm_md](includes/crm_md.md)].

|Стол|Поле "Параметр" в объекте "Организация"|
|----------------------|-------------------------------------------|
|Условия оплаты|Условия оплаты|
|Метод поставки|Адрес 1: условия перевозки|
|Экспедитор|Адрес 1: метод отгрузки|

### <a name="synchronization-rules"></a>Правила синхронизации
В следующей таблице описаны правила, управляющие синхронизацией между приложениями.

> [!NOTE]  
> Изменения данных в [!INCLUDE[crm_md](includes/crm_md.md)], которые были сделаны в учетной записи пользователя соединения [!INCLUDE[crm_md](includes/crm_md.md)], не синхронизируются. Поэтому рекомендуется не изменять данные при использовании этой учетной записи. Дополнительные сведения см. в разделе [Настройка интеграции с Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md).

|Стол|Правило|
|-----|----|
|Клиенты|Перед синхронизацией клиента с организацией продавец, который назначен для клиента, должен быть связан с пользователем в [!INCLUDE[crm_md](includes/crm_md.md)]. Поэтому когда запускается задание синхронизации "КЛИЕНТЫ — Dynamics 365 for Sales" и оно настроено на создание новых записей, убедитесь, что выполняется синхронизация продавцов с пользователями [!INCLUDE[crm_md](includes/crm_md.md)], прежде чем клиенты синхронизируются с организациями в [!INCLUDE[crm_md](includes/crm_md.md)]. <br /> <br />Задание синхронизации "КЛИЕНТЫ — Dynamics 365 for Sales" синхронизирует только организаций Sales с типом связи "Клиент".|
|Контакты|Только контакты в [!INCLUDE[crm_md](includes/crm_md.md)], которые связаны с организацией, будут созданы в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Значение кода менеджера по продажам определяет владельца связанного объекта в [!INCLUDE[crm_md](includes/crm_md.md)].|
|Валюты|Валюты связываются с валютами транзакций в [!INCLUDE[crm_md](includes/crm_md.md)] на основе кодов ISO. Только валюты со стандартным кодом ISO будут связаны и синхронизированы с валютами транзакций.|
|Единицы измерения|Единицы измерения синхронизируются с группами единиц в [!INCLUDE[crm_md](includes/crm_md.md)]. Для группы единиц может быть задана только одна единица измерения.|
|Товаров|При синхронизации товаров с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически создает прайс-лист в [!INCLUDE[crm_md](includes/crm_md.md)]. Чтобы избежать ошибок синхронизации, не следует изменять данный прайс-лист вручную.|
|Менеджеры по продажам|Менеджеры по продажам связываются с пользователям системы в [!INCLUDE[crm_md](includes/crm_md.md)]. Пользователь должен быть активирован и иметь лицензию, а также не должен быть пользователем интеграции. Обратите внимание, что это первая таблица, которую нужно синхронизировать, так как она используется для клиентов, контактов, возможных сделок и счетов продажи.|
|Ресурсы|Ресурсы синхронизируются с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], имеющими тип "Услуга".|
|Ценовые группы клиентов|Ценовые группы клиентов синхронизируются с прайс-листами Sales.|
|Цены продажи|Цены Sales с типом продажи "Ценовая группа клиента" и определенным кодом продаж, синхронизируются со строками прайс-листов [!INCLUDE[crm_md](includes/crm_md.md)].|
|Возможные сделки|Возможные сделки синхронизируются с возможными сделками [!INCLUDE[crm_md](includes/crm_md.md)]. Значение кода менеджера по продажам определяет владельца связанного объекта в [!INCLUDE[crm_md](includes/crm_md.md)].|
|Учтенные счета продажи|Учтенные счета продажи синхронизируются со счетами продажи. Прежде чем счет можно будет синхронизировать, рекомендуется синхронизировать все остальные объекты, которые могут быть использованы в нем, от менеджеров по продажам до прайс-листов. Значение кода менеджера по продажам в заголовке счета определяет владельца связанного объекта в Sales.|
|Заказы на продажу|Выпущенный заказ на продажу (заголовки) синхронизируются с заказом на продажу. Прежде чем заказ можно будет синхронизировать, рекомендуется синхронизировать все остальные объекты, которые могут быть использованы в нем, от менеджеров по продажам до прайс-листов. Значение кода менеджера по продажам в заголовке заказа определяет владельца связанного объекта в Sales.|  

## <a name="see-also"></a>См. также  
[Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Интеграция с Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)
