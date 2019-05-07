---
title: Изменение сопоставления таблиц для синхронизации | Документы Майкрософт
description: Узнайте, как изменить сопоставления таблиц, которые используются при синхронизации данных между Business Central и Dynamics 365 for Sales.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize, table mapping
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: de924baa494ae00c09dcb7657c050f2d9ae3ba87
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "940302"
---
# <a name="modify-table-mappings-for-synchronization"></a>Изменение сопоставлений таблицы для синхронизации
Сопоставление таблицы интеграции связывает таблицу [!INCLUDE[d365fin](includes/d365fin_md.md)] с таблицей интеграции для объекта [!INCLUDE[crm_md](includes/crm_md.md)]. Для каждого объекта в [!INCLUDE[crm_md](includes/crm_md.md)], которую необходимо синхронизировать с соответствующими данными в [!INCLUDE[d365fin](includes/d365fin_md.md)], должно быть соответствующее сопоставление таблиц интеграции. Сопоставление таблицы интеграции включает ряд настроек, позволяющих управлять синхронизацией записей в [!INCLUDE[d365fin](includes/d365fin_md.md)] и объекта [!INCLUDE[crm_md](includes/crm_md.md)] с использованием соответствующих заданий синхронизации интеграции.  

## <a name="filtering-records"></a>Фильтрация записей  
 Если вы не хотите синхронизировать все записи для конкретного объекта [!INCLUDE[crm_md](includes/crm_md.md)] или таблицы в [!INCLUDE[d365fin](includes/d365fin_md.md)], можно настроить фильтры для ограничения синхронизируемых записей. Можно установить фильтры на странице **Сопоставления таблиц интеграции**.  

#### <a name="to-filter-records-for-synchronization"></a>Фильтрация записей для синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите связанную ссылку.

2.  Для фильтрации записей [!INCLUDE[d365fin](includes/d365fin_md.md)] задайте значение в поле **Фильтр таблицы**.  

3.  Для фильтрации записей [!INCLUDE[crm_md](includes/crm_md.md)] задайте значение в поле **Фильтр таблицы интеграции**.  

## <a name="creating-new-records"></a>Создание записей  
 По умолчанию задания синхронизации интеграции выполнят синхронизацию только связанных записей в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Можно настроить сопоставления таблицы, чтобы новые записи были созданы в назначении (например, [!INCLUDE[d365fin](includes/d365fin_md.md)]) для каждой записи в источнике (например, [!INCLUDE[crm_md](includes/crm_md.md)]), которая уже не связана.  

 Например, задание синхронизации "ПРОДАВЦЫ — Dynamics 365 for Sales" использует сопоставление таблицы ПРОДАВЦЫ. Задание синхронизации копирует данные из записей пользователей в [!INCLUDE[crm_md](includes/crm_md.md)] в записи продавцов в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если сопоставление таблицы настроено для создания записей, для каждого пользователя в [!INCLUDE[crm_md](includes/crm_md.md)], который еще не связан с продавцом в [!INCLUDE[d365fin](includes/d365fin_md.md)], в [!INCLUDE[d365fin](includes/d365fin_md.md)] создается новая запись продавца.  

#### <a name="to-create-new-records-during-synchronization"></a>Создание записей во время синхронизации  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите связанную ссылку.

2.  В операции сопоставления таблицы в списке удалите значение в поле **Синхр. только связанные записи**.  

## <a name="using-configuration-templates-on-table-mappings"></a>Использование шаблонов конфигурации для сопоставлений таблицы
Шаблоны конфигурации можно назначить для сопоставлений таблицы, чтобы они использовали новые записи, созданные в [!INCLUDE[d365fin](includes/d365fin_md.md)] или [!INCLUDE[crm_md](includes/crm_md.md)]. Для каждого сопоставления таблицы можно задать шаблон конфигурации, чтобы он использовался для новых записей [!INCLUDE[d365fin](includes/d365fin_md.md)], и другой шаблон, который должен использовать новые записи [!INCLUDE[crm_md](includes/crm_md.md)].  

При установке настройки синхронизации по умолчанию, в большинстве случаев буду автоматически созданы два шаблона конфигурации и применены для сопоставления таблицы для клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)] и организаций [!INCLUDE[crm_md](includes/crm_md.md)]: **CRMCUST** и **CRMACCOUNT**.  

-   **CRMCUST** используется для создания и синхронизации новых клиентов в [!INCLUDE[d365fin](includes/d365fin_md.md)] на основе организации в [!INCLUDE[crm_md](includes/crm_md.md)].  

     Этот шаблон создается путем копирования существующего шаблона конфигурации для клиентов в приложении. **CRMCUST** создается только в том случае, если имеется существующий шаблон конфигурации, а поле **Код валюты** в шаблоне пустое. Если в поле шаблона конфигурации содержится значение, это значение будет использоваться вместо значения в сопоставленном поле для организации [!INCLUDE[crm_md](includes/crm_md.md)]. Например, если в поле **Страна/регион** в организации в [!INCLUDE[crm_md](includes/crm_md.md)] указано *U.S.*, а в поле **Страна/регион** в шаблоне конфигурации указано *GB*, используется *GB* в качестве **Страна/регион** в созданном клиенте в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

-   **CRMACCOUNT** создает и синхронизирует новую организацию в [!INCLUDE[crm_md](includes/crm_md.md)] на основе организации в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

#### <a name="to-specify-configuration-templates-on-a-table-mapping"></a>Указание шаблонов конфигурации для сопоставления таблицы  
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сопоставления таблиц интеграции**, затем выберите связанную ссылку.

2.  В операции сопоставления таблицы в списке в поле **Код шаблона конфигурации таблиц** выберите шаблон конфигурации для использования для новых записей в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

3.  Задайте в поле **Код шаблона конфигурации внутр. табл.** шаблон конфигурации для использования для новых записей в [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="see-also"></a>См. также  
[Об интеграции Dynamics 365 Business Central с Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md )   
[Синхронизация данных в Business Central и Dynamics 365 for Sales](admin-synchronizing-business-central-and-sales.md)   
[Синхронизация по расписанию](admin-scheduled-synchronization-using-the-synchronization-job-queue-entries.md)  
