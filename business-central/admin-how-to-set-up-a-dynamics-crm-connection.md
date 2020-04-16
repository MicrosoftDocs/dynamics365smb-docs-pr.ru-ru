---
title: Подключение к Microsoft Dynamics 365 Sales | Документация Майкрософт
description: Вы можете интегрировать другие приложения с Business Central через Common Data Service.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: bholtorf
ms.openlocfilehash: 3375db0208d1a0275011f0efbfce4a13102c522e
ms.sourcegitcommit: d67328e1992c9a754b14c7267ab11312c80c38dd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3196643"
---
# <a name="connect-to-common-data-service"></a>Подключение к Common Data Service
В этом разделе описывается, как установить соединение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)]. Как правило, предприятия создают соединение для интеграции и синхронизации данных с другим бизнес-приложением Dynamics 365, например [!INCLUDE[crm_md](includes/crm_md.md)].  

## <a name="before-you-start"></a>Перед началом работы
Перед тем, как создать соединение, необходимо подготовить несколько фрагментов информации:  

* URL-адрес для среды [!INCLUDE[d365fin](includes/cds_long_md.md)], к которой требуется подключиться. Если вы используете мастер настройки **Настройка подключения CDS**, чтобы создать соединение, мы обнаружим ваши среды, но вы также можете ввести URL-адрес другой среды в своем клиенте.  
* Имя пользователя и пароль учетной записи пользователя, которая используется для интеграции. Эта учетная запись называется учетной записью "пользователя интеграции". 
* Имя пользователя и пароль учетной записи, которая имеет разрешения администратора в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)].  

> [!Note]
> Эти шаги описывают процедуру для интернет-версии [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="set-up-a-connection-to-d365fin"></a>Настройка подключения к [!INCLUDE[d365fin](includes/cds_long_md.md)]  
Для всех типов проверки подлинности, отличных от проверки подлинности Office 365, вы настраиваете подключение к [!INCLUDE[d365fin](includes/cds_long_md.md)] на странице **Настройка подключения к CDS**. Для аутентификации Office 365 рекомендуется использовать мастер настройки **Настройка подключения к CDS**. Этот мастер позволяет проще настроить подключение и указать расширенные функции, такие как связи между записями.  

### <a name="to-use-the-cds-connection-setup-assisted-setup-guide"></a>Использование мастера настройки подключения к CDS 
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Мастер настройки**, затем выберите соответствующую ссылку.
2. Выберите **Настроить подключение для базовой интеграции CDS**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.

> [!Note]
> Мастер **Настройка подключения к CDS** автоматически назначает роли безопасности **Администратор интеграции** и **Пользователь интеграции** для учетной записи пользователя, используемой для интеграции, и устанавливает для этой учетной записи режим доступа **неинтерактивный**.

### <a name="to-create-or-maintain-the-connection-manually"></a>Создание или ведение подключения вручную
Далее описан порядок настройки подключения вручную на странице **Настройка подключения к CDS**. Это также страница, на которой можно управлять настройками для интеграции.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к CDS**, затем выберите соответствующую ссылку.
2. Введите следующие сведения для подключения из [!INCLUDE[d365fin](includes/cds_long_md.md)] к [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Поле|Описание|
|-----|-----|
|**URL-адрес среды**|Если вы владеете средами в [!INCLUDE[d365fin](includes/cds_long_md.md)], мы найдем их для вас, когда вы запустите мастер настройки. Если вы хотите подключиться к другой среде в другом арендаторе, вы можете ввести учетные данные администратора для этой среды, и мы обнаружим их. |
|**Имя пользователя** и **Пароль**|Эти учетные данные учетной записи пользователя предназначены для интеграции. Дополнительные сведения см. в разделе [Настройка учетных записей пользователей для интеграции с [!INCLUDE[d365fin](includes/cds_long_md.md)]](admin-setting-up-integration-with-dynamics-sales.md).|
|**Включено**|Начните использовать интеграцию. Если выполнять подключение в данный момент не требуется, можно сохранить настройки подключения, однако пользователи не получат доступа к данным [!INCLUDE[d365fin](includes/cds_long_md.md)] из [!INCLUDE[d365fin](includes/d365fin_md.md)]. Позднее следует вернуться на эту страницу и выполнить подключение.  |

3. В поле **Модель ответственности** выберите, хотите ли вы, чтобы сущность рабочей группы в [!INCLUDE[d365fin](includes/cds_long_md.md)] владела новыми записями, или чтобы ответственными были один или несколько конкретных пользователей. Если вы выбираете **Человек**, вы должны указать каждого пользователя. Если вы выбираете вариант **Рабочая группа**, бизнес-подразделение BCI_Company по умолчанию будет отображаться в поле **Связанный филиал**.

<!--Need to verify the details in this table, are these specific to Sales maybe?
Enter the following advanced settings.

|Field|Description|
|-----|-----|
|**[!INCLUDE[d365fin](includes/d365fin_md.md)] Users Must Map to CDS Users**|If you are using the Person ownership model, specify whether [!INCLUDE[d365fin](includes/d365fin_md.md)] user accounts must have a matching user accounts in [!INCLUDE[d365fin](includes/cds_long_md.md)]. The **Office 365 Authentication Email** of the [!INCLUDE[d365fin](includes/d365fin_md.md)] user must be the same as the **Primary Email** of the [!INCLUDE[crm_md](includes/crm_md.md)] user.<br /><br /> If you set the value to **Yes**, [!INCLUDE[d365fin](includes/d365fin_md.md)] users who do not have a matching [!INCLUDE[crm_md](includes/crm_md.md)] user account will not have [!INCLUDE[d365fin](includes/d365fin_md.md)] integration capabilities in the user interface. Access to [!INCLUDE[crm_md](includes/crm_md.md)] data directly from [!INCLUDE[d365fin](includes/d365fin_md.md)] is done on behalf of the [!INCLUDE[crm_md](includes/crm_md.md)] user account.<br /><br /> If you set the value to **No**, all [!INCLUDE[d365fin](includes/d365fin_md.md)] users will have [!INCLUDE[crm_md](includes/crm_md.md)] integration capabilities in the user interface. Access to [!INCLUDE[crm_md](includes/crm_md.md)] data is done on behalf of the [!INCLUDE[crm_md](includes/crm_md.md)] connection (integration) user.|
|**Current Business Central Salesperson is Mapped to a User**|Indicates whether your user account is mapped to an account in [!INCLUDE[crm_md](includes/crm_md.md)] <!--double check the name of this field|-->

4. Для тестирования настроек подключения выберите **Подключение**, затем **Проверить подключение**.  

    > [!NOTE]  
    >  Если шифрование данных не включено в [!INCLUDE[d365fin](includes/d365fin_md.md)], вы получите запрос, требуется ли его включить. Чтобы включить шифрование данных, выберите **Да** и предоставьте требуемую информацию. В противном случае выберите **Нет**. Шифрование данных можно включить позднее. Дополнительные сведения см. в разделе [Шифрование данных в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-encrypting-data.md) в справке для разработчиков и ИТ-специалистов.  

5. Если синхронизация [!INCLUDE[d365fin](includes/cds_long_md.md)] еще не настроена, вы получите запрос, следует ли использовать настройки синхронизации по умолчанию. В зависимости от того, требуется ли соответствие записей в [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите **Да** или **Нет**.

> [!Note]
> При подключении к [!INCLUDE[d365fin](includes/cds_long_md.md)] с помощью страницы **Настройка подключения к CDS** может потребоваться назначить роли безопасности "Администратор интеграции" и "Пользователь интеграции" учетной записи пользователя, используемой для интеграции в Dynamics 365 Sales. Для получения дополнительной информации см. [Назначение роли безопасности пользователю](/dynamics365/customer-engagement/admin/create-users-assign-online-security-roles#assign-a-security-role-to-a-user.md).

### <a name="to-disconnect-from-d365fin"></a>Отключение от [!INCLUDE[d365fin](includes/cds_long_md.md)]  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к CDS**, затем выберите соответствующую ссылку.
2. На странице **Настройка подключения к CDS** выключите переключатель **Включено**.  

## <a name="see-also"></a>См. также  
[Просмотр статуса синхронизации](admin-how-to-view-synchronization-status.md)  
