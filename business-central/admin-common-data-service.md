---
title: Интеграция с Microsoft Dataverse посредством синхронизации данных
description: 'Введение в то, как интегрировать и использовать Microsoft Dataverse и его компоненты для подключения к другим приложениям Dynamics 365.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.date: 03/08/2024
ms.custom: bap-template
ms.search.form: 7214_Primary
ms.service: dynamics-365-business-central
---

# <a name="integrate-with-microsoft-dataverse-via-data-sync"></a>Интеграция с Microsoft Dataverse посредством синхронизации данных

Бизнес-приложения часто используют данные из более чем одного источника. [!INCLUDE[prod_short](includes/cds_long_md.md)] объединяет данные в единый набор логики, облегчающей подключение [!INCLUDE[prod_short](includes/prod_short.md)] к другим приложениям Dynamics 365. Например, [!INCLUDE[crm_md](includes/crm_md.md)] или ваше собственное приложение, созданное на основе [!INCLUDE[prod_short](includes/cds_long_md.md)]. Подробнее о [!INCLUDE[prod_short](includes/cds_long_md.md)] см. в разделе [Что такое Dataverse?](/powerapps/maker/common-data-service/data-platform-intro).

Следующие шаги предоставляют обзор шагов интеграции [!INCLUDE[prod_short](includes/cds_long_md.md)] с [!INCLUDE[prod_short](includes/prod_short.md)].

> [!Note]  
> Для этих задач требуется роль безопасности **Системный администратор** в [!INCLUDE[prod_short](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)].  

1. Назначьте лицензии для [!INCLUDE[prod_short](includes/cds_long_md.md)] пользователям [!INCLUDE[prod_short](includes/prod_short.md)], которые будут использовать интегрированные приложения.

2. Настройте подключение к [!INCLUDE[prod_short](includes/cds_long_md.md)]. Дополнительные сведения см. в разделе [Подключение к Dataverse](admin-how-to-set-up-a-dynamics-crm-connection.md).  

3. Синхронизируйте данные между приложениями. Дополнительные сведения см. в разделе [Синхронизация Business Central и Dataverse](admin-synchronizing-business-central-and-sales.md). 

## <a name="get-started-with-"></a>Начало работы с [!INCLUDE[prod_short](includes/cds_long_md.md)]

Чтобы начать работу с [!INCLUDE[prod_short](includes/cds_long_md.md)], вам понадобится учетная запись Microsoft Power Apps. Если у вас еще нет учетной записи Power Apps, вы можете получить его бесплатно, посетив [powerapps.com](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc) и выбрав ссылку **Начать бесплатно**. Чтобы узнать больше о том, как начать работу с [!INCLUDE[prod_short](includes/cds_long_md.md)], перейдите в модуль [Начало работы с Dataverse](/training/modules/get-started-with-powerapps-common-data-service/) из обучения Microsoft.

## <a name="bi-directional-or-uni-directional-data-synchronization"></a>Двунаправленная или однонаправленная синхронизация данных

Вы можете синхронизировать данные из одного бизнес-приложения Dynamics 365 в другое или наоборот, либо в обоих направлениях в режиме, близком к режиму реального времени, через [!INCLUDE[prod_short](includes/cds_long_md.md)]. Например, если вы интегрируете [!INCLUDE[prod_short](includes/prod_short.md)] с [!INCLUDE[crm_md](includes/crm_md.md)], продавец может создать заказ на продажу в [!INCLUDE[crm_md](includes/crm_md.md)], и заказ синхронизируется с [!INCLUDE[prod_short](includes/prod_short.md)]. И наоборот, из [!INCLUDE[crm_md](includes/crm_md.md)] продавец может проверить наличие номенклатуры из заказа в [!INCLUDE[prod_short](includes/prod_short.md)]. 

## <a name="standard-and-custom-entities"></a>Стандартные и пользовательские сущности

[!INCLUDE[prod_short](includes/cds_long_md.md)] безопасно хранит данные в наборе таблиц, которые представляют собой наборы записей, аналогично тому, как таблица хранит данные в базе данных. [!INCLUDE[prod_short](includes/cds_long_md.md)] включает в себя базовый набор стандартных таблиц, которые охватывают типичные сценарии, но вы также можете создавать собственные таблицы, характерные для вашей организации. В [!INCLUDE[prod_short](includes/prod_short.md)] можно просмотреть стандартные и настраиваемые таблицы, синхронизируемые на странице сопоставления таблиц интеграции.

## <a name="about-the-business-central-base-integration-solution"></a>О базовом решении интеграции Business Central

Базовое решение интеграции является ключевым компонентом интеграции. Это решение добавляет необходимые роли и уровни доступа к учетным записям пользователей для интеграции и создает таблицы, необходимые для сопоставления компании [!INCLUDE[prod_short](includes/prod_short.md)] с бизнес-подразделениями в [!INCLUDE[prod_short](includes/cds_long_md.md)]. 

По умолчанию мастер настройки **Настройка подключения [!INCLUDE[prod_short](includes/cds_long_md.md)]** импортирует интегрированное решение. Для этого мастер настройки использует учетную запись пользователя-администратора, которую вы указали. Эта учетная запись должна принадлежать действительному пользователю [!INCLUDE[prod_short](includes/cds_long_md.md)] с ролью безопасности **Системный администратор**.  

Чтобы узнать больше об учетных записях пользователей, перейдите к следующим статьям:

* [Настройка учетных записей пользователя для интеграции с [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md) 
* [Создание пользователей в Microsoft Dynamics 365 (online) и назначение ем ролей безопасности](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles) 

Учетная запись администратора используется только один раз во время установки для изменений конфигурации, которые базовое решение интеграции вносит в [!INCLUDE[prod_short](includes/cds_long_md.md)]. После импорта решения учетная запись больше не требуется. Интеграция будет продолжать использовать учетную запись пользователя, которая была автоматически создана специально для интеграции.

Помимо настройки [!INCLUDE [cds_long_md](includes/cds_long_md.md)], решение также создает в [!INCLUDE [cds_long_md](includes/cds_long_md.md)] роль безопасности для интеграции:

* **Интеграция Business Central с Dataverse**: позволяет управлять подключением между [!INCLUDE [prod_short](includes/prod_short.md)] и [!INCLUDE [cds_long_md](includes/cds_long_md.md)]. Обычно эта роль назначается только учетной записи пользователя, автоматически созданной для синхронизации. Чтобы узнать больше об этой роли, см. статью [Настройка учетных записей пользователей для интеграции с [!INCLUDE[prod_short](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).

Когда вы настраиваете подключение, вы создаете сопоставления таблиц интеграции, которые необходимы для синхронизации данных. Сущности в [!INCLUDE[prod_short](includes/cds_long_md.md)] сопоставляются с таблицами и полями таблиц в [!INCLUDE [prod_short](includes/prod_short.md)] посредством таблиц интеграции. Чтобы узнать больше о сопоставлениях, перейдите к разделу [Сопоставление стандартных сущностей для синхронизации](admin-synchronizing-business-central-and-sales.md#standard-table-mapping-for-synchronization).

## <a name="handle-differences-in-local-and-base-transaction-currencies"></a>Обработка различий в местной и базовой валютами транзакций

Вы можете подключиться к среде [!INCLUDE[prod_short](includes/cds_long_md.md)], в которой базовая валюта отличается от местной валюты в [!INCLUDE[prod_short](includes/prod_short.md)]. Вы устанавливаете подключение в [!INCLUDE[prod_short](includes/prod_short.md)] на странице **Настройка подключения Dataverse** или с помощью мастера настройки **Настройка подключения к Dataverse**.

Чтобы иметь возможность подключения, убедитесь, что в настройке базовой валюты транзакции в [!INCLUDE[prod_short](includes/cds_long_md.md)] указана валюта, установленная на странице **Валюты** в [!INCLUDE [prod_short](includes/prod_short.md)], и по крайней мере один валютный курс указан для валюты на странице **Валютные курсы**.

Приведем пример. Вы подключаете [!INCLUDE[prod_short](includes/cds_long_md.md)] с евро (EUR), установленным в качестве местной валюты на странице **Настройка ГК**, к среде [!INCLUDE[prod_short](includes/cds_long_md.md)], в которой в качестве базовой валюты транзакции задан доллар США (USD). Вам понадобятся доллары США на странице **Валюты** в [!INCLUDE [prod_short](includes/prod_short.md)] и соответствующий валютный курс. 

Когда вы включаете подключение к [!INCLUDE[prod_short](includes/cds_long_md.md)], [!INCLUDE [prod_short](includes/prod_short.md)] добавляет его локальную валюту в сущность **Валюта** в [!INCLUDE[prod_short](includes/cds_long_md.md)] с валютным курсом из поля **Коэффициент курса валюты** на странице **Валютные курсы**.

Синхронизация валют однонаправленная, из [!INCLUDE [prod_short](includes/prod_short.md)] в [!INCLUDE [!INCLUDE[prod_short](includes/cds_long_md.md)], денежные суммы конвертируются и синхронизируются следующим образом:

* Суммы в базовой валюте [!INCLUDE[prod_short](includes/cds_long_md.md)] конвертируются в местную валюту [!INCLUDE [prod_short](includes/prod_short.md)] на основе последнего обменного курса, синхронизированного с [!INCLUDE [prod_short](includes/prod_short.md)].
* Суммы в местной валюте [!INCLUDE [prod_short](includes/prod_short.md)] синхронизируются с местной валютой [!INCLUDE [prod_short](includes/prod_short.md)] в одной из других (не базовых) валют в [!INCLUDE[prod_short](includes/cds_long_md.md)].

## <a name="what-happens-when-you-copy-a-company"></a>Что происходит, когда вы копируете компанию

Вы можете безопасно копировать компании, которые интегрируются с [!INCLUDE[prod_short](includes/cds_long_md.md)] или [!INCLUDE[crm_md](includes/crm_md.md)]. Копирование компаний помогает снизить риск несогласованности данных и сэкономить ваше драгоценное время. Чтобы узнать больше о копировании компаний, перейдите в раздел [Копирование компании](about-new-company.md#copy-a-company).

[!INCLUDE [dataverse-copy-company](includes/dataverse-copy-company.md)]

## <a name="see-also"></a>См. также

[Модели владения данными](admin-cds-company-concept.md)  
<!--needs to be removed as this is moved to dev-itpro docs[Walkthrough: Customizing an Integration with Dataverse](\dynamics365\business-central\dev-itpro\administration\administration-custom-cds-integration) -->


[!INCLUDE[footer-include](includes/footer-banner.md)]
