---
title: Интеграция с Dynamics 365 for Sales | Документы Майкрософт
description: Узнайте, как подготовить Dynamics 365 Business Central для интеграции с Dynamics 365 for Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 991d8432c24b1963da019e3c8b665f9ad009d077
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1247284"
---
# <a name="integrating-with-dynamics-365-for-sales"></a>Интеграция с Dynamics 365 for Sales
Роль менеджера по продажам часто рассматривается как самая направленная наружу должность в бизнесе. Однако может быть полезно для менеджеров по продажам посмотреть внутрь бизнеса и увидеть, что происходит на заднем дворе. Путем интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], можно предоставить менеджерам по продажи такие аналитические данные, позволив им просматривать информацию в [!INCLUDE[d365fin](includes/d365fin_md.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, при подготовке предложения по продаже может быть полезно знать, имеется ли достаточно запасов для выполнения заказа. Дополнительные сведения см. в разделе [Использование Dynamics 365 for Sales из Business Central](marketing-integrate-dynamicscrm.md).

> [!Note]
> Эти шаги описывают процесс интеграции сетевых версий [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].

<!--## Software Requirements
You must have an Office 365 subscription, and both [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)] must be part of the same organization.  -->

## <a name="overview-of-the-integration-process"></a>Обзор процесса интеграции
Следующие шаги предоставляют обзор шагов интеграции [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!Note]  
> Для этих задач требуется роль безопасности **Системный администратор** в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].  

1. В центре администрирования Office 365 настройте учетную запись пользователя для подключения и синхронизации данных с [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Настройка интеграции с Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md).

2. Назначьте лицензии для [!INCLUDE[crm_md](includes/crm_md.md)] пользователям [!INCLUDE[d365fin](includes/d365fin_md.md)], которые будут использовать интегрированные приложения.

3. Настройте подключение к [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Настройка подключения к Dynamics 365 for Sales](admin-how-to-set-up-a-dynamics-crm-connection.md).  

4. Необязательно: свяжите записи [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md).

5. Синхронизируйте данные между приложениями. Дополнительные сведения см. в разделе [Синхронизация Business Central и Dynamics 365 for Sales](admin-synchronizing-business-central-and-sales.md).  

## <a name="about-the-business-central-integration-solution"></a>О решении интеграции Business Central
Решение позволяет людям просматривать информацию в [!INCLUDE[d365fin](includes/d365fin_md.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, это может предоставить аналитические данные по статистике клиента, позволяя пользователям связывать и просматривать записи в [!INCLUDE[d365fin](includes/d365fin_md.md)] из [!INCLUDE[crm_md](includes/crm_md.md)] и позволяя людям видеть, доступны ли продукты в [!INCLUDE[d365fin](includes/d365fin_md.md)].

По умолчанию мастер настройки подключения к Dynamics 365 for Sales импортирует интегрированное решение [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для этого мастер настройки использует учетную запись пользователя-администратора. Эта учетная запись также должна принадлежать действительному пользователю [!INCLUDE[crm_md](includes/crm_md.md)] со следующими ролями безопасности:

* Системный администратор  
* Настройщик решения  

Дополнительные сведения см. в разделах [Настройка учетных записей пользователей для интеграции с Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md), [Создание пользователей в Microsoft Dynamics 365 (online) и назначение ролей безопасности](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles.md) и [Управление пользователями и разрешениями](ui-how-users-permissions.md).  

Эта учетная запись используется только один раз во время настройки. После импорта решения в [!INCLUDE[d365fin](includes/d365fin_md.md)] учетная запись больше не требуется. Интеграция будет продолжать использовать учетную запись пользователя, которая была создана специально для интеграции.

Помимо настройки [!INCLUDE[crm_md](includes/crm_md.md)], решение интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] также создает следующие роли в [!INCLUDE[crm_md](includes/crm_md.md)] для интеграции:

* **Администратор интеграции** — позволяет пользователям управлять подключением между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Обычно назначается только учетной записи пользователя для синхронизации.  
* **Пользователь интеграции** — позволяет пользователям получать доступ к синхронизированным данным. Обычно назначается учетной записи пользователя для синхронизации и любому другому пользователю, которому необходимо просматривать синхронизированные данные или получать к ним доступ.
* **Пользователь наличия товара** — позволяет пользователям запрашивать наличие товара в [!INCLUDE[d365fin](includes/d365fin_md.md)] из [!INCLUDE[crm_md](includes/crm_md.md)].

В конце мастера настройки [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагает связать менеджеров по продаже с пользователями в [!INCLUDE[crm_md](includes/crm_md.md)]. Записи в [!INCLUDE[crm_md](includes/crm_md.md)] обычно имеют назначенного им ответственного (пользователя), и если связывание между пользователем в [!INCLUDE[crm_md](includes/crm_md.md)] и менеджером по продажам в [!INCLUDE[d365fin](includes/d365fin_md.md)] не существует, синхронизация потерпит неудачу. Это можно также сделать позже с помощью действия **Связать менеджеров по продажам** на странице **Настройка подключения Microsoft Dynamics 365**.

## <a name="see-also"></a>См. также  
[Настройка учетных записей пользователя для интеграции с Dynamics 365 for Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Настройка подключения к Dynamics 365 for Sales](admin-how-to-set-up-a-dynamics-crm-connection.md)
[Синхронизация Business Central и Dynamics 365 for Sales](admin-synchronizing-business-central-and-sales.md)
