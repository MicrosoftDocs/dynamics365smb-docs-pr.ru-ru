---
title: Сопоставление таблиц и полей для синхронизации | Microsoft Docs
description: Узнайте, как сопоставить таблицы и поля для синхронизации данных между Business Central и Microsoft Dataverse.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize, table mapping
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 9c11e4f5acb0055b42a2d172f9a7deba75edfb08
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5779811"
---
# <a name="mapping-the-tables-and-fields-to-synchronize"></a>Сопоставление таблиц и полей для синхронизации
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

Основой синхронизации данных является сопоставление таблиц и полей в [!INCLUDE[prod_short](includes/prod_short.md)] с таблицами и столбцами в [!INCLUDE[prod_short](includes/cds_long_md.md)], чтобы они могли обмениваться данными. Сопоставление происходит через таблицы интеграции. 

## <a name="mapping-integration-tables"></a>Сопоставление таблиц интеграции
Таблица интеграции — это таблица базе данных [!INCLUDE[prod_short](includes/prod_short.md)], представляющая таблицу, например счет, в [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Таблица интеграции включает поля, соответствующие столбцам в таблице [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Например, таблица интеграции "Счет" связывается с таблицей "Счета" в [!INCLUDE[cds_short_md](includes/cds_long_md.md)]. Для каждой таблице в [!INCLUDE[cds_short_md](includes/cds_short_md.md)], которую необходимо синхронизировать с данными в [!INCLUDE[prod_short](includes/prod_short.md)], должно быть соответствующее сопоставление таблиц интеграции.

Когда вы создаете связь между приложениями, [!INCLUDE[prod_short](includes/prod_short.md)] настраивает некоторые сопоставления по умолчанию. При желании вы можете изменить сопоставление таблиц. Дополнительные сведения см. в разделе [Сопоставление стандартных таблиц для синхронизации](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization). Если вы изменили сопоставления по умолчанию и хотите отменить изменения, на странице **Сопоставления таблиц интеграции**, выберите **Использовать настройку синхронизации по умолчанию**.

> [!Note]
> Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)], сопоставления таблиц интеграции хранятся в таблице "5335 Сопоставления таблиц интеграции", где можно просмотреть и изменить сопоставления. Сложные сопоставления и правила синхронизации определены в модуле Codeunit 5341. 

### <a name="synchronization-rules"></a>Правила синхронизации
Сопоставление таблиц интеграции также включает в себя правила, управляющие тем, как задания синхронизации интеграции синхронизируют записи в таблице [!INCLUDE[prod_short](includes/prod_short.md)] и таблице в [!INCLUDE[prod_short](includes/cds_long_md.md)]. <!--For examples of rules for an integration with Sales, see [Synchronization Rules](admin-synchronizing-business-central-and-sales.md#synchronization-rules). need to verify link -->

### <a name="strategies-for-auto-resolving-conflicts"></a>Стратегии автоматического разрешения конфликтов
Конфликты данных могут легко возникнуть, когда бизнес-приложения обмениваются данными на постоянной основе. Например, кто-то может удалить или изменить строку в одном из приложений или в обоих. Чтобы уменьшить количество конфликтов, которые вам придется разрешать вручную, вы можете указать стратегии разрешения, и [!INCLUDE[prod_short](includes/prod_short.md)] автоматически будет разрешать конфликты в соответствии с правилами в стратегиях.

Сопоставления таблиц интеграции включают правила, управляющие тем, как задания синхронизации синхронизируют записи. На странице **Сопоставление таблиц интеграции** в столбцах **Разрешение конфликтов удаления** и **Разрешение конфликтов обновления** вы можете указать, как [!INCLUDE[prod_short](includes/prod_short.md)] разрешает конфликты, возникающие из-за удаления записей в таблицах в одном или другом бизнес-приложении или обновления в обоих. 

В столбце **Разрешение конфликтов удаления** вы можете выбрать, чтобы [!INCLUDE[prod_short](includes/prod_short.md)] автоматически восстанавливал удаленные записи, удалял связи между записями или ничего не делал. Если вы ничего не сделаете, вы должны вручную разрешить конфликты. 

В столбце **Разрешение конфликтов обновления** вы можете выбрать, чтобы [!INCLUDE[prod_short](includes/prod_short.md)] автоматически отправлял обновление данных в таблицу интеграции при отправке данных в [!INCLUDE[prod_short](includes/cds_long_md.md)], получал обновление данных из таблицы интеграции при получении данных из [!INCLUDE[prod_short](includes/cds_long_md.md)] или ничего не делал. Если вы ничего не сделаете, вы должны вручную разрешить конфликты.

После того, как вы укажете стратегию, на странице **Ошибки синхронизации связанных данных**, вы можете выбрать действие **Повторить все** для автоматического разрешения конфликтов. 

## <a name="mapping-integration-fields"></a>Сопоставления полей интеграции
Составление таблиц — это только первый шаг. Вы также должны сопоставить поля в таблицах. Сопоставления полей интеграции связывают поля в таблицах [!INCLUDE[prod_short](includes/prod_short.md)] с соответствующими столбцам в [!INCLUDE[prod_short](includes/cds_long_md.md)] и определяют, нужно ли синхронизировать данные в каждой таблице. Стандартное сопоставление таблиц, которое предоставляет [!INCLUDE[prod_short](includes/prod_short.md)], включает сопоставления полей, но вы можете изменить их. Дополнительные сведения см. в разделе [Просмотр сопоставлений таблиц](admin-synchronizing-business-central-and-sales.md#tip-for-admins-viewing-table-mappings).

> [!Note]
> Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)], сопоставления полей интеграции определены в таблице 5336 Сопоставление полей интеграции.

### <a name="handling-differences-in-field-values"></a>Обработка различий в значениях полей
Иногда значения в полях, которые, вы хотите сопоставить, различаются. Например, в [!INCLUDE[crm_md](includes/crm_md.md)] код языка для США — "U.S.", а в [!INCLUDE[prod_short](includes/prod_short.md)] — "US". Это означает, что вы должны преобразовать значение при синхронизации данными. Это происходит через правила преобразования, которые вы определяете для полей. Вы определяете правила преобразования на странице **Сопоставления таблиц интеграции**, выбрав **Сопоставление**, затем **Поля**. Доступные готовые правила, но вы также можете создавать свои собственные. Для получения дополнительной информации см. [Правила преобразования](across-how-to-set-up-data-exchange-definitions.md#transformation-rules).

### <a name="handling-missing-option-values-in-mapping"></a>Обработка отсутствующих значений параметров в сопоставлении
[!INCLUDE[prod_short](includes/cds_long_md.md)] содержит столбцы набора параметров, предоставляющие значения параметров, которые можно сопоставить полям [!INCLUDE[prod_short](includes/prod_short.md)] типа **Параметр** для автоматической синхронизации. Во время синхронизации несопоставленные параметры игнорируются, а отсутствующие параметры добавляются к связанной таблице [!INCLUDE[prod_short](includes/prod_short.md)] и добавляются в системную таблицу **Сопоставление параметров CDS** для обработки вручную позже. Например, добавив отсутствующие параметры в любом продукте, а затем обновив сопоставление. Дополнительные сведения см. в разделе [Обработка отсутствующих значений параметров](admin-cds-missing-option-values.md).

## <a name="coupling-records"></a>Связывание записей
Связывание сопоставляет строки в [!INCLUDE[prod_short](includes/cds_long_md.md)] с записями в [!INCLUDE[prod_short](includes/prod_short.md)]. Например, счета в [!INCLUDE[prod_short](includes/cds_long_md.md)] обычно связываются с клиентами в [!INCLUDE[prod_short](includes/prod_short.md)]. Связывание записей дает следующие преимущества:

* Оно делает возможной синхронизацию.
* Пользователи могут открывать записи или строки в одном бизнес-приложении из другого. Это требует, чтобы приложения уже были интегрированы.

Связывания могут быть настроены автоматически с помощью заданий синхронизации или вручную путем изменения записи в [!INCLUDE[prod_short](includes/prod_short.md)]. Для получения дополнительной информации см. [Синхронизация данных в [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md) и [Связывание и синхронизация записей вручную](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings).

## <a name="filtering-records-and-rows"></a>Фильтрация записей и строк  
Если вы не хотите синхронизировать все строки для конкретной таблицы [!INCLUDE[prod_short](includes/cds_long_md.md)] или таблицы в [!INCLUDE[prod_short](includes/prod_short.md)], можно настроить фильтры для ограничения синхронизируемых данных. Можно установить фильтры на странице **Сопоставления таблиц интеграции**.  

#### <a name="to-filter-records-or-rows-for-synchronization"></a>Фильтрация записей или строк для синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  Для фильтрации записей [!INCLUDE[prod_short](includes/prod_short.md)] задайте значение в поле **Фильтр таблицы**.  

3.  Для фильтрации строк [!INCLUDE[prod_short](includes/cds_long_md.md)] задайте значение в поле **Фильтр таблицы интеграции**.  

## <a name="creating-new-records"></a>Создание записей  
По умолчанию задания синхронизации интеграции выполнят синхронизацию только связанных записей в [!INCLUDE[prod_short](includes/prod_short.md)] и строк в [!INCLUDE[prod_short](includes/cds_long_md.md)]. Можно настроить сопоставления таблицы, чтобы новые записи или строки были созданы в назначении (например, [!INCLUDE[prod_short](includes/prod_short.md)]) для каждой строки в источнике (например, [!INCLUDE[prod_short](includes/cds_long_md.md)]), которая уже не связана.  

Например, задание синхронизации "ПРОДАВЦЫ — Dynamics 365 Sales" использует сопоставление таблицы ПРОДАВЦЫ. Задание синхронизации копирует данные из пользователей в [!INCLUDE[prod_short](includes/cds_long_md.md)] в продавцов в [!INCLUDE[prod_short](includes/prod_short.md)]. Если сопоставление таблицы настроено для создания записей, для каждого пользователя в [!INCLUDE[prod_short](includes/cds_long_md.md)], который еще не связан с продавцом в [!INCLUDE[prod_short](includes/prod_short.md)], в [!INCLUDE[prod_short](includes/prod_short.md)] создается новая строка продавца.  

#### <a name="to-create-new-records-during-synchronization"></a>Создание записей во время синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  В операции сопоставления таблицы в списке удалите значение в поле **Синхр. только связанные записи**.  

## <a name="using-configuration-templates-on-table-mappings"></a>Использование шаблонов конфигурации для сопоставлений таблицы
Шаблоны конфигурации можно назначить для сопоставлений таблицы, чтобы они использовали новые записи или строки, созданные в [!INCLUDE[prod_short](includes/prod_short.md)] или [!INCLUDE[prod_short](includes/cds_long_md.md)]. Для каждого сопоставления таблицы можно задать шаблон конфигурации, чтобы он использовался для новых записей [!INCLUDE[prod_short](includes/prod_short.md)], и другой шаблон, который должен использовать новые строки [!INCLUDE[prod_short](includes/cds_long_md.md)].  

При установке настройки синхронизации по умолчанию, в большинстве случаев буду автоматически созданы два шаблона конфигурации и применены для сопоставления таблицы для клиентов [!INCLUDE[prod_short](includes/prod_short.md)] и организаций [!INCLUDE[crm_md](includes/crm_md.md)]: **CDSCUST** и **CDSACCOUNT**.  

-   **CDSCUST** используется для создания и синхронизации новых клиентов в [!INCLUDE[prod_short](includes/prod_short.md)] на основе организации в [!INCLUDE[crm_md](includes/crm_md.md)].  

     Этот шаблон создается путем копирования существующего шаблона конфигурации для клиентов в приложении. **CDSCUST** создается только в том случае, если имеется существующий шаблон конфигурации, а поле **Код валюты** в шаблоне пустое. Если в поле шаблона конфигурации содержится значение, это значение будет использоваться вместо значения в сопоставленном столбце для организации [!INCLUDE[prod_short](includes/cds_long_md.md)]. Например, если в столбце **Страна/регион** в организации в [!INCLUDE[prod_short](includes/cds_long_md.md)] указано *U.S.*, а в поле **Страна/регион** в шаблоне конфигурации указано *GB*, используется *GB* в качестве **Страна/регион** в созданном клиенте в [!INCLUDE[prod_short](includes/prod_short.md)].  

-   **CDSACCOUNT** создает и синхронизирует новую организацию в [!INCLUDE[prod_short](includes/cds_long_md.md)] на основе организации в [!INCLUDE[prod_short](includes/prod_short.md)].  

#### <a name="to-specify-configuration-templates-on-a-table-mapping"></a>Указание шаблонов конфигурации для сопоставления таблицы  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  В операции сопоставления таблицы в списке в поле **Код шаблона конфигурации таблиц** выберите шаблон конфигурации для использования для новых записей в [!INCLUDE[prod_short](includes/prod_short.md)].  

3.  Задайте в поле **Код шаблона конфигурации внутр. табл.** шаблон конфигурации для использования для новых записей в [!INCLUDE[prod_short](includes/cds_long_md.md)].

## <a name="see-also"></a>См. также  
[Об интеграции Dynamics 365 Business Central с [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-prepare-dynamics-365-for-sales-for-integration.md )   
[Синхронизация данных в Business Central и [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-synchronizing-business-central-and-sales.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]