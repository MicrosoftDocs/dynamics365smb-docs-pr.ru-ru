---
title: Настройка учетных записей пользователя для интеграции с Microsoft Dataverse | Документы Майкрософт
description: Узнайте, как настроить учетные записи пользователей, которые приложения используют для обмена данными, и что используют люди для доступа к данным в приложениях и их синхронизации.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 1699d10a0d01d2143f26fe59313d6ba073272eef
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5385253"
---
# <a name="setting-up-user-accounts-for-integrating-with-microsoft-dataverse"></a><span data-ttu-id="9a9bc-103">Настройка учетных записей пользователя для интеграции с Microsoft Dataverse</span><span class="sxs-lookup"><span data-stu-id="9a9bc-103">Setting Up User Accounts for Integrating with Microsoft Dataverse</span></span>
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

<span data-ttu-id="9a9bc-104">Эта статья содержит обзор порядка настройки учетных записей пользователей, которые требуются для интеграции [!INCLUDE[prod_short](includes/cds_long_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="9a9bc-104">This article provides an overview of how to set up the user accounts that are required to integrate [!INCLUDE[prod_short](includes/cds_long_md.md)] with [!INCLUDE[prod_short](includes/prod_short.md)].</span></span>  

## <a name="setting-up-the-administrator-user-account"></a><span data-ttu-id="9a9bc-105">Настройка учетной записи пользователя-администратора</span><span class="sxs-lookup"><span data-stu-id="9a9bc-105">Setting Up the Administrator User Account</span></span>
<span data-ttu-id="9a9bc-106">Вы должны добавить свою учетную запись администратора для [!INCLUDE[prod_short](includes/prod_short.md)] как пользователя в [!INCLUDE[prod_short](includes/cds_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="9a9bc-106">You must add your administrator user account for [!INCLUDE[prod_short](includes/prod_short.md)] as a user in [!INCLUDE[prod_short](includes/cds_long_md.md)].</span></span> <span data-ttu-id="9a9bc-107">Когда вы устанавливаете подключение между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)], мы будем использовать эту учетную запись один раз для установки и настройки некоторых необходимых компонентов.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-107">When you set up the connection between [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[prod_short](includes/cds_long_md.md)] we will use this account one time to install and configure some required components.</span></span> 

## <a name="permissions-and-security-roles-for-user-accounts-in-prod_short"></a><span data-ttu-id="9a9bc-108">Разрешения и роли безопасности для учетных записей пользователей в [!INCLUDE[prod_short](includes/cds_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="9a9bc-108">Permissions and Security Roles for User Accounts in [!INCLUDE[prod_short](includes/cds_long_md.md)]</span></span>
<span data-ttu-id="9a9bc-109">При установке базового решения интеграции CDS разрешения для учетной записи пользователя интеграции настраиваются.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-109">When you install the CDS Base Integration Solution, permissions for the integration user account are configured.</span></span> <span data-ttu-id="9a9bc-110">Если эти разрешения изменены вручную, можно сбросить их.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-110">If those permissions are changed manually you can reset them.</span></span> <span data-ttu-id="9a9bc-111">Вы можете сделать это, переустановив базовое решение интеграции CDS, выбрав **Повторить развертывание решения интеграции** на странице **Настройка подключения Common Data Service**.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-111">You can do that by reinstalling the CDS Base Integration Solution by choosing **Redeploy Integration Solution** on the **Common Data Service Connection Setup** page.</span></span> <span data-ttu-id="9a9bc-112">Роль безопасности интеграции Business Central CDS развернута.</span><span class="sxs-lookup"><span data-stu-id="9a9bc-112">The Business Central CDS Integration security role is deployed.</span></span>

<!--
The following tables list the minimum permissions for the user accounts in [!INCLUDE[prod_short](includes/cds_long_md.md)].

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

### Minimum Permissions for automatically created [!INCLUDE[prod_short](includes/prod_short.md)] Integration application user
The following table displays the minimum permissions on each tab for each security role that is required for the automatically created [!INCLUDE[prod_short](includes/prod_short.md)] Integration application user.

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

## <a name="see-also"></a><span data-ttu-id="9a9bc-113">См. также</span><span class="sxs-lookup"><span data-stu-id="9a9bc-113">See Also</span></span>  
[<span data-ttu-id="9a9bc-114">Интеграция с Microsoft Dataverse</span><span class="sxs-lookup"><span data-stu-id="9a9bc-114">Integrating with Microsoft Dataverse</span></span>](admin-common-data-service.md)  
[<span data-ttu-id="9a9bc-115">Интеграция с Dynamics 365 Sales</span><span class="sxs-lookup"><span data-stu-id="9a9bc-115">Integrating with Dynamics 365 Sales</span></span>](admin-prepare-dynamics-365-for-sales-for-integration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]