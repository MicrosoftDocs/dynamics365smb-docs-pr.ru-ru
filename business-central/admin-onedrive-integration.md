---
title: Управление интеграцией OneDrive с Business Central
description: Узнайте о том, что вы можете сделать для управления интеграцией между Business Central и OneDrive для бизнеса.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: OneDrive, share, browser
ms.date: 05/12/2021
ms.author: bholtorf
ms.openlocfilehash: cceb05c1ad19a95494c188cd2482b45962535c94
ms.sourcegitcommit: 99c705d160451c05b226350ff94b52fb0c3ae7a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "7606414"
---
# <a name="managing-onedrive-integration-with-business-central"></a>Управление интеграцией OneDrive с Business Central 
В этой статье представлен обзор того, что администратор может делать для управления интеграцией OneDrive для бизнеса с [!INCLUDE[prod_short](includes/prod_short.md)]. Клиенты [!INCLUDE[prod_short](includes/prod_short.md)] Online получают выгоду от автоматической интеграции, без дополнительной настройки, необходимой для использования этих функций. 

## <a name="minimum-requirements"></a>Минимальные требования

* У каждого пользователя должна быть лицензия на [!INCLUDE[prod_short](includes/prod_short.md)] и OneDrive как часть плана Microsoft 365.
* OneDrive должны быть настроены для каждого пользователя.

## <a name="governance"></a>Управление
Центр администрирования SharePoint обеспечивает широкий контроль над политиками, которые регулируют использование OneDrive во всей организации. Глобальные администраторы или пользователи, у которых есть роль администратора SharePoint, могут настраивать политики, определяющие, у кого есть доступ к OneDrive, где хранятся данные, жизненный цикл контента и многое другое. Следующие ссылки предоставляют информацию о часто используемых функциях и настройках, которые могут улучшить вашу интеграцию с [!INCLUDE[prod_short](includes/prod_short.md)]. 

* [Управление настройками общего доступа](/sharepoint/turn-external-sharing-on-or-off)
* [Используйте информационные барьеры с SharePoint](/sharepoint/information-barriers)
* [Узнайте о защите от потери данных](/microsoft-365/compliance/dlp-learn-about-dlp)
* [Установите пространство для хранения по умолчанию для пользователей OneDrive](/onedrive/set-default-storage-space)
* [Добавление и удаление администраторов для OneDrive пользователя](/sharepoint/manage-user-profiles#add-and-remove-admins-for-a-users-onedrive)
* [Запрет создания OneDrive для некоторых пользователей](/sharepoint/manage-user-profiles#disable-onedrive-creation-for-some-users)
* [Возможности Multi-Geo в OneDrive и SharePoint Online](/microsoft-365/enterprise/multi-geo-capabilities-in-onedrive-and-sharepoint-online-in-microsoft-365)

> [!NOTE]
> Некоторые функции могут быть доступны только для определенных планов.

## <a name="managing-privacy"></a>Управление конфиденциальностью
Администраторы и конечные пользователи контролируют контент, хранящийся в OneDrive, и эти данные принадлежат исключительно вашей организации. Для получения дополнительной информации см. [Как SharePoint и OneDrive защищают ваши данные в облаке](/sharepoint/safeguarding-your-data). Вы также можете прочесть наше [Заявление о конфиденциальности Microsoft](https://privacy.microsoft.com/en-us/privacystatement), в котором объясняется, какие данные обрабатывает Microsoft, как Microsoft обрабатывает их и для каких целей.

## <a name="restoring-onedrive-and-prod_short"></a>Восстановление OneDrive и [!INCLUDE[prod_short](includes/prod_short.md)]
В рамках процедуры аварийного восстановления администраторам может потребоваться восстановить среду [!INCLUDE[prod_short](includes/prod_short.md)] в резервную копию из момента в прошлом и синхронизировать хранилище OneDrive на этот момент времени. OneDrive предоставляет для этого различные инструменты, такие как восстановление OneDrive пользователя к предыдущему моменту, восстановление предыдущей версии отдельного файла или восстановление удаленных файлов. Для получения дополнительных сведений см. следующие статьи:

* Для [!INCLUDE[prod_short](includes/prod_short.md)] см. [Восстановление среды в центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-backup-restore).
* Для OneDrive см. [Восстановление OneDrive](https://support.microsoft.com/en-us/office/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15?ui=en-us&rs=en-us&ad=us)

## <a name="configuring-business-central-on-premises"></a>Настройка локальной версии Business Central

Администратор должен установить соединение между локальной версией [!INCLUDE[prod_short](includes/prod_short.md)] и OneDrive. В отличие от [!INCLUDE[prod_short](includes/prod_short.md)] Online соединение не автоматическое. Если соединение не настроено, пользователи не могут использовать функции для OneDrive. 

Локальная версия [!INCLUDE[prod_short](includes/prod_short.md)] может быть подключена только к OneDrive, размещенному Microsoft в облаке. Подключение локальной версии [!INCLUDE[prod_short](includes/prod_short.md)] к репозиторию Мои сайты сервера SharePoint не поддерживается.

> [!IMPORTANT]
> Настраивая эту функцию, вы также включаете устаревшие функции, которые отправляют файлы в OneDrive.  
>
>* Функция «Открыть в Excel» автоматически скопирует файл Excel в OneDrive, затем откроет его в Excel Online. 
>* При экспорте любого отчета в файл он автоматически копирует файл в OneDrive, затем открывает его в Excel Online, Word Online или OneDrive. 
>* Другие функции также могут автоматически открываться в OneDrive.

### <a name="to-prepare-prod_short-on-premises-for-connecting-to-onedrive"></a>Подготовка локальной версии [!INCLUDE[prod_short](includes/prod_short.md)] для подключения к OneDrive

<!-- 
1. For the best experience Configure Azure Active Directory (AD) authentication.

   For more information, see [Authenticating Business Central Users with Azure Active Directory](/dynamics365/business-central/dev-itpro/administration/authenticating-users-with-azure-active-directory)-->

Добавьте зарегистрированное приложение для Business Central в свой арендатор Azure AD вашего плана Microsoft 365. Как и другие службы Azure, которые работают с Business Central, OneDrive требует регистрации приложения в Azure Active Directory (Azure AD). Регистрация приложения предоставляет услуги аутентификации и авторизации между Business Central и SharePoint, что используется OneDrive.

Настройте зарегистрированное приложение со следующими делегированными разрешениями для API SharePoint:

- AllSites.Write
- MyFiles.Write
- User.Read.All 

Вы выполняете эту работу на портале Azure. Обязательно скопируйте идентификатор приложения (клиента) и секрет клиента, используемые зарегистрированным приложением. Эта информация понадобится вам в следующем задании.

Для получения дополнительной информации о регистрации приложения и настройке разрешений см. [Регистрация приложения в Azure Active Directory](/dynamics365/business-central/dev-itpro/administration/register-app-azure#register-an-application-in-azure-active-directory) в справке для ИТ-специалистов и разработчиков.

> [!TIP]
> Если вы уже зарегистрировали приложение в рамках интеграции с другим продуктом Microsoft, например Power BI, вы можете повторно использовать эту регистрацию приложения. В этом случае вам просто нужно установить разрешения SharePoint.

### <a name="to-set-up-the-connection-in-prod_short-on-premises"></a>Чтобы установить соединение в локальной версии [!INCLUDE[prod_short](includes/prod_short.md)]

<!--
> [!NOTE]
> This requires the following types of authentication credentials:
>
> * Windows
> * NavUserPassword
> * Azure Active Directory
-->
1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") введите **Настройка подключения Microsoft SharePoint**, а затем выберите связанную ссылку.
2. В поле **Описание** введите описание для подключения, например **OneDrive**.
3. В поле **Папка** введите **Business Central**.
4. В поле **Расположение** введите URL-адрес вашего OneDrive.

    URL-адрес для OneDrive обычно имеет следующий формат: `https://<tenant name>-my.sharepoint.com`. Для получения дополнительной информации см. [URL-адреса OneDrive для пользователей в вашей организации](/onedrive/list-onedrive-urls) в документации OneDrive.
5. В поле **Идентификатор клиента** введите идентификатор клиента, указанный при регистрации вашего приложения.
6. В поле **Секрет клиента** введите секрет клиента, указанный при регистрации вашего приложения. 
   <!-- 
   For information about how to find the URLs, see the following:
   * [How to find your SharePoint server URL]
   * [How to find your OneDrive URL]-->

> [!IMPORTANT]
> Страница настройки подключения SharePoint используется для настройки нескольких устаревших функций. В разделе **Общее** настраивается подключение к OneDrive, а раздел **Общие документы** перенаправляет файлы в SharePoint вместо этого. Устаревшая функция SharePoint будет убрана в ближайшем будущем. Мы рекомендуем не настраивать раздел **Общие документы**.

## <a name="see-also"></a>См. также
[Интеграция Business Central и OneDrive для бизнеса](across-onedrive-overview.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)

