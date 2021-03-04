---
title: Использование Microsoft Dataverse
description: Введение в Microsoft Dataverse и его компоненты.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 10/01/2020
ms.openlocfilehash: 1d740cf645739e89dddc9173583eb5fa639f6be6
ms.sourcegitcommit: edac6cbb8b19ac426f8dcbc83f0f9e308fb0d45d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/29/2020
ms.locfileid: "4817108"
---
# <a name="integrating-with-microsoft-dataverse"></a>Интеграция с Microsoft Dataverse
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

Бизнес-приложения часто используют данные из более чем одного источника. [!INCLUDE[prod_short](includes/cds_long_md.md)] объединяет данные в единый набор логики, облегчающей подключение других приложений Dynamics 365, таких как [!INCLUDE[crm_md](includes/crm_md.md)] или ваше собственное приложение, построенное на основе [!INCLUDE[prod_short](includes/cds_long_md.md)], к [!INCLUDE[prod_short_md](includes/prod_short.md)]. Для получения дополнительных сведений о [!INCLUDE[prod_short](includes/cds_long_md.md)] см. раздел [Что такое Dataverse?](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro)

Следующие шаги предоставляют обзор шагов интеграции [!INCLUDE[prod_short](includes/cds_long_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Note]  
> Для этих задач требуется роль безопасности **Системный администратор** в [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)].  

1. Назначьте лицензии для [!INCLUDE[prod_short](includes/cds_long_md.md)] пользователям [!INCLUDE[prod_short](includes/prod_short.md)], которые будут использовать интегрированные приложения.

2. Настройте подключение к [!INCLUDE[prod_short](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Подключение к Dataverse](admin-how-to-set-up-a-dynamics-crm-connection.md).  

3. Синхронизируйте данные между приложениями. Дополнительные сведения см. в разделе [Синхронизация Business Central и Dataverse](admin-synchronizing-business-central-and-sales.md). 

## <a name="getting-started-with-prod_short"></a>Приступая к работе с [!INCLUDE[prod_short](includes/cds_long_md.md)]
Чтобы начать работу с [!INCLUDE[prod_short](includes/cds_long_md.md)], вам понадобится учетная запись Microsoft Power Apps. Если у вас еще нет учетной записи Power Apps, вы можете получить его бесплатно, посетив [powerapps.com](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) и выбрав ссылку **Начать бесплатно**. Чтобы узнать больше о том, как начать работу с [!INCLUDE[prod_short](includes/cds_long_md.md)], см. модуль [Начало работы с Dataverse](https://docs.microsoft.com/learn/modules/get-started-with-powerapps-common-data-service/) от Microsoft Learn.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a>Двунаправленная или однонаправленная синхронизация данных
В зависимости от потребностей вашего бизнеса, вы можете настроить интеграцию для синхронизации данных из одного бизнес-приложения Dynamics 365 в другое или наоборот, либо в обоих направлениях в режиме, близком к режиму реального времени, через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Например, если вы интегрируете [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] через [!INCLUDE[prod_short](includes/cds_long_md.md)], продавец может создать заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], и заказ будет синхронизирован с [!INCLUDE[prod_short](includes/prod_short.md)]. И наоборот, из [!INCLUDE[crm_md](includes/crm_md.md)] продавец может просматривать информацию из [!INCLUDE[prod_short](includes/prod_short.md)] о наличии товара в заказе. 

## <a name="standard-and-custom-entities"></a>Стандартные и пользовательские объекты
[!INCLUDE[prod_short](includes/cds_long_md.md)] безопасно хранит данные в наборе таблиц, которые представляют собой наборы записей, аналогично тому, как таблица хранит данные в базе данных. [!INCLUDE[prod_short](includes/cds_long_md.md)] включает в себя базовый набор стандартных таблиц, которые охватывают типичные сценарии, но вы также можете создавать собственные таблицы, характерные для вашей организации. В [!INCLUDE[prod_short](includes/prod_short.md)] можно просмотреть стандартные и настраиваемые таблицы, синхронизируемые на странице сопоставления таблиц интеграции.

## <a name="about-the-business-central-base-integration-solution"></a>О базовом решении интеграции Business Central

Базовое решение интеграции является ключевым компонентом интеграции. Это решение добавляет необходимые роли и уровни доступа к учетным записям пользователей для интеграции и создает таблицы, необходимые для сопоставления компании [!INCLUDE[prod_short](includes/prod_short.md)] с бизнес-подразделениями в [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

По умолчанию мастер настройки **Настройка подключения [!INCLUDE[prod_short](includes/cds_long_md.md)]** импортирует интегрированное решение. Для этого мастер настройки использует учетную запись пользователя-администратора, которую вы указали. Эта учетная запись должна принадлежать действительному пользователю [!INCLUDE[prod_short](includes/cds_long_md.md)] со следующей ролью безопасности:

* Системный администратор  

Дополнительные сведения см. в разделах [Настройка учетных записей пользователей для интеграции с [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) и [Создание пользователей в Microsoft Dynamics 365 (online) и назначение ролей безопасности](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles). 

Учетная запись администратора используется только один раз во время установки для изменений конфигурации, которые базовое решение интеграции вносит в [!INCLUDE[prod_short](includes/cds_long_md.md)]. После импорта решения учетная запись больше не требуется. Интеграция будет продолжать использовать учетную запись пользователя, которая была автоматически создана специально для интеграции.

Помимо настройки [!INCLUDE[prod_short](includes/cds_long_md.md)], решение также создает следующие роли в [!INCLUDE[prod_short](includes/cds_long_md.md)] для интеграции:

* **Администратор интеграции** — позволяет пользователям управлять подключением между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[prod_short](includes/cds_long_md.md)]. Обычно она назначается только автоматически созданной учетной записи пользователя для синхронизации.  
* **Пользователь интеграции** — позволяет пользователям получать доступ к синхронизированным данным. Обычно она назначается автоматически созданной учетной записи пользователя для синхронизации и любым другим пользователя, которому необходимо просматривать синхронизированные данные или получать к ним доступ.

Для получения подробной информации о каждой роли, например о разрешениях и уровнях доступа, см. [Настройка учетных записей пользователей для интеграции с [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

Во время настройки соединения создаются сопоставления таблиц интеграции, которые необходимы для синхронизации данных. Сущности в [!INCLUDE[prod_short](includes/cds_long_md.md)] сопоставляются с таблицами и полями таблиц в Business Central посредством таблиц интеграции. Дополнительные сведения см. в разделе [Сопоставление стандартных объектов для синхронизации](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

## <a name="see-also"></a>См. также
[Модели владения данными](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Dataverse](\dynamics365\business-central\dev-itpro\administration\administration-custom-cds-integration) -->





[!INCLUDE[footer-include](includes/footer-banner.md)]