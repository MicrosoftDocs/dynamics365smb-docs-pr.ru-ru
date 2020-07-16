---
title: Подключение к Common Data Service | Документы Майкрософт
description: Вы можете интегрировать другие приложения с Business Central через Common Data Service.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/30/2020
ms.author: bholtorf
ms.openlocfilehash: 4c57d8c79f91319675527f514b01b6ddeb83e722
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3529217"
---
# <a name="connect-to-common-data-service"></a>Подключение к Common Data Service
В этом разделе описывается, как установить соединение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)]. Как правило, предприятия создают соединение для интеграции и синхронизации данных с другим бизнес-приложением Dynamics 365, например [!INCLUDE[crm_md](includes/crm_md.md)].  

## <a name="before-you-start"></a>Перед началом работы
Перед тем, как создать соединение, необходимо подготовить несколько фрагментов информации:  

* URL-адрес для среды [!INCLUDE[d365fin](includes/cds_long_md.md)], к которой требуется подключиться. Если вы используете мастер настройки **Настройка подключения CDS**, чтобы создать соединение, мы обнаружим ваши среды, но вы также можете ввести URL-адрес другой среды в своем клиенте.  
* Имя пользователя и пароль учетной записи, которая имеет разрешения администратора в [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[d365fin](includes/cds_long_md.md)].  

> [!Note]
> Эти шаги описывают процедуру для интернет-версии [!INCLUDE[d365fin](includes/d365fin_md.md)].
> Если вы используете локальную версию Business Central и не используете учетную запись Azure Active Directory для подключения Common Data Service, Вы также должны указать имя пользователя и пароль учетной записи пользователя для интеграции. Эта учетная запись называется учетной записью "пользователя интеграции". Если вы используете учетная запись Azure Active Directory интеграция учетной записи пользователя не требуется или не отображается. Пользователь интеграции будет настроен автоматически и не потребует лицензии.

## <a name="set-up-a-connection-to-d365fin"></a>Настройка подключения к [!INCLUDE[d365fin](includes/cds_long_md.md)]  
Для всех типов проверки подлинности, отличных от проверки подлинности Office 365, вы настраиваете подключение к [!INCLUDE[d365fin](includes/cds_long_md.md)] на странице **Настройка подключения к CDS**. Для аутентификации Office 365 рекомендуется использовать мастер настройки **Настройка подключения Common Data Service**. Этот мастер позволяет проще настроить подключение и указать расширенные функции, такие как модель ответственности и начальной синхронизации.  

> [!Important]
> Во время настройки подключения к [!INCLUDE[d365fin](includes/cds_long_md.md)] администратору будет предложено предоставить следующие разрешения зарегистрированному приложению Azure с именем Интеграция [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[d365fin](includes/cds_long_md.md)]:
> * Требуется разрешение **доступ [!INCLUDE[d365fin](includes/cds_long_md.md)] как вы**, поэтому [!INCLUDE[d365fin](includes/d365fin_md.md)] может от имени администратора автоматически создавать нелицензионные неинтерактивные пользователи приложения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)], назначьте роли безопасности этому пользователю и разверните [!INCLUDE[d365fin](includes/d365fin_md.md)] Базовое решение для интеграции CDS для [!INCLUDE[d365fin](includes/cds_long_md.md)]. Это разрешение используется только один раз при настройке подключения к [!INCLUDE[d365fin](includes/cds_long_md.md)]. 
> * Требуется разрешение **Полный доступ к Dynamics 365[!INCLUDE[d365fin](includes/d365fin_md.md)]**, поэтому автоматически создаваемый пользователь приложения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)] может получить доступ к данные [!INCLUDE[d365fin](includes/d365fin_md.md)], которые будут синхронизированы. 
> * Требуется разрешение **войдите и прочтите свой профиль**, чтобы убедиться, что пользователь, входящий в систему, на самом деле имеет роль администратора системы, назначенную в [!INCLUDE[d365fin](includes/cds_long_md.md)]. 
>
> Предоставляя согласие от имени организации, администратор дает право зарегистрированному приложению Azure, которое называется Интеграция [!INCLUDE[d365fin](includes/d365fin_md.md)] в [!INCLUDE[d365fin](includes/cds_long_md.md)] синхронизировать данные, используя автоматически созданные учетные данные пользователя приложения интеграции [!INCLUDE[d365fin](includes/d365fin_md.md)].

### <a name="to-use-the-set-up-common-data-service-connection-assisted-setup-guide"></a>Использование мастера настройки для настройки подключения Common Data Service 
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Мастер настройки**, затем выберите соответствующую ссылку.
2. Выберите пункт **Настройка подключения к Common Data Service**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.

### <a name="to-create-or-maintain-the-connection-manually"></a>Создание или ведение подключения вручную
Далее описан порядок настройки подключения вручную на странице **Настройка подключения к CDS**. Это также страница, на которой можно управлять настройками для интеграции.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к CDS**, затем выберите соответствующую ссылку.
2. Введите следующие сведения для подключения из [!INCLUDE[d365fin](includes/cds_long_md.md)] к [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Поле|Описание|
|-----|-----|
|**URL-адрес среды**|Если вы владеете средами в [!INCLUDE[d365fin](includes/cds_long_md.md)], мы найдем их для вас, когда вы запустите мастер настройки. Если вы хотите подключиться к другой среде в другом арендаторе, вы можете ввести учетные данные администратора для этой среды, и мы обнаружим их. |
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
    >  Если шифрование данных не включено в [!INCLUDE[d365fin](includes/d365fin_md.md)], вы получите запрос, требуется ли его включить. Чтобы включить шифрование данных, выберите **Да** и предоставьте требуемую информацию. В противном случае выберите **Нет**. Шифрование данных можно включить позднее. Дополнительные сведения см. в разделе [Шифрование данных в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-encrypting-data) в справке для разработчика и администратора.  

5. Если синхронизация [!INCLUDE[d365fin](includes/cds_long_md.md)] еще не настроена, вы получите запрос, следует ли использовать настройки синхронизации по умолчанию. В зависимости от того, требуется ли соответствие записей в [!INCLUDE[d365fin](includes/cds_long_md.md)] и [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите **Да** или **Нет**.

## <a name="connecting-on-premises-versions"></a>Подключение локальных версий
Чтобы подключить локальную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] [!INCLUDE[d365fin](includes/cds_long_md.md)], необходимо указать некоторую информацию на странице **Настройка подключения Common Data Service**.

Если вы хотите подключиться с помощью учетной записи Azure Active Directory ( Azure AD), вы должны зарегистрировать заявку в Azure AD и укажите идентификатор приложения, секретный ключ хранилища и используемый URL-адрес перенаправления. URL-адрес перенаправления предварительно заполнен и должен работать для большинства установок. Вы должны настроить вашу установку на использование HTTPS. Для получения дополнительной информации см. [Настройка SSL для защиты подключения веб-клиента Business Central](/dynamics365/business-central/dev-itpro/deployment/configure-ssl-web-client-connection). Если вы настраиваете на своем сервере другую начальную страницу, вы всегда можете изменить URL-адрес. Секрет клиента будет сохранен как зашифрованная строка в вашей базе данных. 

### <a name="to-register-an-application-in-azure-ad-for-connecting-from-business-central-to-common-data-service"></a>Чтобы зарегистрировать заявку в Azure AD для подключения из Business Central к Common Data Service
Следующие шаги предполагают, что вы используете Azure AD, чтобы управлять удостоверениями и доступом. Дополнительные сведения о регистрации приложения в Azure AD, см. в [Быстрый старт: зарегистрируйте приложение на платформе идентификации Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app). Если вы не используете Azure AD, см. [Использование другой службы управления удостоверениями и доступом](admin-how-to-set-up-a-dynamics-crm-connection.md#using-another-identity-and-access-management-service). 

1. В Azure Portal, в **управлять** на панели навигации выберите **Аутентификация**. 
2. В **URL-адреса перенаправления** добавьте URL-адрес перенаправления, который предлагается на страница **Настройка подключения Common Data Service** в [!INCLUDE[d365fin](includes/d365fin_md.md)].
3. В **управлять** выберите **Разрешения API**.
4. В **Настроенные разрешения** выберите **Добавить разрешение** и затем добавьте делегированные разрешения на вкладке **API-интерфейсы Microsoft** следующим образом:
    * Для Business Central добавьте разрешения **Financials.ReadWrite.All**.
    * Для Dynamics CRM, добавить разрешения **user_impersonation**. 

> [!NOTE]
> Имя API Dynamics CRM может измениться.

5.  В **управлять** выберите **Сертификаты и секреты**, а затем создайте новый секрет для вашего приложения. Вы будете использовать секрет либо в [!INCLUDE[d365fin](includes/d365fin_md.md)], в поле **Секрет клиента** на **Настройка подключения Common Data Service** или сохраните в защищенном хранилище и предоставьте его подписчику события, как описано ранее в этом разделе.
6. Выберите **обзор**, а затем найдите значение **Код приложения (клиента)**. Это код клиента вашего приложения. Вы должны ввести его либо на страница **Настройка подключения Common Data Service** в **Код клиента**или сохраните его в безопасном хранилище и предоставьте его подписчику события.
7. В [!INCLUDE[d365fin](includes/d365fin_md.md)], на страница **Настройка подключения Common Data Service**, в поле **URL-адрес среды** введите URL-адрес для вашей среды [!INCLUDE[d365fin](includes/cds_long_md.md)].
8. Чтобы включить подключение к [!INCLUDE[d365fin](includes/cds_long_md.md)] включите переключатель **Включено**.
9. Войдите в систему с учетной записью администратора для Azure Active Directory (эта учетная запись должна иметь действующую лицензию для [!INCLUDE[d365fin](includes/cds_long_md.md)] и быть администратором в вашей среде [!INCLUDE[d365fin](includes/cds_long_md.md)]). После входа в систему вам будет предложено разрешить зарегистрированному приложению войти в [!INCLUDE[d365fin](includes/cds_long_md.md)] от имени организации. Вы должны дать согласие на завершение установки.

   > [!NOTE]
   > Если вам не предлагается войти в систему с учетной записью администратора, возможно, это связано с блокировкой всплывающих окон. Чтобы войти, разрешите всплывающие окна от https://login.microsoftonline.com.

#### <a name="using-another-identity-and-access-management-service"></a>Использование другой службы управления удостоверениями и доступом
Если вы не используете Azure Active Directory для управления удостоверениями и доступом, вам потребуется помощь разработчика. Если вы предпочитаете хранить код приложения и секрет в другом месте, вы можете оставить поля «Код клиента» и «Секрет клиента» пустыми и написать расширение для получения кода и секрета из местоположения. Вы можете предоставить секрет во время выполнения, подписавшись на события OnGetCDSConnectionClientId и OnGetCDSConnectionClientSecret в codeunit 7201 «CDS Integration Impl».

### <a name="to-disconnect-from-d365fin"></a>Отключение от [!INCLUDE[d365fin](includes/cds_long_md.md)]  
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к CDS**, затем выберите соответствующую ссылку.
2. На странице **Настройка подключения к CDS** выключите переключатель **Включено**.  

## <a name="see-also"></a>См. также  
[Просмотр статуса синхронизации](admin-how-to-view-synchronization-status.md)  
