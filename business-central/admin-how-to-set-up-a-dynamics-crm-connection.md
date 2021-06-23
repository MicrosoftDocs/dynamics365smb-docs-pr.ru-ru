---
title: Подключение к Microsoft Dataverse
description: Вы можете интегрировать другие приложения с Business Central через Microsoft Dataverse. В этой статье представлены советы и рекомендации по настройке подключений.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/26/2021
ms.author: bholtorf
ms.openlocfilehash: ebe708efacbaa03d5f10deb7b21b090222f28818
ms.sourcegitcommit: 61e279b253370cdf87b7bc1ee0f927e4f0521344
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "6063481"
---
# <a name="connect-to-microsoft-dataverse"></a>Подключение к Microsoft Dataverse

[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

В этом разделе описывается, как установить соединение между [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Как правило, предприятия создают соединение для интеграции и синхронизации данных с другим бизнес-приложением Dynamics 365, например [!INCLUDE[crm_md](includes/crm_md.md)].  

## <a name="before-you-start"></a>Перед началом работы

Перед тем, как создать соединение, необходимо подготовить несколько фрагментов информации:  

* URL-адрес для среды [!INCLUDE[cds_long_md](includes/cds_long_md.md)], к которой требуется подключиться. Если вы используете мастер настройки **Настройка подключения Dataverse**, чтобы создать соединение, мы обнаружим ваши среды, но вы также можете ввести URL-адрес другой среды в своем клиенте.  
* Имя пользователя и пароль учетной записи, которая имеет разрешения администратора в [!INCLUDE[prod_short](includes/prod_short.md)] и [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  
* Если у вас есть локальная версия [!INCLUDE[prod_short](includes/prod_short.md)] выпуска 2020, волна 1, версия 16.5, ознакомьтесь со статьей [Некоторые известные проблемы](/dynamics365/business-central/dev-itpro/upgrade/known-issues#wrong-net-assemblies-for-external-connected-services). Вам нужно будет выполнить описанный обходной метод, прежде чем вы сможете создать подключение к [!INCLUDE[cds_long_md](includes/cds_long_md.md)].
* Местная валюта компании в [!INCLUDE[prod_short](includes/prod_short.md)] должна быть такой же, как и базовая валюта транзакции в [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. После того, как базовая транзакция установлена в [!INCLUDE[cds_long_md](includes/cds_long_md.md)], это не может быть изменено. Для получения дополнительной информации см. [Сущность валюты транзакции (валюта)](/powerapps/developer/data-platform/transaction-currency-currency-entity). Это означает, что у всех компаний [!INCLUDE[prod_short](includes/prod_short.md)], которые вы подключаете к организации [!INCLUDE[cds_long_md](includes/cds_long_md.md)], должна использоваться та же валюта.

> [!IMPORTANT]
> Ваша среда [!INCLUDE[cds_long_md](includes/cds_long_md.md)] не должна находиться в режиме администрирования. Режим администрирования приведет к сбою подключения, поскольку у учетной записи пользователя интеграции для подключения нет прав администратора. Дополнительные сведения см. в разделе [Режим администрирования](/power-platform/admin/admin-mode).

> [!Note]
> Эти шаги описывают процедуру для [!INCLUDE[prod_short](includes/prod_short.md)] Online.
> Если вы используете локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] и не используете учетную запись Azure Active Directory для подключения [!INCLUDE [cds_long_md](includes/cds_long_md.md)], вы также должны указать имя пользователя и пароль учетной записи пользователя для интеграции. Эта учетная запись называется учетной записью "пользователя интеграции". Если вы используете учетная запись Azure Active Directory интеграция учетной записи пользователя не требуется или не отображается. Пользователь интеграции будет настроен автоматически и не потребует лицензии.

## <a name="set-up-a-connection-to-cds_long_md"></a>Настройка подключения к [!INCLUDE[cds_long_md](includes/cds_long_md.md)]

Для всех типов проверки подлинности, отличных от проверки подлинности Microsoft 365, вы настраиваете подключение к [!INCLUDE[cds_long_md](includes/cds_long_md.md)] на странице **Настройка подключения Dataverse**. Для аутентификации Microsoft 365 рекомендуется использовать мастер настройки **Настройка подключения Dataverse**. Этот мастер позволяет проще настроить подключение и указать расширенные функции, такие как модель ответственности и начальной синхронизации.  

> [!IMPORTANT]
> Во время настройки подключения к [!INCLUDE[cds_long_md](includes/cds_long_md.md)] администратору будет предложено предоставить следующие разрешения зарегистрированному приложению Azure с именем "Интеграция [!INCLUDE[prod_short](includes/prod_short.md)]" в [!INCLUDE[cds_long_md](includes/cds_long_md.md)]:
>
> * Требуется разрешение **доступ [!INCLUDE[cds_long_md](includes/cds_long_md.md)] как вы**, поэтому [!INCLUDE[prod_short](includes/prod_short.md)] может от имени администратора автоматически создавать нелицензионные неинтерактивные пользователи приложения интеграции [!INCLUDE[prod_short](includes/prod_short.md)], назначьте роли безопасности этому пользователю и разверните решение для интеграции [!INCLUDE[prod_short](includes/prod_short.md)] для [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Это разрешение используется только один раз при настройке подключения к [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  
> * Требуется разрешение **Полный доступ к Dynamics 365[!INCLUDE[prod_short](includes/prod_short.md)]**, поэтому автоматически создаваемый пользователь приложения интеграции [!INCLUDE[prod_short](includes/prod_short.md)] может получить доступ к данные [!INCLUDE[prod_short](includes/prod_short.md)], которые будут синхронизированы.  
> * Требуется разрешение **войдите и прочтите свой профиль**, чтобы убедиться, что пользователь, входящий в систему, на самом деле имеет роль администратора системы, назначенную в [!INCLUDE[cds_long_md](includes/cds_long_md.md)].  
>
> Предоставляя согласие от имени организации, администратор дает право зарегистрированному приложению Azure, которое называется Интеграция [!INCLUDE[prod_short](includes/prod_short.md)] в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] синхронизировать данные, используя автоматически созданные учетные данные пользователя приложения интеграции [!INCLUDE[prod_short](includes/prod_short.md)].

### <a name="to-use-the-dataverse-connection-setup-assisted-setup-guide"></a>Использование мастера настройки подключения Dataverse
Руководство по настройке подключения Dataverse может упростить подключение приложений и даже помочь вам выполнить первоначальную синхронизацию. Если вы выберете запуск начальной синхронизации, [!INCLUDE[prod_short](includes/prod_short.md)] проверит данные в обоих приложениях и предоставит рекомендации по подходу к начальной синхронизации. В следующей таблице описаны эти рекомендации.

|Рекомендация  |Описание  |
|---------|---------|
|**Полная синхронизация**|Данные существуют только в [!INCLUDE[prod_short](includes/prod_short.md)] или только в [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. Рекомендация: синхронизировать все данные из службы, в которой они есть, с другой службой.|
|**Без синхронизации**|Данные существуют в обоих приложениях, и выполнение полной синхронизации приведет к их дублированию. Рекомендуется связать записи.|
|**Зависимость не удовлетворена**|Данные существуют в обоих приложениях, но строка или таблица не могут быть синхронизированы, потому что она зависит от строки или таблицы, для которых есть рекомендация "Без синхронизации". Например, если клиенты не могут быть синхронизированы, то данные для контактов, которые зависят от данных клиентов, также не могут быть синхронизированы.|

> [!IMPORTANT]
> Обычно вы используете полную синхронизацию только тогда, когда интегрируете приложения впервые, и только одно приложение содержит данные. Полная синхронизация может быть полезна в демонстрационной среде, поскольку она автоматически создает и связывает записи в каждом приложении, что ускоряет начало работы с синхронизированными данными. Однако вам следует запускать полную синхронизацию только в том случае, если вам нужна одна строка в [!INCLUDE[prod_short](includes/prod_short.md)] для каждой строки в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] для сопоставления таблиц. В противном случае результатом могут быть повторяющиеся записи.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Мастер настройки**, затем выберите соответствующую ссылку.
2. Выберите пункт **Настройка подключения к Microsoft Dataverse**, чтобы запустить мастер настройки.
3. Заполните соответствующим образом поля.

> [!NOTE]
> Если вам не предлагается войти в систему с учетной записью администратора, возможно, это связано с блокировкой всплывающих окон. Чтобы войти, разрешите всплывающие окна от `https://login.microsoftonline.com`.

### <a name="to-create-or-maintain-the-connection-manually"></a>Создание или ведение подключения вручную

Далее описан порядок настройки подключения вручную на странице **Настройка подключения Dataverse**. Это также страница, на которой можно управлять настройками для интеграции.

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к Dataverse**, затем выберите соответствующую ссылку.
2. Введите следующие сведения для подключения из [!INCLUDE[cds_long_md](includes/cds_long_md.md)] к [!INCLUDE[prod_short](includes/prod_short.md)].

    |Поле|Описание|
    |-----|-----|
    |**URL-адрес среды**|Если вы владеете средами в [!INCLUDE[cds_long_md](includes/cds_long_md.md)], мы найдем их для вас, когда вы запустите мастер настройки. Если вы хотите подключиться к другой среде в другом арендаторе, вы можете ввести учетные данные администратора для этой среды, и мы обнаружим их. |
    |**Включено**|Начните использовать интеграцию. Если выполнять подключение в данный момент не требуется, можно сохранить настройки подключения, однако пользователи не получат доступа к данным [!INCLUDE[cds_long_md](includes/cds_long_md.md)] из [!INCLUDE[prod_short](includes/prod_short.md)]. Позднее следует вернуться на эту страницу и выполнить подключение.  |

3. В поле **Модель ответственности** выберите, хотите ли вы, чтобы таблица рабочей группы в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] владела новыми записями, или чтобы ответственными были один или несколько конкретных пользователей. Если вы выбираете **Человек**, вы должны указать каждого пользователя. Если вы выбираете вариант **Рабочая группа**, бизнес-подразделение по умолчанию будет отображаться в поле **Связанный филиал**.

    <!--Need to verify the details in this table, are these specific to Sales maybe?  IK: No they are not and no longer relevant 
    Enter the following advanced settings.-->

    <!-- |Field|Description|
    |-----|-----|
    |**[!INCLUDE[prod_short](includes/prod_short.md)] Users Must Map to CDS Users**|If you are using the Person ownership model, specify whether [!INCLUDE[prod_short](includes/prod_short.md)] user accounts must have a matching user accounts in [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. The **Microsoft 365 Authentication Email** of the [!INCLUDE[prod_short](includes/prod_short.md)] user must be the same as the **Primary Email** of the [!INCLUDE[crm_md](includes/crm_md.md)] user.<br /><br /> If you set the value to **Yes**, [!INCLUDE[prod_short](includes/prod_short.md)] users who do not have a matching [!INCLUDE[crm_md](includes/crm_md.md)] user account will not have [!INCLUDE[prod_short](includes/prod_short.md)] integration capabilities in the user interface. Access to [!INCLUDE[crm_md](includes/crm_md.md)] data directly from [!INCLUDE[prod_short](includes/prod_short.md)] is done on behalf of the [!INCLUDE[crm_md](includes/crm_md.md)] user account.<br /><br /> If you set the value to **No**, all [!INCLUDE[prod_short](includes/prod_short.md)] users will have [!INCLUDE[crm_md](includes/crm_md.md)] integration capabilities in the user interface. Access to [!INCLUDE[crm_md](includes/crm_md.md)] data is done on behalf of the [!INCLUDE[crm_md](includes/crm_md.md)] connection (integration) user.|
    |**Current Business Central Salesperson is Mapped to a User**|Indicates whether your user account is mapped to an account in [!INCLUDE[crm_md](includes/crm_md.md)] double check the name of this field-->|
4. Для тестирования настроек подключения выберите **Подключение**, затем **Проверить подключение**.  

    > [!NOTE]  
    > Если шифрование данных не включено в [!INCLUDE[prod_short](includes/prod_short.md)], вы получите запрос, требуется ли его включить. Чтобы включить шифрование данных, выберите **Да** и предоставьте требуемую информацию. В противном случае выберите **Нет**. Шифрование данных можно включить позднее. Дополнительные сведения см. в разделе [Шифрование данных в Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-encrypting-data) в справке для разработчика и администратора.  
5. Если синхронизация [!INCLUDE[cds_long_md](includes/cds_long_md.md)] еще не настроена, вы получите запрос, следует ли использовать настройки синхронизации по умолчанию. В зависимости от того, требуется ли соответствие записей в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] и [!INCLUDE[prod_short](includes/prod_short.md)], выберите **Да** или **Нет**.

<!--
## Show Me the Process

The following video shows the steps to connect [!INCLUDE[prod_short](includes/prod_short.md)] and [!INCLUDE[cds_long_md](includes/cds_long_md.md)]. <br>
  
> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RE4ArlP]

-->

## <a name="connecting-on-premises-versions"></a>Подключение локальных версий

Чтобы подключить локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] [!INCLUDE[cds_long_md](includes/cds_long_md.md)], необходимо указать некоторую информацию на странице **Настройка подключения Dataverse**.

Если вы хотите подключиться с помощью учетной записи Azure Active Directory ( Azure AD), вы должны зарегистрировать заявку в Azure AD и укажите идентификатор приложения, секретный ключ хранилища и используемый URL-адрес перенаправления. URL-адрес перенаправления предварительно заполнен и должен работать для большинства установок. Вы должны настроить вашу установку на использование HTTPS. Для получения дополнительной информации см. [Настройка SSL для защиты подключения веб-клиента Business Central](/dynamics365/business-central/dev-itpro/deployment/configure-ssl-web-client-connection). Если вы настраиваете на своем сервере другую начальную страницу, вы всегда можете изменить URL-адрес. Секрет клиента будет сохранен как зашифрованная строка в вашей базе данных. 

### <a name="prerequisites"></a>Предварительные требования

Dataverse должна использовать один из следующих типов аутентификации:

* Office365 (устаревшая версия)

  > [!IMPORTANT]
  > С апреля 2022 года поддержка Office365 (устаревшая версия) будет прекращена. Дополнительные сведения см. в разделе [Запланированные важные изменения (устаревания) в Power Apps, Power Automate и приложениях для взаимодействия с клиентами](/power-platform/important-changes-coming#deprecation-of-office365-authentication-type-and-organizationserviceproxy-class-for-connecting-to-dataverse).
* Office365 (современный, на основе секрета клиента OAuth2)
* OAuth

### <a name="to-register-an-application-in-azure-ad-for-connecting-from-business-central-to-dataverse"></a>Чтобы зарегистрировать заявку в Azure AD для подключения из Business Central к Dataverse

Следующие шаги предполагают, что вы используете Azure AD, чтобы управлять удостоверениями и доступом. Дополнительные сведения о регистрации приложения в Azure AD, см. в [Быстрый старт: зарегистрируйте приложение на платформе идентификации Microsoft](/azure/active-directory/develop/quickstart-register-app). 

1. В Azure Portal, в **управлять** на панели навигации выберите **Аутентификация**.  
2. В **URL-адреса перенаправления** добавьте URL-адрес перенаправления, который предлагается на страница **Настройка подключения Dataverse** в [!INCLUDE[prod_short](includes/prod_short.md)].
3. В **управлять** выберите **Разрешения API**.
4. В **Настроенные разрешения** выберите **Добавить разрешение** и затем добавьте делегированные разрешения на вкладке **API-интерфейсы Microsoft** следующим образом:
    * Для Business Central добавьте разрешения **Financials.ReadWrite.All**.
    * Для Dynamics CRM, добавить разрешения **user_impersonation**.  

    > [!NOTE]
    > Имя API Dynamics CRM может измениться.

5. В **управлять** выберите **Сертификаты и секреты**, а затем создайте новый секрет для вашего приложения. Вы будете использовать секрет либо в [!INCLUDE[prod_short](includes/prod_short.md)], в поле **Секрет клиента** на **Настройка подключения Dataverse** или сохраните в защищенном хранилище и предоставьте его подписчику события, как описано ранее в этом разделе.
6. Выберите **обзор**, а затем найдите значение **Код приложения (клиента)**. Это код клиента вашего приложения. Вы должны ввести его либо на страница **Настройка подключения Dataverse** в **Код клиента** или сохраните его в безопасном хранилище и предоставьте его подписчику события.
7. В [!INCLUDE[prod_short](includes/prod_short.md)], на страница **Настройка подключения Dataverse**, в поле **URL-адрес среды** введите URL-адрес для вашей среды [!INCLUDE[cds_long_md](includes/cds_long_md.md)].
8. Чтобы включить подключение к [!INCLUDE[cds_long_md](includes/cds_long_md.md)] включите переключатель **Включено**.
9. Войдите в систему с учетной записью администратора для Azure Active Directory (эта учетная запись должна иметь действующую лицензию для [!INCLUDE[cds_long_md](includes/cds_long_md.md)] и быть администратором в вашей среде [!INCLUDE[cds_long_md](includes/cds_long_md.md)]). После входа в систему вам будет предложено разрешить зарегистрированному приложению войти в [!INCLUDE[cds_long_md](includes/cds_long_md.md)] от имени организации. Вы должны дать согласие на завершение установки.

   > [!NOTE]
   > Если вам не предлагается войти в систему с учетной записью администратора, возможно, это связано с блокировкой всплывающих окон. Чтобы войти, разрешите всплывающие окна от `https://login.microsoftonline.com`.

### <a name="to-disconnect-from-cds_long_md"></a>Отключение от [!INCLUDE[cds_long_md](includes/cds_long_md.md)]

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка подключения к Dataverse**, затем выберите соответствующую ссылку.
2. На странице **Настройка подключения Dataverse** выключите переключатель **Включено**.  

## <a name="see-also"></a>См. также

[Просмотр статуса синхронизации](admin-how-to-view-synchronization-status.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]