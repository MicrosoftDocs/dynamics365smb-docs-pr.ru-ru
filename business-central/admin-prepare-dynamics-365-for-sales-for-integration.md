---
title: Интеграция с Dynamics 365 Sales | Документация Майкрософт
description: Узнайте, как подготовить Dynamics 365 Business Central к интеграции с Dynamics 365 Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, integrating
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 9f56e96b86fb7462799c9a9c655010ee2fb04381
ms.sourcegitcommit: cd5d3d288feee76d058d325720135275f4c8ad85
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/08/2019
ms.locfileid: "2775311"
---
# <a name="integrating-with-dynamics-365-sales"></a>Интеграция с Dynamics 365 Sales
Роль менеджера по продажам часто рассматривается как самая направленная наружу должность в бизнесе. Однако может быть полезно для менеджеров по продажам посмотреть внутрь бизнеса и увидеть, что происходит на заднем дворе. Путем интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)], можно предоставить менеджерам по продажи такие аналитические данные, позволив им просматривать информацию в [!INCLUDE[d365fin](includes/d365fin_md.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, при подготовке предложения по продаже может быть полезно знать, имеется ли достаточно запасов для выполнения заказа. Дополнительные сведения см. в разделе [Использование Dynamics 365 Sales из Business Central](marketing-integrate-dynamicscrm.md).

> [!NOTE]
> Эти шаги описывают процесс интеграции сетевых версий [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)]. Сведения о локальной конфигурации см. в разделе [Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration).

<!--## Software Requirements
You must have an Office 365 subscription, and both [!INCLUDE[crm_md](includes/crm_md.md)] and [!INCLUDE[d365fin](includes/d365fin_md.md)] must be part of the same organization.  -->

## <a name="overview-of-the-integration-process"></a>Обзор процесса интеграции
Следующие шаги предоставляют обзор шагов интеграции [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!Note]  
> Для этих задач требуется роль безопасности **Системный администратор** в [!INCLUDE[crm_md](includes/crm_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].  

1. В центре администрирования Office 365 настройте учетную запись пользователя для подключения и синхронизации данных с [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md).

2. Назначьте лицензии для [!INCLUDE[crm_md](includes/crm_md.md)] пользователям [!INCLUDE[d365fin](includes/d365fin_md.md)], которые будут использовать интегрированные приложения.

3. Настройте подключение к [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Настройка подключения к Dynamics 365 Sales](admin-how-to-set-up-a-dynamics-crm-connection.md),  

4. Необязательно: свяжите записи [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Дополнительные сведения см. в разделе [Связывание и синхронизация записей вручную](admin-how-to-couple-and-synchronize-records-manually.md).

5. Синхронизируйте данные между приложениями. Дополнительные сведения см. в разделе [Синхронизация Business Central и Dynamics 365 Sales](admin-synchronizing-business-central-and-sales.md).  

## <a name="about-the-business-central-integration-solution"></a>О решении интеграции Business Central
Решение позволяет людям просматривать информацию в [!INCLUDE[d365fin](includes/d365fin_md.md)] во время работы в [!INCLUDE[crm_md](includes/crm_md.md)]. Например, это может предоставить аналитические данные по статистике клиента, позволяя пользователям связывать и просматривать записи в [!INCLUDE[d365fin](includes/d365fin_md.md)] из [!INCLUDE[crm_md](includes/crm_md.md)] и позволяя людям видеть, доступны ли продукты в [!INCLUDE[d365fin](includes/d365fin_md.md)].

По умолчанию мастер настройки **Настройка подключения к Dynamics 365 Sales** импортирует решение интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)]. Для этого мастер настройки использует учетную запись пользователя-администратора. Эта учетная запись также должна принадлежать действительному пользователю [!INCLUDE[crm_md](includes/crm_md.md)] со следующими ролями безопасности:

* Системный администратор  
* Настройщик решения  

Дополнительные сведения см. в разделах [Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md), [Создание пользователей в Microsoft Dynamics 365 (online) и назначение ролей безопасности](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles) и [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).  

Эта учетная запись используется только один раз во время настройки. После импорта решения в [!INCLUDE[d365fin](includes/d365fin_md.md)] учетная запись больше не требуется. Интеграция будет продолжать использовать учетную запись пользователя, которая была создана специально для интеграции.

Помимо настройки [!INCLUDE[crm_md](includes/crm_md.md)], решение интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] также создает следующие роли в [!INCLUDE[crm_md](includes/crm_md.md)] для интеграции:

* **Администратор интеграции** — позволяет пользователям управлять подключением между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)]. Обычно назначается только учетной записи пользователя для синхронизации.  
* **Пользователь интеграции** — позволяет пользователям получать доступ к синхронизированным данным. Обычно назначается учетной записи пользователя для синхронизации и любому другому пользователю, которому необходимо просматривать синхронизированные данные или получать к ним доступ.
* **Пользователь наличия товара** — позволяет пользователям запрашивать наличие товара в [!INCLUDE[d365fin](includes/d365fin_md.md)] из [!INCLUDE[crm_md](includes/crm_md.md)].

Для получения подробной информации о каждой роли, например о разрешениях и уровнях доступа, см. в разделе [Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md).

В конце мастера настройки [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагает связать менеджеров по продаже с пользователями в [!INCLUDE[crm_md](includes/crm_md.md)]. Записи в [!INCLUDE[crm_md](includes/crm_md.md)] обычно имеют назначенного им ответственного (пользователя), и если связывание между пользователем в [!INCLUDE[crm_md](includes/crm_md.md)] и менеджером по продажам в [!INCLUDE[d365fin](includes/d365fin_md.md)] не существует, синхронизация потерпит неудачу. Это можно также сделать позже с помощью действия **Связать менеджеров по продажам** на странице **Настройка подключения Microsoft Dynamics 365**.

## <a name="see-also"></a>См. также  
[Настройка учетных записей пользователей для интеграции с Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Настройка подключения к Dynamics 365 Sales](admin-how-to-set-up-a-dynamics-crm-connection.md)  
[Синхронизация Business Central и Dynamics 365 Sales](admin-synchronizing-business-central-and-sales.md)  
[Подготовка Dynamics 365 Sales к локальной интеграции](/dynamics365/business-central/dev-itpro/administration/prepare-dynamics-365-for-sales-for-integration)
