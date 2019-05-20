---
title: Настройка учетных записей пользователя для интеграции с Dynamics 365 for Sales | Документы Майкрософт
description: Узнайте, как настроить учетные записи пользователей, которые приложения используют для обмена данными, и что используют люди для доступа к данным в приложениях и их синхронизации.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: c318346c62b7776a550a77a2947173e33d5f17c0
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1246578"
---
# <a name="setting-up-user-accounts-for-integrating-with-dynamics-365-for-sales"></a>Настройка учетных записей пользователя для интеграции с Dynamics 365 for Sales
Эта статья содержит обзор порядка настройки учетных записей пользователей, которые требуются для интеграции [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)].  

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2085500]

## <a name="setting-up-the-admininstrator-user-account-in-sales"></a>Настройка учетной записи пользователя-администратора в Sales
Необходимо добавить учетную запись пользователя-администратора для [!INCLUDE[d365fin](includes/d365fin_md.md)] как пользователя в [!INCLUDE[crm_md](includes/crm_md.md)], а затем повысить пользователя до администратора в [!INCLUDE[crm_md](includes/crm_md.md)]. Учетная запись пользователя-администратора должна также включать роль специалиста по настройке системы и по крайней мере одну неадминистративную роль пользователя, такую как менеджер по продажам, в [!INCLUDE[crm_md](includes/crm_md.md)].

## <a name="setting-up-the-user-account-for-the-integration"></a>Настройка учетной записи пользователя для интеграции
Необходимо создать специальную учетную запись пользователя в вашей подписке Office 365, которую могут использовать [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)] для синхронизации данных. Данная учетная запись пользователя должна иметь возможность выполнять вход в [!INCLUDE[crm_md](includes/crm_md.md)], что означает, что этот пользователь должен иметь лицензию для [!INCLUDE[crm_md](includes/crm_md.md)]. Эта учетная запись также должна быть неинтерактивной учетной записью в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения о том, как создавать пользователей в [!INCLUDE[crm_md](includes/crm_md.md)], см. в разделе [Управление безопасностью, пользователями и рабочими группами](http://go.microsoft.com/fwlink/?LinkID=616518). После того как подключение настроено, [!INCLUDE[d365fin](includes/d365fin_md.md)] назначит учетной записи пользователя роли безопасности, которые требуются в [!INCLUDE[d365fin](includes/d365fin_md.md)].

![Мастер настройки, в котором показано место для ввода учетных данных пользователя синхронизации](media/sync-user-setup.png "Визуализация страница мастера настройки, в котором показано место для ввода учетных данных пользователя синхронизации")

> [!IMPORTANT]  
> Не используйте учетную запись администратора для [!INCLUDE[crm_md](includes/crm_md.md)] для синхронизации. Если это сделать, синхронизация будет нарушена.
> Кроме того, чтобы избежать постоянной синхронизации, изменения данных, которые вносятся учетной записью пользователя интеграции не синхронизируются. <!--What changes would this account make?--> После установления подключения рекомендуется настроить режим доступа для учетной записи пользователя для интеграции на неинтерактивный режим в [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Создание неинтерактивной учетной записи пользователя](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#create-a-non-interactive-user-account).

## <a name="setting-up-accounts-for-sales-people"></a>Настройка учетных записей для менеджеров по продаже
Следует создать учетные записи пользователей в [!INCLUDE[d365fin](includes/d365fin_md.md)] для менеджеров по продажам из [!INCLUDE[crm_md](includes/crm_md.md)]. Чтобы упростить эту операцию, центр администрирования Microsoft 365 предлагает шаблон Excel, который можно использовать. На странице **Активные пользователи** выберите **Дополнительно**, затем — **Импорт нескольких пользователей**. Выберите **Загрузить только CSV-файл с заголовками**, затем введите информацию для менеджеров по продажам. Чтобы посмотреть пример, выберите **Загрузить CSV-файл с заголовками и примерами сведений о пользователях**. После ввода информации о пользователях, следующим шагом процесса импорта будет назначить пользователям лицензии план Dynamics 365 Customer Engagement.  

После импорта пользователей и назначения им лицензий для Dynamics 365 Customer Engagement необходимо назначить пользователей роли **Менеджер по продажам** в [!INCLUDE[crm_md](includes/crm_md.md)].

![Связывание менеджеров по продажам с пользователями в Dynamics 365 for Sales](media/couple-salespeople.png "Визуализация связывания менеджеров по продажам с пользователями в Dynamics 365 for Sales")

## <a name="see-also"></a>См. также  
[Интеграция с Dynamics 365 for Sales](admin-prepare-dynamics-365-for-sales-for-integration.md)  
