---
title: Использование Common Data Service
description: Введение в Common Data Service и его компоненты.
author: bholtorf
ms.author: bholtorf
ms.custom: na
ms.reviewer: na
ms.service: dynamics365-business-central
ms.topic: article
ms.date: 10/01/2020
ms.openlocfilehash: 85823e93b1d239bf4e59ec6a8872cdc4a2cef9c1
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911584"
---
# <a name="integrating-with-common-data-service"></a>Интеграция с Common Data Service

Бизнес-приложения часто используют данные из более чем одного источника. [!INCLUDE[d365fin](includes/cds_long_md.md)] объединяет данные в единый набор логики, облегчающей подключение других приложений Dynamics 365, таких как [!INCLUDE[crm_md](includes/crm_md.md)] или ваше собственное приложение, построенное на основе [!INCLUDE[d365fin](includes/cds_long_md.md)], к [!INCLUDE[d365fin_md](includes/d365fin_md.md)]. Для получения дополнительных сведений о [!INCLUDE[d365fin](includes/cds_long_md.md)] см. раздел [Что такое Common Data Service?](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro)

Следующие шаги предоставляют обзор шагов интеграции [!INCLUDE[d365fin](includes/cds_long_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)].

> [!Note]  
> Для этих задач требуется роль безопасности **Системный администратор** в [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)].  

1. Назначьте лицензии для [!INCLUDE[d365fin](includes/cds_long_md.md)] пользователям [!INCLUDE[d365fin](includes/d365fin_md.md)], которые будут использовать интегрированные приложения.

2. Настройте подключение к [!INCLUDE[d365fin](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Подключение к Common Data Service](admin-how-to-set-up-a-dynamics-crm-connection.md).  

3. Синхронизируйте данные между приложениями. Дополнительные сведения см. в разделе [Синхронизация Business Central и Common Data Service](admin-synchronizing-business-central-and-sales.md). 

## <a name="getting-started-with-d365fin"></a>Приступая к работе с [!INCLUDE[d365fin](includes/cds_long_md.md)]
Чтобы начать работу с [!INCLUDE[d365fin](includes/cds_long_md.md)], вам понадобится учетная запись Microsoft Power Apps. Если у вас еще нет учетной записи Power Apps, вы можете получить его бесплатно, посетив [powerapps.com](https://web.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) и выбрав ссылку **Начать бесплатно**. Чтобы узнать больше о том, как начать работу с [!INCLUDE[d365fin](includes/cds_long_md.md)], см. модуль [Начало работы с Common Data Service](https://docs.microsoft.com/learn/modules/get-started-with-powerapps-common-data-service/) от Microsoft Learn.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a>Двунаправленная или однонаправленная синхронизация данных
В зависимости от потребностей вашего бизнеса, вы можете настроить интеграцию для синхронизации данных из одного бизнес-приложения Dynamics 365 в другое или наоборот, либо в обоих направлениях в режиме, близком к режиму реального времени, через [!INCLUDE[d365fin](includes/cds_long_md.md)]. Например, если вы интегрируете [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] через [!INCLUDE[d365fin](includes/cds_long_md.md)], продавец может создать заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], и заказ будет синхронизирован с [!INCLUDE[d365fin](includes/d365fin_md.md)]. И наоборот, из [!INCLUDE[crm_md](includes/crm_md.md)] продавец может просматривать информацию из [!INCLUDE[d365fin](includes/d365fin_md.md)] о наличии товара в заказе. 

## <a name="standard-and-custom-entities"></a>Стандартные и пользовательские объекты
[!INCLUDE[d365fin](includes/cds_long_md.md)] безопасно хранит данные в наборе объектов, которые представляют собой наборы записей, аналогично тому, как таблица хранит данные в базе данных. [!INCLUDE[d365fin](includes/cds_long_md.md)] включает в себя базовый набор стандартных объектов, которые охватывают типичные сценарии, но вы также можете создавать собственные объекты, характерные для вашей организации. В [!INCLUDE[d365fin](includes/d365fin_md.md)] можно просмотреть стандартные и настраиваемые объекты, синхронизируемые на странице сопоставления таблиц интеграции.

## <a name="about-the-base-cds-integration-solution"></a>О базовом решении интеграции CDS

Базовое решение интеграции CDS является ключевым компонентом интеграции. Это решение добавляет необходимые роли и уровни доступа к учетным записям пользователей для интеграции и создает объекты, необходимые для сопоставления компании [!INCLUDE[d365fin](includes/d365fin_md.md)] с бизнес-подразделениями в [!INCLUDE[d365fin](includes/cds_long_md.md)]. 

По умолчанию мастер настройки **Настройка подключения [!INCLUDE[d365fin](includes/cds_long_md.md)]** импортирует интегрированное решение. Для этого мастер настройки использует учетную запись пользователя-администратора, которую вы указали. Эта учетная запись должна принадлежать действительному пользователю [!INCLUDE[d365fin](includes/cds_long_md.md)] со следующей ролью безопасности:

* Системный администратор  

Дополнительные сведения см. в разделах [Настройка учетных записей пользователей для интеграции с [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) и [Создание пользователей в Microsoft Dynamics 365 (online) и назначение ролей безопасности](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles). 

Учетная запись администратора используется только один раз во время установки из-за изменений конфигурации, которые базовое решение CDS вносит в [!INCLUDE[d365fin](includes/cds_long_md.md)]. После импорта решения учетная запись больше не требуется. Интеграция будет продолжать использовать учетную запись пользователя, которая была автоматически создана специально для интеграции.

Помимо настройки [!INCLUDE[d365fin](includes/cds_long_md.md)], решение также создает следующие роли в [!INCLUDE[d365fin](includes/cds_long_md.md)] для интеграции:

* **Администратор интеграции** — позволяет пользователям управлять подключением между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)]. Обычно она назначается только автоматически созданной учетной записи пользователя для синхронизации.  
* **Пользователь интеграции** — позволяет пользователям получать доступ к синхронизированным данным. Обычно она назначается автоматически созданной учетной записи пользователя для синхронизации и любым другим пользователя, которому необходимо просматривать синхронизированные данные или получать к ним доступ.

Для получения подробной информации о каждой роли, например о разрешениях и уровнях доступа, см. [Настройка учетных записей пользователей для интеграции с [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

Во время настройки соединения создаются сопоставления таблиц интеграции, которые необходимы для синхронизации данных. Сущности в Common Data Service сопоставляются с таблицами и полями таблиц в Business Central посредством таблиц интеграции. Дополнительные сведения см. в разделе [Сопоставление стандартных объектов для синхронизации](admin-synchronizing-business-central-and-sales.md#standard-entity-mapping-for-synchronization).

## <a name="see-also"></a>См. также
[Модели владения данными](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Common Data Service](docs.microsoft.com/en-us/dynamics365/business-central/dev-itpro/administration/administration-custom-cds-integration) -->



