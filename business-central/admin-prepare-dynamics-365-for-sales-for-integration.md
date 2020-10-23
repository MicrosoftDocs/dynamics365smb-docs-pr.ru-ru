---
title: Интеграция с Dynamics 365 Sales | Документация Майкрософт
description: Узнайте, как подготовить Dynamics 365 Business Central к интеграции с Dynamics 365 Sales.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: e93d36c2767bc43444b5b23471b6d0aaa0c84adf
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917830"
---
# <a name="integrating-with-dynamics-365-sales"></a>Интеграция с Dynamics 365 Sales

Роль менеджера по продажам часто рассматривается как самая направленная наружу должность в бизнесе. Однако может быть полезно для менеджеров по продажам посмотреть внутрь бизнеса и увидеть, что происходит на заднем дворе. Путем интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], можно предоставить менеджерам по продажи такие аналитические данные, позволив им просматривать информацию в [!INCLUDE[d365fin](includes/d365fin_md.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, при подготовке предложения по продаже может быть полезно знать, имеется ли достаточно запасов для выполнения заказа. Дополнительные сведения см. в разделе [Использование Dynamics 365 Sales из Business Central](marketing-integrate-dynamicscrm.md).

> [!NOTE]
> В этом разделе описывается процесс интеграции сетевых версий [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)] через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Сведения о локальной конфигурации см. в разделе [Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration).

## <a name="integrating-through-common-data-service"></a>Интеграция через Common Data Service
[!INCLUDE[d365fin](includes/d365fin_md.md)] также интегрируется с [!INCLUDE[d365fin](includes/cds_long_md.md)], что позволяет легко подключать и синхронизировать данные с другими приложениями Dynamics 365, такими как [!INCLUDE[crm_md](includes/crm_md.md)], или даже с приложениями, которые вы создаете сами. Если вы впервые выполняете интеграцию, мы рекомендуем сделать это через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Интеграция с Common Data Service](admin-common-data-service.md).

Если вы уже интегрировали [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], вы можете продолжить синхронизацию данных, используя ваши настройки. Однако, если вы обновите или выключите интеграцию [!INCLUDE[crm_md](includes/crm_md.md)], чтобы включить его снова, вы должны подключиться через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Обновление интеграции с Dynamics 365 Sales](admin-upgrade-sales-to-cds.md).

> [!NOTE]
> При повторном подключении через [!INCLUDE[d365fin](includes/cds_long_md.md)] применяются настройки синхронизации по умолчанию и перезаписываются все ваши конфигурации. Например, будут применены сопоставления таблиц по умолчанию.

## <a name="integration-settings-that-are-specific-to-a-crm_md-integration"></a>Параметры интеграции, специфичные для интеграции [!INCLUDE[crm_md](includes/crm_md.md)]
Интеграция с [!INCLUDE[d365fin](includes/d365fin_md.md)] происходит через [!INCLUDE[d365fin](includes/cds_long_md.md)], и есть много стандартных настроек и сущностей, которые обеспечиваются интеграцией. В дополнение к стандартным настройкам, есть некоторые, которые являются специфическими для [!INCLUDE[crm_md](includes/crm_md.md)]. Они перечислены в следующих разделах.

## <a name="permissions-and-security-roles-for-user-accounts-in-sales"></a>Разрешения и роли безопасности для учетных записей пользователей в Sales
При установке решения интеграции разрешения для учетной записи пользователя интеграции настраиваются. Если эти разрешения изменены, вам может потребоваться сбросить их. Вы можете сделать это, переустановив решение интеграции, выбрав **Повторить развертывание решения интеграции** на странице **Настройка подключения Dynamics 365**. Развернуты следующие роли безопасности:

* Администратор интеграции Dynamics 365 Business Central
* Пользователь интеграции Dynamics 365 Business Central
* Пользователь наличия товара Dynamics 365 Business Central

### <a name="connection-settings-in-the-setup-guide"></a>Настройки подключения в руководстве по установке

Вы можете использовать мастер настройки, чтобы быстро настроить подключение и указать расширенные функции, такие как связи между записями.

1. Выберите **Настройка и расширения**, затем выберите **Мастер настройки**.
2. Выберите **Настройка подключения к Dynamics 365 Sales**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.
4. При необходимости, имеются расширенные настройки, которые могут улучшить безопасность и включить дополнительные возможности, такие как обработка заказов на продажу и просмотр уровней запасов. Расширенные параметры рассматриваются в таблице ниже.  

| Поле | Описание |
|--|--|
| **Импорт решения Dynamics 365 Sales** | Разрешить это, чтобы установить и настроить решение интеграции в [!INCLUDE[crm_md](includes/crm_md.md)]. <!--For more information, see [About the Base CDS Integration Solution](admin-common-data-service.md#about-the-business-central-integration-solution). Need to add a new topic--> |
| **Публикация веб-службы наличия товаров** | Разрешите пользователям, которые используют [!INCLUDE[crm_md](includes/crm_md.md)], просматривать наличие товаров (продуктов) в запасах в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для этого необходима учетная запись пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] с ключом доступа к веб-службам. Назначение ключа выполняется в два этапа. В учетной записи пользователя в [!INCLUDE[d365fin](includes/d365fin_md.md)] необходимо выбрать действие **Изменить ключ веб-службы**. В мастере настройки "Настройка подключения к Dynamics 365 Sales" необходимо указать URL-адрес веб-службы Dynamics 365 Business Central OData и предоставить учетные данные пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] для получения доступа к сервису. Дополнительные сведения см. в разделе [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services). |
| **URL-адрес веб-службы OData Business Central** | Если включена веб-служба для просмотра наличия товаров, URL-адрес веб-службы OData предоставляется для вас. |
| **Имя пользователя веб-службы OData Business Central** | Имя пользователя учетной записи [!INCLUDE[d365fin](includes/d365fin_md.md)], которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для извлечения сведений о наличии товаров в [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData. |
| **Ключ доступа веб-службы OData Business Central** | Ключ доступа учетной записи пользователя, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData. Ключ назначается пользователю, выбранному в поле **Имя пользователя веб-службы OData Business Central**. Чтобы получить ключ, выберите кнопку **Найти значение** рядом с именем пользователя, выберите пользователя, выберите **Управление**, затем выберите **Правка**. В карточке пользователя выберите **Действия**, **Проверка подлинности**, затем выберите **Изменить ключ веб-службы**. |
| **Включить интеграцию с заказом на продажу** | Когда сотрудники создают заказы на продажу в [!INCLUDE[crm_md](includes/crm_md.md)] и выполняют заказы в [!INCLUDE[d365fin](includes/d365fin_md.md)], это интегрирует процесс в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Включение интеграции обработки заказов на продажу](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration). Для этого требуется, чтобы вы предоставили учетные данные для учетной записи пользователя-администратора в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Обработка данных в заказах на продажу](marketing-integrate-dynamicscrm.md#handling-sales-order-data). |
| **Включить подключение к CDS** | Включите подключение к [!INCLUDE[d365fin](includes/cds_long_md.md)]. |
| **Версия SDK Dynamics 365** | Это необходимо только в том случае, если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)]. Это комплект разработки программного обеспечения Dynamics 365 (также называемый Xrm), который используется для подключения [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Версия должна быть совместима с версией пакета SDK, которая используется [!INCLUDE[crm_md](includes/crm_md.md)], и равна или новее версии, используемой [!INCLUDE[crm_md](includes/crm_md.md)]. |

### <a name="connection-settings-on-the-microsoft-dynamics-365-connection-setup-page"></a>Параметры подключения на странице настройки подключения Microsoft Dynamics 365

Введите следующие сведения для подключения из [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)].

| Поле | Описание |
|--|--|
| **URL-адрес Dynamics 365 Sales** | URL-адрес вашего экземпляра [!INCLUDE[crm_md](includes/crm_md.md)]. Это позволяет пользователям открывать соответствующие записи в [!INCLUDE[d365fin](includes/d365fin_md.md)] из записей в [!INCLUDE[crm_md](includes/crm_md.md)], например счет или продукт. Записи [!INCLUDE[d365fin](includes/d365fin_md.md)] открываются в [!INCLUDE[d365fin](includes/d365fin_md.md)]. |
|**URL-адрес Dynamics 365 Sales**|URL-адрес вашего экземпляра [!INCLUDE[crm_md](includes/crm_md.md)]. Это позволяет пользователям открывать соответствующие записи в [!INCLUDE[d365fin](includes/d365fin_md.md)] из записей в [!INCLUDE[crm_md](includes/crm_md.md)], например счет или продукт. Записи [!INCLUDE[d365fin](includes/d365fin_md.md)] открываются в [!INCLUDE[d365fin](includes/d365fin_md.md)].|
|**Веб-служба наличия товаров включена**|Разрешите пользователям, которые используют [!INCLUDE[crm_md](includes/crm_md.md)], просматривать наличие товаров (продуктов) в запасах в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Если она включена, также необходимо указать имя пользователя и ключ доступа для [!INCLUDE[crm_md](includes/crm_md.md)], чтобы использовать веб-службу OData для наличия товаров (продуктов). Дополнительные сведения см. в разделе [Веб-службы OData](/dynamics365/business-central/dev-itpro/webservices/odata-web-services).|
|**URL-адрес веб-службы OData Dynamics 365 Business Central**|Если включена веб-служба наличия товаров, URL-адрес веб-службы OData предоставляется для вас. Для использования задайте в этом поле URL-адрес экземпляра [!INCLUDE[d365fin](includes/d365fin_md.md)].<br /><br /> Для возврата в поле URL-адреса по умолчанию для [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите действие **Сбросить URL-адрес веб-клиента**.<br /><br /> Это поле используется только в случае установки решения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)].|
|**Имя пользователя веб-службы OData Dynamics 365 Business Central**|Имя пользователя учетной записи, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData.|
|**Ключ доступа веб-службы OData Dynamics 365 Business Central**|Ключ доступа учетной записи пользователя, которую [!INCLUDE[crm_md](includes/crm_md.md)] использует для получения сведений о наличии товаров из [!INCLUDE[d365fin](includes/d365fin_md.md)] через веб-службу OData. Ключ назначается пользователю, выбранному в поле **Имя пользователя веб-службы OData Dynamics 365 Business Central**. Чтобы получить ключ, выберите кнопку **Найти значение** рядом с именем пользователя, выберите пользователя, выберите **Управление**, затем выберите **Правка**. В карточке пользователя выберите **Действия**, **Проверка подлинности**, затем выберите **Изменить ключ веб-службы**.|
|**Версия SDK Dynamics 365**|Если выполняется интеграция с локальной версией [!INCLUDE[crm_md](includes/crm_md.md)], следует использовать набор разработки программного обеспечения Dynamics 365 (также называемый Xrm) для подключения [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)]. Выбранная версия должна быть совместима с версией SDK, которая используется приложением [!INCLUDE[crm_md](includes/crm_md.md)]. Эта версия равна или новее версии, используемой приложением [!INCLUDE[crm_md](includes/crm_md.md)].|-->

В дополнение к приведенным выше параметрам введите следующие настройки для [!INCLUDE[crm_md](includes/crm_md.md)].

| Поле | Описание |
|--|--|
| **Интеграция заказов на продажу разрешена** | Разрешите пользователям отправлять заказы на продажу и активированные предложения в [!INCLUDE[crm_md](includes/crm_md.md)] и затем просматривать и обрабатывать их в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Это интегрирует процесс в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Включение интеграции обработки заказов на продажу](/dynamics365/customer-engagement/sales-enterprise/developer/enable-sales-order-processing-integration). |
| **Автоматически создавать заказы на продажу** | Создание заказов на продажу в [!INCLUDE[d365fin](includes/d365fin_md.md)], когда пользователь создает и отправляет заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)]. |
| **Автоматически обрабатывать предложения по продаже** | Обработка предложения по продаже в [!INCLUDE[d365fin](includes/d365fin_md.md)], когда пользователь создает и активирует его в [!INCLUDE[crm_md](includes/crm_md.md)]. |

<!--
### User Account Settings
Integrate with Business Central through Common Data Service requires an administrator user account and an account that is used only for the connection between the apps. This account is called the "integration user." When you install the CDS Base Integration Solution, permissions for the integration user account are configured in [!INCLUDE[crm_md](includes/crm_md.md)]. If those permissions are changed you might need to reset them. You can do that by reinstalling the Integration Solution or by manually resetting them. The following tables list the minimum permissions for the user accounts in [!INCLUDE[crm_md](includes/crm_md.md)].  -->

### <a name="standard-sales-entity-mapping-for-synchronization"></a>Сопоставление стандартных объектов Sales для синхронизации

Объекты в [!INCLUDE[crm_md](includes/crm_md.md)], например заказы, интегрируются с эквивалентными типами объектов в [!INCLUDE[d365fin](includes/d365fin_md.md)], например заказы на продажу. Для работы с данными [!INCLUDE[crm_md](includes/crm_md.md)] нужно настроить ссылки, называемые связываниями, между объектами в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].

В следующей таблице перечислено стандартное соответствие между объектами в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], которое предоставляет [!INCLUDE[d365fin](includes/d365fin_md.md)].

| [!INCLUDE[d365fin](includes/d365fin_md.md)] | [!INCLUDE[crm_md](includes/crm_md.md)] | Направление синхронизации | Фильтр по умолчанию |
|--|--|--|--|
| Единица измерения | Группа единиц | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Товар | Продукт | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Тип контактов Sales: **Тип продукта** — **Товарный запас** |
| Ресурс | Продукт | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] | Тип контактов Sales: **Тип продукта** — **Услуги** |
| Ценовая группа клиента | Прайс-лист | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Цена продажи | Прайс-лист на продукцию | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] | Фильтр контактов [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Код продажи** не пустой, **Тип продажи** — **Ценовая группа клиента** |
| Возможность | Возможность | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] |  |
| Заголовок счета продажи | Счет | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Строка счета продажи | Продукт счета | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] |  |
| Заголовок заказа на продажу | Заказ на продажу | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] | Фильтр заголовков продаж [!INCLUDE[d365fin](includes/d365fin_md.md)]: **Тип документа** — Заказ, **Статус** — Выпущено |
| Примечания заказа на продажу | Примечания заказа на продажу | [!INCLUDE[d365fin](includes/d365fin_md.md)] -> [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] -> [!INCLUDE[d365fin](includes/d365fin_md.md)] |  |

### <a name="synchronization-rules"></a>Правила синхронизации

В следующей таблице перечислены правила, управляющие синхронизацией между [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)]. Это в дополнение к правилам, определенным для Common Data Service, которые также применяются. Дополнительные сведения см. в разделе [Сопоставление стандартных сущностей](/dynamics365/business-central/admin-synchronizing-business-central-and-sales?branch=master-cds-crm#standard-entity-mapping-for-synchronization).

> [!NOTE]  
> Изменения данных, которые были сделаны в учетной записи пользователя интеграции, не синхронизируются. Поэтому рекомендуется не изменять данные при использовании этой учетной записи. Дополнительные сведения см. в разделе [Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md).

|Стол|Правило|
|-----|----|
|Единицы измерения|Единицы измерения синхронизируются с группами единиц в [!INCLUDE[crm_md](includes/crm_md.md)]. Для группы единиц может быть задана только одна единица измерения.|
|Товаров|При синхронизации товаров с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], [!INCLUDE[d365fin](includes/d365fin_md.md)] автоматически создает прайс-лист в [!INCLUDE[crm_md](includes/crm_md.md)]. Чтобы избежать ошибок синхронизации, не следует изменять данный прайс-лист вручную.|
|Ресурсы|Ресурсы синхронизируются с продуктами [!INCLUDE[crm_md](includes/crm_md.md)], имеющими тип "Услуга".|
|Ценовые группы клиентов|Ценовые группы клиентов синхронизируются с прайс-листами Sales.|
|Цены продажи|Цены Sales с типом продажи "Ценовая группа клиента" и определенным кодом продаж, синхронизируются со строками прайс-листов [!INCLUDE[crm_md](includes/crm_md.md)].|
|Возможные сделки|Возможные сделки синхронизируются с возможными сделками [!INCLUDE[crm_md](includes/crm_md.md)]. Значение кода менеджера по продажам определяет владельца связанного объекта в [!INCLUDE[crm_md](includes/crm_md.md)].|
|Учтенные счета продажи|Учтенные счета продажи синхронизируются со счетами продажи. Прежде чем счет можно будет синхронизировать, рекомендуется синхронизировать все остальные объекты, которые могут быть использованы в нем, от менеджеров по продажам до прайс-листов. Значение кода менеджера по продажам в заголовке счета определяет владельца связанного объекта в Sales.|
|Заказы на продажу|Когда включена интеграция заказов на продажу, заказы на продажу в [!INCLUDE[d365fin](includes/d365fin_md.md)], которые созданы из отправленных заказов на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], синхронизируются с заказами на продажу в INCLUDE SALES, когда они выпущены. Прежде чем синхронизировать заказы, рекомендуется сначала синхронизировать все объекты, связанные с заказом, такие как продавцы и прайс-листы. Поле кода менеджера по продажам в заголовке заказа определяет владельца связанного объекта в [!INCLUDE[crm_md](includes/crm_md.md)].|

### <a name="synchronization-jobs-for-a-sales-integration"></a>Задания синхронизации для интеграции Sales

Задания выполняются в следующем порядке во избежание зависимостей связывания между объектами. Есть дополнительные задания, доступные из Common Data Service. Дополнительные сведения см. в разделе [Использование очередей работ для планирования задач](/dynamics365/business-central/admin-job-queues-schedule-tasks).

1. Задание синхронизации "ЕДИНИЦА ИЗМЕРЕНИЯ — Dynamics 365 Sales"  
2. Задание синхронизации "РЕСУРС-ПРОДУКТ - Dynamics 365 Sales"  
3. Задание синхронизации "ТОВАР-ПРОДУКТ — Dynamics 365 Sales"  
4. Задание синхронизации "CUSTPRCGRP-PRICE — Dynamics 365 Sales".
5. Задание синхронизации "SALESPRC-PRODPRICE — Dynamics 365 Sales".
6. Задание синхронизации "POSTEDSALESINV-INV — Dynamics 365 Sales".

### <a name="default-synchronization-job-queue-entries"></a>Операции очереди заданий синхронизации по умолчанию

В следующей таблице описываются задания синхронизации по умолчанию для Sales.  

|Операция очереди работ|Описание|Направление|Сопоставление таблиц интеграции|Частота синхронизации по умолчанию (мин)|Время бездействия по умолчанию (мин)|  
|---------------------|---------------------------------------|---------------|-------------------------------|-----|-----|  
|Задание синхронизации "ЕДИНИЦА ИЗМЕРЕНИЯ — Dynamics 365 Sales"|Синхронизирует группы единиц [!INCLUDE[crm_md](includes/crm_md.md)] с единицами измерения [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ЕДИНИЦА ИЗМЕРЕНИЯ|30|720<br> (12 ч.)|
|Задание синхронизации "РЕСУРС-ПРОДУКТ - Dynamics 365 Sales"|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с ресурсами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|РЕСУРС-ПРОДУКТ|30|720<br> (12 ч.)|
|Задание синхронизации "ТОВАР-ПРОДУКТ — Dynamics 365 Sales"|Синхронизирует продукты [!INCLUDE[crm_md](includes/crm_md.md)] с товарами [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|ТОВАР-ПРОДУКТ|30|1440<br> (24 ч.)|
|Задание синхронизации "CUSTPRCGRP-PRICE — Dynamics 365 Sales"|Синхронизирует прайс-листы продаж [!INCLUDE[crm_md](includes/crm_md.md)] с ценовыми группами клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)].| |ЦЕНОВЫЕ ГРУППЫ КЛИЕНТОВ — ПРАЙС-ЛИСТЫ ПРОДАЖ|30|1440<br> (24 ч.)|
|Задание синхронизации "SALESPRC-PRODUCTPRICE — Dynamics 365 Sales"|Синхронизирует цены продуктов [!INCLUDE[crm_md](includes/crm_md.md)] с ценами продажи [!INCLUDE[d365fin](includes/d365fin_md.md)].||ЦЕНА ПРОДУКТА — ЦЕНА ПРОДАЖ|30|1440<br> (24 ч.)|
|Задание синхронизации "POSTEDSALESINV-INV — Dynamics 365 Sales"|Синхронизирует счета [!INCLUDE[crm_md](includes/crm_md.md)] с учтенными счетами продаж [!INCLUDE[d365fin](includes/d365fin_md.md)].|Из [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]|СЧЕТА — УЧТЕННЫЕ СЧЕТА ПРОДАЖ|30|1440<br> (24 ч.)|
|Синхронизация "Статистика по клиенту — Dynamics 365 Sales"|Обновление организаций [!INCLUDE[crm_md](includes/crm_md.md)] с новейшими данными клиентов [!INCLUDE[d365fin](includes/d365fin_md.md)]. В [!INCLUDE[crm_md](includes/crm_md.md)] данная информация отображается в форме быстрого просмотра **Статистика организации Business Central** организаций, которые связаны с клиентами [!INCLUDE[d365fin](includes/d365fin_md.md)].<br /><br /> Эти данные можно также обновлять вручную из каждой записи клиента. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md). </BR></BR>**Примечание.** Эта запись очереди заданий используется только в случае установки решения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[crm_md](includes/crm_md.md)]. |Неприменимо|Неприменимо|30|Неприменимо| 

### <a name="note-for-on-premises-versions"></a>Примечание для локальных версий

> [!Note]
> Если вы подключаете локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] к [!INCLUDE[crm_md](includes/crm_md.md)] и хотите настроить подключение к экземпляру [!INCLUDE[crm_md](includes/crm_md.md)] с определенным типом проверки подлинности, заполните поля на экспресс-вкладке **Сведения о типе проверки подлинности**. Дополнительные сведения см. в разделе [Использование строк подключения в средстве XRM для подключения к Dynamics 365](https://go.microsoft.com/fwlink/?linkid=843055). Этот шаг не требуется при подключении к сетевой версии [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="see-also"></a>См. также

[Настройка учетных записей пользователя для интеграции с [!INCLUDE[crm_md](includes/crm_md.md)]](admin-setting-up-integration-with-dynamics-sales.md)  
[Настройка подключения к [!INCLUDE[crm_md](includes/crm_md.md)]](admin-how-to-set-up-a-dynamics-crm-connection.md)  
[Синхронизация Business Central и [!INCLUDE[crm_md](includes/crm_md.md)]](admin-synchronizing-business-central-and-sales.md)  
[Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration)
