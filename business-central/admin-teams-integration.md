---
title: Управление интеграцией Microsoft Teams с Business Central | Документация Майкрософт
description: Управление интеграцией Business Central с Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork
ms.date: 04/12/2021
ms.author: jswymer
ms.openlocfilehash: ecb3f88bf14c74f026f10fd49efe28f189036589
ms.sourcegitcommit: e13b80d4e5141f414109e660e0918eae561acb36
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "5882209"
---
# <a name="managing-microsoft-teams-integration-with-prod_short"></a>Управление интеграцией Microsoft Teams с [!INCLUDE [prod_short](includes/prod_short.md)]

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье представлен обзор того, что вы можете делать как администратор для управления интеграцией Microsoft Teams с [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="in-microsoft-teams"></a>В Microsoft Teams

### <a name="minimum-requirements"></a>Минимальные требования

В этом разделе описаны минимальные требования для работы функций приложения [!INCLUDE [prod_short](includes/prod_short.md)] в Teams.

- Необходимые лицензии

    В этой таблице представлен обзор лицензий, необходимых для работы функций приложения [!INCLUDE [prod_short](includes/prod_short.md)] в Teams.

    |Какая|Лицензия Teams|Лицензия [!INCLUDE [prod_short](includes/prod_short.md)]|
    |----|---|---|
    |Поиск контактов [!INCLUDE [prod_short](includes/prod_short.md)].|![флажок](media/check.png "галочка")|![флажок](media/check.png "галочка")|
    |Вставьте ссылку в запись [!INCLUDE [prod_short](includes/prod_short.md)] в беседу и отправьте как карточку.|![флажок](media/check.png "галочка")|![флажок](media/check.png "галочка")|
    |Посмотреть карточку записи [!INCLUDE [prod_short](includes/prod_short.md)] в разговоре.|![флажок](media/check.png "галочка")||
    |Посмотреть подробности карточки записи [!INCLUDE [prod_short](includes/prod_short.md)] в разговоре.|![флажок](media/check.png "галочка")|![флажок](media/check.png "галочка")|

- Разрешить предварительный просмотр URL-адресов

    Параметр политики **Разрешить предварительный просмотр URL-адресов** должен быть включен. В противном случае невозможно создать карточку для ссылок [!INCLUDE [prod_short](includes/prod_short.md)], вставленных в беседу Teams. Для получения дополнительной информации об этом параметре см. [Управляйте политиками обмена сообщениями в Teams](/microsoftteams/messaging-policies-in-teams).

### <a name="managing-the-prod_short-app-optional"></a>Управление приложением [!INCLUDE [prod_short](includes/prod_short.md)] (необязательно)

Как администратор Teams вы можете управлять всеми приложениями для своей организации, включая приложение [!INCLUDE [prod_short](includes/prod_short.md)]. Вы можете утвердить или установить приложение [!INCLUDE [prod_short](includes/prod_short.md)] для вашей организации, запретить пользователю устанавливать приложение и т. д.

Для получения дополнительной информации см. следующие статьи в документации Microsoft Teams:

- [Управляйте своими приложениями в центре администрирования Microsoft Teams](/MicrosoftTeams/manage-apps)
- [Управляйте политиками настройки приложений в Microsoft Teams](/microsoftteams/teams-app-setup-policies)

## <a name="in-prod_short"></a>В [!INCLUDE [prod_short](includes/prod_short.md)]

### <a name="minimum-requirements"></a>Минимальные требования

- Версия [!INCLUDE [prod_short](includes/prod_short.md)]:

    [!INCLUDE [prod_short](includes/prod_short.md)] выпуск 2021, волна 1, или новее. Интеграция Teams поддерживается только для [!INCLUDE [prod_short](includes/prod_short.md)] (онлайн); не локально.

- Codeunit **2718, поставщик сводки по страницам** публикуется как веб-сервис:

    Этот codeunit публикуется как веб-служба по умолчанию. codeunit является частью системного приложения [!INCLUDE [prod_short](includes/prod_short.md)]. Он используется для получения данных поля для страницы [!INCLUDE [prod_short](includes/prod_short.md)], добавленной в беседу Teams. Сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

- <a name="permissions"></a>Разрешения пользователя:

    Как правило, поиск контактов, страницы и данные, которые пользователи могут просматривать и редактировать в беседе Teams, контролируются их разрешениями в [!INCLUDE [prod_short](includes/prod_short.md)].
    
    - Для поиска контактов пользователи должны иметь как минимум разрешение на чтение для таблицы **Контакты**. 
    - Чтобы вставить ссылку [!INCLUDE [prod_short](includes/prod_short.md)] в беседу Teams и развернуть ее в карточку, пользователи должны иметь как минимум разрешение на чтение страницы и ее данных.
    - После того, как карточка отправлена в беседу, любой пользователь в этой беседе может просматривать эту карточку без разрешения [!INCLUDE [prod_short](includes/prod_short.md)].
    - Чтобы просмотреть подробную информацию о карте или открыть запись в [!INCLUDE [prod_short](includes/prod_short.md)], пользователи должны иметь разрешение на чтение страницы и ее данных.
    - Чтобы изменить данные, пользователю необходимо изменить разрешения.
    
    Сведения о разрешениях см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).

## <a name="managing-privacy-and-compliance"></a>Управление конфиденциальностью и соблюдением требований 

Microsoft Teams обеспечивает обширный контроль за соблюдением и управлением конфиденциальными или личными данными &mdash; включая данные, добавленные в чаты и каналы приложением [!INCLUDE [prod_short](includes/prod_short.md)].

### <a name="understanding-where-prod_short-cards-are-stored"></a>Сведения о том, где хранятся карточки [!INCLUDE [prod_short](includes/prod_short.md)] 

После отправки карточки в чат она и поля, отображаемые на карточке, копируются в Teams. Эта информация регулируется политиками Teams для вашей организации, такими как политики хранения данных. При отображении сведений карточки никакие данные в окне сведений не хранятся в Teams. Данные остаются в [!INCLUDE [prod_short](includes/prod_short.md)] и будут извлечены Teams только тогда, когда пользователь решит просмотреть сведения. 

- Чтобы узнать больше о том, где Teams хранит эти данные, см. раздел [Расположение данных в Microsoft Teams](/microsoftteams/location-of-data-in-teams).
- Чтобы узнать больше о политиках хранения в Teams, см. раздел [Политики хранения в Microsoft Teams](/microsoftteams/retention-policies).

### <a name="restricting-sharing-of-cards"></a>Ограничение доступа к карточкам 

Вы запрещаете отдельным пользователям или группам отправлять карточки в чаты или каналы, настраивая политики обмена сообщениями, которые отключают настройку **Предварительный просмотр URL-адресов**. Для получения дополнительной информации об этом параметре см. [Управление политиками обмена сообщениями в Teams](/microsoftteams/messaging-policies-in-teams). 

Вы также можете использовать информационные барьеры, чтобы люди или группы не могли общаться друг с другом. Дополнительные сведения см. в разделе [Информационные барьеры в Microsoft Teams](/microsoftteams/information-barriers-in-teams).

Функции предотвращения потери данных в Центре безопасности и соответствия требованиям Microsoft 365 нельзя применять специально к карточкам. Но их можно применить к сообщениям чата, содержащим карточки. <!-- To track upcoming advanced features that include enabling DLP for cards, see [https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093](https://www.microsoft.com/en-us/microsoft-365/roadmap?featureid=67093).-->

### <a name="responding-to-data-requests"></a>Ответы на запросы данных

Вы разрешаете членам групп и владельцам групп удалять сообщения, содержащие конфиденциальные карточки, путем настройки политик обмена сообщениями, например: **Владельцы могут удалять отправленные сообщения** и **Пользователи могут удалять отправленные сообщения**. Дополнительные сведения см. в разделе [Управление политиками обмена сообщениями в Teams](/microsoftteams/messaging-policies-in-teams).

Функции поиска содержимого и соответствия eDiscovery в Центре безопасности и соответствия требованиям Microsoft 365 можно также применять к карточкам.

Поскольку данные карточек в Teams являются копией данных в [!INCLUDE [prod_short](includes/prod_short.md)], вы также можете использовать функции [!INCLUDE [prod_short](includes/prod_short.md)] для экспорта данных клиента по запросу. Дополнительные сведения о конфиденциальности в [!INCLUDE [prod_short](includes/prod_short.md)] см. в разделе [Вопросы и ответы о конфиденциальности для клиентов Business Central](/dynamics365/business-central/dev-itpro/security/privacyfaq).

## <a name="see-also"></a>См. также
[Обзор интеграции [!INCLUDE [prod_short](includes/prod_short.md)] и Microsoft Teams](across-teams-overview.md)  
[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Вопросы и ответы по Teams](teams-faq.md)  
[Устранение неполадок Teams](admin-teams-troubleshooting.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]