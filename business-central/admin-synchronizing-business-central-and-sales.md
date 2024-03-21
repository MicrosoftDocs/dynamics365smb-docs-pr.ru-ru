---
title: Синхронизация и интеграция данных | Документация Майкрософт
description: Синхронизация копирует данные между таблицами Microsoft Dataverse и записями Business Central и поддерживает актуальность данных в обеих системах.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: ivkoleti
ms.topic: conceptual
ms.date: 03/31/2023
ms.custom: bap-template
ms.search.keywords: 'Dataverse, integration, sync, synchronize, mapping'
ms.service: dynamics-365-business-central
---

# <a name="synchronizing-data-in-business-central-with-microsoft-dataverse"></a>Синхронизация данных в Business Central с Microsoft Dataverse

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

## <a name="standard-table-mapping-for-synchronization"></a>Сопоставление стандартных таблиц для синхронизации

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

### <a name="tip-for-admins-viewing-table-mappings"></a>Совет для администраторов: просмотр сопоставлений таблиц

Можно просмотреть сопоставления между таблицами в [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)] на странице **Сопоставления таблиц интеграции**, где можно также применять фильтры. Сопоставления определяются между полями в таблицах [!INCLUDE[prod_short](includes/prod_short.md)] и столбцами в таблицах [!INCLUDE[prod_short](includes/cds_long_md.md)] на странице **Сопоставление полей интеграции**, где можно добавить дополнительную логику сопоставления. Например, это может быть полезно в случае необходимости устранить проблему синхронизации.

## <a name="use-virtual-tables-to-get-more-data"></a>Использование виртуальных таблиц для получения дополнительных данных

При настройке интеграции вы можете использовать виртуальные таблицы, чтобы сделать больше данных доступными в [!INCLUDE[prod_short](includes/cds_long_md.md)] — не прибегая к помощи разработчика.

Виртуальная таблица — это пользовательская таблица со столбцами и строками, которые содержат данные из внешнего источника данных, такого как [!INCLUDE [prod_short](includes/prod_short.md)]. Столбцы и строки в виртуальной таблице выглядят как обычная таблица, однако данные не хранятся в физической таблице в базе данных [!INCLUDE[prod_short](includes/cds_long_md.md)]. Вместо этого данные извлекаются во время выполнения.

> [!NOTE]
> [!INCLUDE [prod_short](includes/prod_short.md)] содержит объекты, которые также называются виртуальными таблицами. Эти объекты-таблицы не связаны с виртуальными таблицами, которые вы используете с [!INCLUDE[prod_short](includes/cds_long_md.md)].

Подробнее о виртуальных таблицах можно узнать из следующих статей:

* [Создание и изменение виртуальных таблиц, содержащих данные из внешнего источника данных](/power-apps/maker/data-platform/create-edit-virtual-entities) (документация по Power Apps)
* [Справочника администратора по виртуальным таблицам Business Central для Microsoft Dataverse](/business-central/dev-itpro/powerplatform/powerplat-admin-reference) (документация по [!INCLUDE [prod_short](includes/prod_short.md)])

Чтобы использовать виртуальные таблицы, необходимо установить приложение **Виртуальная сущность Business Central** из [AppSource](https://appsource.microsoft.com/en-US/product/dynamics-365/microsoftdynsmb.businesscentral_virtualentity). 

После установки приложения вы можете включить виртуальные таблицы на одной из следующих страниц в [!INCLUDE [prod_short](includes/prod_short.md)]:

* При использовании мастера настройки **Настройка подключения к Dataverse** вы можете выбрать несколько виртуальных таблиц на странице **Доступные виртуальные таблицы — Dataverse**. После этого эти таблицы будут доступны в [!INCLUDE[prod_short](includes/cds_long_md.md)] и на PowerApps Maker Portal. 
* На страницах **Настройка подключения к Dataverse**, **Виртуальные таблицы** и **Доступные виртуальные таблицы**.  
* На Power App Maker Portal.

## <a name="synchronize-data-from-multiple-companies-or-environments"></a>Синхронизация данных из нескольких организаций или сред

Вы можете синхронизировать данные из нескольких организаций [!INCLUDE [prod_short](includes/prod_short.md)] или сред со своей средой [!INCLUDE[prod_short](includes/cds_long_md.md)]. В сценариях синхронизации нескольких организаций необходимо учитывать несколько моментов.

### <a name="set-company-ids"></a>Задание идентификаторов организаций

Когда вы синхронизируете записи, мы устанавливаем идентификатор организации в сущности [!INCLUDE[prod_short](includes/cds_long_md.md)], чтобы уточнить, из какой организации [!INCLUDE [prod_short](includes/prod_short.md)] поступили записи. Сопоставления таблиц интеграции имеют поля фильтра для таблиц интеграции, в которых учитывается идентификатор организации. Чтобы включить сопоставление таблиц в конфигурацию с несколькими организациями, на странице **Сопоставление таблиц интеграции** установите флажок **Синхронизация нескольких организаций включена**. Этот флажок оптимизирует фильтрацию по идентификаторам организаций в фильтре таблиц интеграции в конфигурации с несколькими организациями.

Для сопоставлений таблиц интеграции, которые синхронизируют документы, такие как заказы, предложения и возможности, при установке флажка **Синхронизация нескольких организаций включена** интеграция будет учитывать только сущности с идентификатором организации, соответствующим текущей организации [!INCLUDE [prod_short](includes/prod_short.md)]. Например, чтобы синхронизировать документы между Business Central и Sales, пользователи в Sales должны указывать идентификатор организации в документах. В противном случае документы не будут синхронизироваться.  

Для всех других сопоставлений таблиц интеграции установка флажка **Синхронизация нескольких организаций включена** убирает фильтр по идентификатору организации. При синхронизации будут учитываться связанные сущности независимо от их идентификатора организации.

### <a name="specify-the-synchronization-direction"></a>Задание направления синхронизации

Если вы включаете поддержку нескольких организации для сопоставления таблиц интеграции, мы рекомендуем установить направление синхронизации **Из интеграции**. Если вы зададите направление **В интеграцию** или **Двунаправленная**, желательно использовать **Фильтр таблиц** и **Фильтр таблиц интеграции** для управления тем, какие сущности синхронизируются с какой организацией. Также рекомендуется использовать связывание на основе совпадений во избежание создания повторяющихся записей. Подробнее о связывании на основе совпадений см. в статье [Настройка связывания на основе совпадений](/dynamics365/business-central/admin-how-to-set-up-a-dynamics-crm-connection#customize-the-match-based-coupling).

### <a name="use-unique-numbers"></a>Использование уникальных номеров

Если ваша серия номеров не гарантирует уникальность значений первичного ключа для каждой организации, мы рекомендуем использовать префиксы. Чтобы начать использовать префиксы, создайте правило преобразования в сопоставлении полей интеграции. Подробнее о правилах трансформации см. в разделе [Обработка различий в значениях полей](admin-how-to-modify-table-mappings-for-synchronization.md#handle-differences-in-field-values).

## <a name="see-also"></a>См. также

[Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)   
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
