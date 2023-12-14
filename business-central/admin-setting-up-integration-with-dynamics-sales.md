---
title: Настройка учетных записей пользователя для интеграции с Microsoft Dataverse | Документы Майкрософт
description: 'Узнайте, как настроить учетные записи пользователей, которые приложения используют для обмена данными, и что используют люди для доступа к данным в приложениях и их синхронизации.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: bholtorf
---
# <a name="setting-up-user-accounts-for-integrating-with-microsoft-dataverse-via-data-sync"></a>Настройка учетных записей пользователя для интеграции с Microsoft Dataverse путем синхронизации данных

Эта статья содержит обзор порядка настройки учетных записей пользователей, которые требуются для интеграции [!INCLUDE[prod_short](includes/cds_long_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="set-up-the-administrator-user-account"></a>Настройка учетной записи пользователя-администратора

Для настройки подключения между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)] вы должны войти в [!INCLUDE[prod_short](includes/prod_short.md)] с учетной записью пользователя, которой назначена лицензия [!INCLUDE[prod_short](includes/prod_short.md)] Essential или [!INCLUDE[prod_short](includes/prod_short.md)] Premium. Эта учетная запись будет использоваться однократно для установки и настройки некоторых необходимых компонентов.

> [!IMPORTANT]
> Во время установки вам будет предложено ввести учетные данные для среды [!INCLUDE[prod_short](includes/cds_long_md.md)]. Укажите учетные данные учетной записи, которая является лицензированным пользователем и назначена роли безопасности **Системный администратор** в среде [!INCLUDE[prod_short](includes/cds_long_md.md)] и роли глобального администратора в арендаторе, к которому относится среда. Этой учетной записи не требуется лицензия на [!INCLUDE[prod_short](includes/prod_short.md)], так как она будет использоваться только для выполнения задач настройки в среде [!INCLUDE[prod_short](includes/cds_long_md.md)].
>
> По завершении настройки подключения этого пользователя [!INCLUDE[prod_short](includes/cds_long_md.md)] можно будет удалить. Интеграция будет продолжать использовать учетную запись пользователя, которая была автоматически создана специально для интеграции.

## <a name="permissions-and-security-roles-for-user-accounts-in-"></a>Разрешения и роли безопасности для учетных записей пользователей в [!INCLUDE[prod_short](includes/cds_long_md.md)]

Базовое решение интенрации создает для интеграции следующе роли в [!INCLUDE[cds_long](includes/cds_long_md.md)]:

* **Администратор интеграции** — позволяет пользователям управлять подключением между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[cds_long](includes/cds_long_md.md)]. Обычно она назначается только автоматически созданной учетной записи пользователя для синхронизации.
* **Пользователь интеграции** — позволяет пользователям получать доступ к синхронизированным данным. Обычно она назначается автоматически созданной учетной записи пользователя для синхронизации и любым другим пользователя, которому необходимо просматривать синхронизированные данные или получать к ним доступ.

> [!NOTE]
>
> Роли **Администратор интеграции**и **Пользователь интеграции** должны использоваться только пользователем приложения, который запускает интеграцию. Пользователю приложения не требуется назначенная лицнензия на [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[cds_long](includes/cds_long_md.md)].

Когда вы устанавливаете базовое решение интеграции, оно настраивает разрешения для учетной записи пользователя интеграции. Если эти разрешения были изменены вручную, их можно сбросить. На странице **Настройка подключения к Dataverse** выберите **Повторить развертывание решения интеграции**, чтобы переустановить базовое решение интеграции. В рамках этого действия будет развернута роль безопасности "Интеграция Business Central".

<!--
The following tables list the minimum permissions for the user accounts in [!INCLUDE[prod_short](includes/cds_long_md.md)].

### <a name="minimum-permissions-for-the-administrator"></a>Minimum Permissions for the Administrator
The following table displays the minimum permissions on each tab for each security role that is required for the administrator user.

##### <a name="customization"></a>Customization
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Model Driven App|Global|||Read|
|Plugin Assembly|Global|Read|Read|Read|
|Plugin Type|Global|Read|Read|Read|
|Relationship|Global|||Read|
|SDK Message|Global|Read|Read|Read|
|SDK Message Proessing Step|Global|Read|Read|Read|
|SDK Message Proessing Step Image|Global|Read|Read|Read|
|System From|Global|||Write|

##### <a name="custom-entities"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2020|
|----|----|-----|----|----|
|Business Central Account Statistics|Global|Read|Read|Read|
|Business Central Connection|Global|Create, Read, Write, Delete|Create, Read, Write, Delete|Create, Read, Write, Delete|
|Post Configuration|Global|||Write|

### <a name="minimum-permissions-for-automatically-created--integration-application-user"></a>Minimum Permissions for automatically created [!INCLUDE[prod_short](includes/prod_short.md)] Integration application user
The following table displays the minimum permissions on each tab for each security role that is required for the automatically created [!INCLUDE[prod_short](includes/prod_short.md)] Integration application user.

##### <a name="core-records"></a>Core Records
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Account|Global|Create, Read, Write, Append, Append To, Assign|Create, Read, Write, Append, Append To, Assign|Create, Read, Write, Append, Append To, Assign|
|Action Card|Global||Read|Read|
|Connection|Global|Read|Read|Read|
|Contact|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Note|Global|||Create, Read, Write, Delete Append, Assign|
|Opportunity|Global||Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Post|Global|||Create, Read, Append To|
|User Entity UI|User|Create, Read, Write|Create, Read, Write|Create, Read, Write|

##### <a name="sales"></a>Sales
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Invoice|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Order|Global|Read, Write, Append To|Read, Write, Append To|Read, Write, Append, Append To, Assign|
|Product|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Property|Global|Read|Read|Read|
|Property Association|Global|Read|Read|Read|
|Property Option Set Item|Global|Read|Read|Read|
|Quote|Global|Read|Read|Read|

##### <a name="service"></a>Service
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Case|Global|Read|Read|Read|

##### <a name="business-management"></a>Business Management
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Currency|Global|Create, Read, Write|Create, Read, Write|Create, Read, Write|
|Organization|Global|Read, Write|Read, Write|Read, Write|
|Security Role|Global|||Read|
|User|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|User Settings|Global|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|
|Act on Behalf of Another User|Global|Yes|Yes|Yes|

##### <a name="customization-1"></a>Customization
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Field|Global||Read|Read|
|Plug-in Assembly|Global|Read|Read|Read|
|Plug-in Type|Global|Read|Read|Read|
|SDK Message|Global|Read|Read|Read|
|SDK Message Processing Step|Global|Read|Read|Read|
|Web Resource|Global|Read|Read|Read|

##### <a name="custom-entities-1"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

### <a name="product-availability-user"></a>Product Availability User
You can allow sales people to view inventory levels for the items they sell by granting them the permissions described in the following table.

##### <a name="custom-entities-2"></a>Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

-->

## <a name="see-also"></a>См. также

[Интеграция с Microsoft Dataverse](admin-common-data-service.md)  
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
