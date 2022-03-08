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
ms.date: 10/08/2020
ms.author: jswymer
ms.openlocfilehash: 3c04dfb2f77eba906b2567ca9438849e1cc20861
ms.sourcegitcommit: 4bca699d2a5ce182eb5572d72fac4fb478c4f293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2020
ms.locfileid: "3989362"
---
# <a name="managing-microsoft-teams-integration-with-business-central"></a>Управление интеграцией Microsoft Teams с Business Central

[!INCLUDE [teams_preview.md](includes/teams_preview.md)]

В этой статье представлен обзор того, что вы можете делать как администратор для управления интеграцией Microsoft Teams с [!INCLUDE [prodshort](includes/prodshort.md)].

## <a name="in-microsoft-teams"></a>В Microsoft Teams

### <a name="minimum-requirements"></a>Минимальные требования

В этом разделе описаны минимальные требования для работы функций приложения [!INCLUDE [prodshort](includes/prodshort.md)] в Teams.

- Необходимые лицензии

    В этой таблице представлен обзор лицензий, необходимых для работы функций приложения [!INCLUDE [prodshort](includes/prodshort.md)] в Teams.

    |Какая|Лицензия Teams|Лицензия Business Central|
    |----|---|---|
    |Вставьте ссылку в запись [!INCLUDE [prodshort](includes/prodshort.md)] в беседу и отправьте как карточку.|![флажок](media/check.png "галочка")|![флажок](media/check.png "галочка")|
    |Посмотреть карточку записи [!INCLUDE [prodshort](includes/prodshort.md)] в разговоре.|![флажок](media/check.png "галочка")||
    |Посмотреть подробности карточки записи [!INCLUDE [prodshort](includes/prodshort.md)] в разговоре.|![флажок](media/check.png "галочка")|![флажок](media/check.png "галочка")|

- Разрешить предварительный просмотр URL-адресов

    Параметр политики **Разрешить предварительный просмотр URL-адресов** должен быть включен. В противном случае невозможно создать карточку для ссылок Business Central, вставленных в беседу Teams. Для получения дополнительной информации об этом параметре см. [Управляйте политиками обмена сообщениями в Teams](/microsoftteams/messaging-policies-in-teams).

### <a name="managing-the-business-central-app-optional"></a>Управление приложением Business Central (необязательно)

Как администратор Teams вы можете управлять всеми приложениями для своей организации, включая приложение [!INCLUDE [prodshort](includes/prodshort.md)]. Вы можете утвердить или установить приложение [!INCLUDE [prodshort](includes/prodshort.md)] для вашей организации, запретить пользователю устанавливать приложение и т. д.

Для получения дополнительной информации см. следующие статьи в документации Microsoft Teams:

- [Управляйте своими приложениями в центре администрирования Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/manage-apps)
- [Управляйте политиками настройки приложений в Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-app-setup-policies)

## <a name="in-prodshort"></a>В [!INCLUDE [prodshort](includes/prodshort.md)]

### <a name="minimum-requirements"></a>Минимальные требования

- Версия [!INCLUDE [prodshort](includes/prodshort.md)]:

    [!INCLUDE [prodshort](includes/prodshort.md)] выпуск 2020, волна 2 (версия 17) или новее. Интеграция Teams поддерживается только для [!INCLUDE [prodshort](includes/prodshort.md)] (онлайн); не локально.

- Codeunit **2718, поставщик сводки по страницам** публикуется как веб-сервис:

    Этот codeunit публикуется как веб-служба по умолчанию. codeunit является частью системного приложения [!INCLUDE [prodshort](includes/prodshort.md)]. Он используется для получения данных поля для страницы [!INCLUDE [prodshort](includes/prodshort.md)], добавленной в беседу Teams. 

- Разрешения пользователя:

    Как правило, страницы и данные, которые пользователи могут просматривать и редактировать в беседе Teams, контролируются их разрешениями в [!INCLUDE [prodshort](includes/prodshort.md)].
    
    - Чтобы вставить ссылку [!INCLUDE [prodshort](includes/prodshort.md)] в беседу Teams и развернуть ее в карточку, пользователи должны иметь как минимум разрешение на чтение страницы и ее данных.
    - После того, как карточка отправлена в беседу, любой пользователь в этой беседе может просматривать эту карточку без разрешения Business Central.
    - Чтобы просмотреть подробную информацию о карте или открыть запись в [!INCLUDE [prodshort](includes/prodshort.md)], пользователи должны иметь разрешение на чтение страницы и ее данных.
    - Чтобы изменить данные, пользователю необходимо изменить разрешения.
    
    Сведения о разрешениях см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md).

## <a name="see-also"></a>См. также
[Обзор интеграции Business Central и Microsoft Teams](across-teams-overview.md)  
[Установите приложение [!INCLUDE [prodshort](includes/prodshort.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  
[Приступая к работе](product-get-started.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
