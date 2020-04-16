---
title: Настройка учетных записей пользователя для интеграции с Common Data Service | Документы Майкрософт
description: Узнайте, как настроить учетные записи пользователей, которые приложения используют для обмена данными, и что используют люди для доступа к данным в приложениях и их синхронизации.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: ad10aa53b4fe6a8b9b65ad798c206fa251e08a7a
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196499"
---
# <a name="setting-up-user-accounts-for-integrating-with-common-data-service"></a>Настройка учетных записей пользователя для интеграции с Common Data Service
Эта статья содержит обзор порядка настройки учетных записей пользователей, которые требуются для интеграции [!INCLUDE[d365fin](includes/cds_long_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="setting-up-the-administrator-user-account"></a>Настройка учетной записи пользователя-администратора
Вы должны добавить свою учетную запись администратора для [!INCLUDE[d365fin](includes/d365fin_md.md)] как пользователя в [!INCLUDE[d365fin](includes/cds_long_md.md)]. Когда вы устанавливаете подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)], мы будем использовать эту учетную запись один раз для установки и настройки некоторых необходимых компонентов. <!--Verify this-->

## <a name="setting-up-the-user-account-for-the-integration"></a>Настройка учетной записи пользователя для интеграции
Необходимо создать специальную учетную запись пользователя в вашей подписке Office 365, которую могут использовать [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)] для синхронизации данных. Данная учетная запись пользователя должна обеспечивать вход в [!INCLUDE[d365fin](includes/cds_long_md.md)], это означает, что данный пользователь должен иметь лицензию на [!INCLUDE[d365fin](includes/cds_long_md.md)] и хотя бы одну роль безопасности, назначенную ему в [!INCLUDE[d365fin](includes/cds_long_md.md)]. <!--not sure that this applies as described [here](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-user-account). For more information about how to create users in [!INCLUDE[d365fin](includes/cds_long_md.md)], see [Manage security, users, and teams](https://go.microsoft.com/fwlink/?LinkID=616518). --> После того как подключение настроено, [!INCLUDE[d365fin](includes/d365fin_md.md)] назначит учетной записи пользователя роли безопасности, которые требуются в [!INCLUDE[d365fin](includes/d365fin_md.md)].

<!--![Assisted setup guide showing place to enter synchronization user credentials](media/sync-user-setup.png "Visualization assisted setup wizard page showing place to enter synchronization user credentials")-->

> [!IMPORTANT]  
> Не используйте учетную запись администратора для [!INCLUDE[d365fin](includes/cds_long_md.md)] для синхронизации. Если это сделать, синхронизация будет нарушена.

## <a name="permissions-and-security-roles-for-user-accounts-in-d365fin"></a>Разрешения и роли безопасности для учетных записей пользователей в [!INCLUDE[d365fin](includes/cds_long_md.md)]
При установке базового решения интеграции CDS разрешения для учетной записи пользователя интеграции настраиваются. Если эти разрешения изменены, вам может потребоваться сбросить их. Вы можете сделать это, переустановив базовое решение интеграции CDS, выбрав **Повторить развертывание решения интеграции** на странице **Настройка подключения Common Data Service**. Роль безопасности интеграции Business Central CDS развернута.


<!--
The following tables list the minimum permissions for the user accounts in [!INCLUDE[d365fin](includes/cds_long_md.md)].

### Minimum Permissions for the Administrator
The following table displays the minimum permissions on each tab for each security role that is required for the administrator user.

##### Customization
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

##### Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2020|
|----|----|-----|----|----|
|Business Central Account Statistics|Global|Read|Read|Read|
|Business Central Connection|Global|Create, Read, Write, Delete|Create, Read, Write, Delete|Create, Read, Write, Delete|
|Post Configuration|Global|||Write|

#### Integration User
The following table displays the minimum permissions on each tab for each security role that is required for the integration user.

##### Core Records
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

##### Sales
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Invoice|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Order|Global|Read, Write, Append To|Read, Write, Append To|Read, Write, Append, Append To, Assign|
|Product|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|Property|Global|Read|Read|Read|
|Property Association|Global|Read|Read|Read|
|Property Option Set Item|Global|Read|Read|Read|
|Quote|Global|Read|Read|Read|

##### Service
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Case|Global|Read|Read|Read|

##### Business Management
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Currency|Global|Create, Read, Write|Create, Read, Write|Create, Read, Write|
|Organization|Global|Read, Write|Read, Write|Read, Write|
|Security Role|Global|||Read|
|User|Global|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|Create, Read, Write, Append, Append To|
|User Settings|Global|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|Create, Read, Write, Delete, Append To|
|Act on Behalf of Another User|Global|Yes|Yes|Yes|

##### Customization
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Field|Global||Read|Read|
|Plug-in Assembly|Global|Read|Read|Read|
|Plug-in Type|Global|Read|Read|Read|
|SDK Message|Global|Read|Read|Read|
|SDK Message Processing Step|Global|Read|Read|Read|
|Web Resource|Global|Read|Read|Read|

##### Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

### Product Availability User
You can allow sales people to view inventory levels for the items they sell by granting them the permissions described in the following table.

##### Custom Entities
|Security Role|Access Level|Dynamics NAV 2018 and Earlier|Business Central <br> October 2018|Business Central <br> April 2019|
|----|----|-----|----|----|
|Dynamics 365 Business Central Account Statistics|Global|Create, Read, Write, Append To|Create, Read, Write, Append To|Create, Read, Write, Append To|
|Dynamics 365 Business Central Connection|Global|Read|Read|Read|

-->

## <a name="see-also"></a>См. также  
[Интеграция с Common Data Service](admin-common-data-service.md)  
[Интеграция с Dynamics 365 Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
