---
title: Сопоставление таблиц и полей для синхронизации | Microsoft Docs
description: Узнайте, как сопоставить таблицы и поля для синхронизации данных между Business Central и Dynamics 365 Sales.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize, table mapping
ms.date: 12/18/2019
ms.author: bholtorf
ms.openlocfilehash: 371bd80c04917495ea1b35f214d10d716ed5f9ad
ms.sourcegitcommit: b570997f93d1f7141bc9539c93a67a91226660a8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2020
ms.locfileid: "2943117"
---
# <a name="mapping-the-tables-and-fields-to-synchronize"></a>Сопоставление таблиц и полей для синхронизации
Основой синхронизации данных в [!INCLUDE[d365fin](includes/d365fin_md.md)] с данными в [!INCLUDE[crm_md](includes/crm_md.md)] является сопоставление таблиц и полей, которые содержат данные, друг с другом. Сопоставление происходит через таблицы интеграции. 

## <a name="mapping-integration-tables"></a>Сопоставление таблиц интеграции
Таблица интеграции — это таблица базе данных [!INCLUDE[d365fin](includes/d365fin_md.md)], представляющая объект, например счет, в [!INCLUDE[crm_md](includes/crm_md.md)]. Таблица интеграции включает поля, соответствующие полям в таблице объекта [!INCLUDE[crm_md](includes/crm_md.md)]. Например, таблица интеграции "Счет" связывается с объектом "Счета" в [!INCLUDE[crm_md](includes/crm_md.md)]. Для каждого объекта в [!INCLUDE[crm_md](includes/crm_md.md)], который необходимо синхронизировать с данными в [!INCLUDE[d365fin](includes/d365fin_md.md)], должно быть соответствующее сопоставление таблиц интеграции.

Когда вы создаете связь между приложениями, [!INCLUDE[d365fin](includes/d365fin_md.md)] настраивает некоторые сопоставления таблиц и полей по умолчанию. При желании вы можете изменить сопоставление таблиц. Дополнительные сведения см. в разделе [Сопоставление стандартных объектов Sales для синхронизации](admin-synchronizing-business-central-and-sales.md#standard-sales-entity-mapping-for-synchronization). Если вы изменили сопоставления по умолчанию и хотите отменить изменения, на странице **Настройка подключения к Dynamics 365**, выберите **Использовать настройку синхронизации по умолчанию**.

> [!Note]
> Если вы используете локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] сопоставления таблиц интеграции хранятся в таблице 5335 Сопоставления таблиц интеграции, и их можно просмотреть и изменить на странице 5335 Сопоставления таблиц интеграции. Сложные сопоставления и правила синхронизации определены в модуле Codeunit 5341. 

### <a name="synchronization-rules"></a>Правила синхронизации
Сопоставление таблиц интеграции также включает в себя правила, управляющие тем, как задания синхронизации интеграции синхронизируют записи в таблице [!INCLUDE[d365fin](includes/d365fin_md.md)] и объекте в [!INCLUDE[crm_md](includes/crm_md.md)]. Для получения дополнительной информации см. [Правила синхронизации](admin-synchronizing-business-central-and-sales.md#synchronization-rules). 

## <a name="mapping-integration-fields"></a>Сопоставления полей интеграции
Составление таблиц — это только первый шаг. Вы также должны сопоставить поля в таблицах. Сопоставления полей интеграции связывают поля в таблицах [!INCLUDE[d365fin](includes/d365fin_md.md)] с соответствующими полями в [!INCLUDE[crm_md](includes/crm_md.md)] и определяют, нужно ли синхронизировать данные в каждой таблице. Стандартное сопоставление таблиц, которое предоставляет [!INCLUDE[d365fin](includes/d365fin_md.md)], включает сопоставления полей, но вы можете изменить их. Дополнительные сведения см. в разделе [Просмотр сопоставлений объектов](admin-synchronizing-business-central-and-sales.md#tip-for-admins-viewing-entity-mappings).

> [!Note]
> Если вы используете локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)], сопоставления полей интеграции определены в таблице 5336 Сопоставление полей интеграции.

## <a name="coupling-records"></a>Связывание записей
Связывание сопоставляет записи в [!INCLUDE[crm_md](includes/crm_md.md)] с записями в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Например, счета в [!INCLUDE[crm_md](includes/crm_md.md)] обычно связываются с клиентами в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Связывание записей дает следующие преимущества:

* Оно делает возможной синхронизацию.
* Пользователи могут открывать записи в одном бизнес-приложении из другого. Для этого требуется, чтобы в [!INCLUDE[crm_md](includes/crm_md.md)] было настроено решение интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)].

Связывания могут быть настроены автоматически с помощью заданий синхронизации или вручную путем изменения записи в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для получения дополнительной информации см. [Синхронизация данных в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]](admin-synchronizing-business-central-and-sales.md) и [Связывание и синхронизация записей вручную](admin-manual-synchronization-of-table-mappings.md#synchronize-individual-table-mappings).

## <a name="filtering-records"></a>Фильтрация записей  
Если вы не хотите синхронизировать все записи для конкретного объекта [!INCLUDE[crm_md](includes/crm_md.md)] или таблицы в [!INCLUDE[d365fin](includes/d365fin_md.md)], можно настроить фильтры для ограничения синхронизируемых записей. Можно установить фильтры на странице **Сопоставления таблиц интеграции**.  

#### <a name="to-filter-records-for-synchronization"></a>Фильтрация записей для синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  Для фильтрации записей [!INCLUDE[d365fin](includes/d365fin_md.md)] задайте значение в поле **Фильтр таблицы**.  

3.  Для фильтрации записей [!INCLUDE[crm_md](includes/crm_md.md)] задайте значение в поле **Фильтр таблицы интеграции**.  

## <a name="creating-new-records"></a>Создание записей  
 По умолчанию задания синхронизации интеграции выполнят синхронизацию только связанных записей в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Можно настроить сопоставления таблицы, чтобы новые записи были созданы в назначении (например, [!INCLUDE[d365fin](includes/d365fin_md.md)]) для каждой записи в источнике (например, [!INCLUDE[crm_md](includes/crm_md.md)]), которая уже не связана.  

 Например, задание синхронизации "ПРОДАВЦЫ — Dynamics 365 Sales" использует сопоставление таблицы ПРОДАВЦЫ. Задание синхронизации копирует данные из записей пользователей в [!INCLUDE[crm_md](includes/crm_md.md)] в записи продавцов в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сопоставление таблицы настроено для создания записей, для каждого пользователя в [!INCLUDE[crm_md](includes/crm_md.md)], который еще не связан с продавцом в [!INCLUDE[d365fin](includes/d365fin_md.md)], в [!INCLUDE[d365fin](includes/d365fin_md.md)] создается новая запись продавца.  

#### <a name="to-create-new-records-during-synchronization"></a>Создание записей во время синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  В операции сопоставления таблицы в списке удалите значение в поле **Синхр. только связанные записи**.  

## <a name="using-configuration-templates-on-table-mappings"></a>Использование шаблонов конфигурации для сопоставлений таблицы
Шаблоны конфигурации можно назначить для сопоставлений таблицы, чтобы они использовали новые записи, созданные в [!INCLUDE[d365fin](includes/d365fin_md.md)] или [!INCLUDE[crm_md](includes/crm_md.md)]. Для каждого сопоставления таблицы можно задать шаблон конфигурации, чтобы он использовался для новых записей [!INCLUDE[d365fin](includes/d365fin_md.md)], и другой шаблон, который должен использовать новые записи [!INCLUDE[crm_md](includes/crm_md.md)].  

При установке настройки синхронизации по умолчанию, в большинстве случаев буду автоматически созданы два шаблона конфигурации и применены для сопоставления таблицы для клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)] и организаций [!INCLUDE[crm_md](includes/crm_md.md)]: **CRMCUST** и **CRMACCOUNT**.  

-   **CRMCUST** используется для создания и синхронизации новых клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] на основе организации в [!INCLUDE[crm_md](includes/crm_md.md)].  

     Этот шаблон создается путем копирования существующего шаблона конфигурации для клиентов в приложении. **CRMCUST** создается только в том случае, если имеется существующий шаблон конфигурации, а поле **Код валюты** в шаблоне пустое. Если в поле шаблона конфигурации содержится значение, это значение будет использоваться вместо значения в сопоставленном поле для организации [!INCLUDE[crm_md](includes/crm_md.md)]. Например, если в поле **Страна/регион** в организации в [!INCLUDE[crm_md](includes/crm_md.md)] указано *U.S.*, а в поле **Страна/регион** в шаблоне конфигурации указано *GB*, используется *GB* в качестве **Страна/регион** в созданном клиенте в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

-   **CRMACCOUNT** создает и синхронизирует новую организацию в [!INCLUDE[crm_md](includes/crm_md.md)] на основе организации в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

#### <a name="to-specify-configuration-templates-on-a-table-mapping"></a>Указание шаблонов конфигурации для сопоставления таблицы  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите соответствующую ссылку.

2.  В операции сопоставления таблицы в списке в поле **Код шаблона конфигурации таблиц** выберите шаблон конфигурации для использования для новых записей в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

3.  Задайте в поле **Код шаблона конфигурации внутр. табл.** шаблон конфигурации для использования для новых записей в [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>См. также  
[Об интеграции Dynamics 365 Business Central с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md )   
[Синхронизация Business Central и Dynamics 365 Sales](admin-synchronizing-business-central-and-sales.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
