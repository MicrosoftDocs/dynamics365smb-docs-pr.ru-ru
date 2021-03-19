---
title: Устранение неполадок интеграции Microsoft Teams
description: Узнайте о том, что вы можете делать как администратор для управления интеграцией Microsoft Teams.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, troubleshooting, errors
ms.date: 01/20/2021
ms.author: jswymer
ms.openlocfilehash: 7a98b53a34ddf403cf6507da7740b97924d4c81c
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5385203"
---
# <a name="troubleshooting-microsoft-teams-integration-with-prod_short"></a>Устранение неполадок интеграции Microsoft Teams с [!INCLUDE [prod_short](includes/prod_short.md)]

[!INCLUDE [online_only](includes/online_only.md)]

В этой статье содержится информация о том, как определить и исправить проблемы, которые могут возникнуть при использовании Microsoft Teams с [!INCLUDE [prod_short](includes/prod_short.md)] в качестве обычного пользователя или администратора.

## <a name="none-of-my-links-expand-into-a-card"></a>Ни одна из моих ссылок не разворачивается в карточку 

Если вы столкнулись с этой проблемой, попробуйте следующее:

1. Сначала убедитесь, что приложение [!INCLUDE [prod_short](includes/prod_short.md)] для Teams установлено.

    Чтобы проверить, войдите в классическое приложение Teams или в Teams в браузере. Затем с левой стороны выберите **Приложения** и найдите **[!INCLUDE [prod_short](includes/prod_short.md)]**. Когда вы найдете приложение **[!INCLUDE [prod_short](includes/prod_short.md)]**, выберите его, чтобы открыть страницу сведений о приложении. Если отображается кнопка **Добавить для меня**, то приложение [!INCLUDE [prod_short](includes/prod_short.md)] не установлено. Для получения дополнительной информации о том, как установить приложение, см. раздел [Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md).

    > [!NOTE]
    > Гостевые пользователи не могут сразу устанавливать приложения. Дополнительные сведения о гостевых пользователях см. в разделе вопросов и ответов о сотрудничестве с гостями. 

2. Затем убедитесь, что вы вошли в систему под правильным идентификатором.

    В Teams перейдите в любой чат и под полем создания сообщения выберите значок [!INCLUDE [prod_short](includes/prod_short.md)]. Когда появится окно, проверьте, соответствует ли пользователь, который в нем указан как подключенный, тому пользователю, которого вы используете для подключения к [!INCLUDE [prod_short](includes/prod_short.md)].

3. Убедитесь, что codeunit 2718 **Поставщик сводки по страницам** публикуется как веб-сервис.

    Teams подключается к [!INCLUDE [prod_short](includes/prod_short.md)], используя конечную точку этого codeunit в службе [!INCLUDE [prod_short](includes/prod_short.md)]. Сведения о публикации веб-служб см. в разделе [Публикация веб-службы](across-how-publish-web-service.md).

4. Ваша организация может также запретить вам вставлять ссылки, которые расширяются в карточки. Свяжитесь со своим администратором, чтобы понять политики организации в Teams, которые могут применяться к вам.

## <a name="my-link-sometimes-doesnt-expand-into-a-card"></a>Моя ссылка иногда не расширяется в карточку 

Ссылка не превращается в карточку в следующих ситуациях:

- Ссылка нацелена на страницу, тип которой не представляет собой запись. Например, это может быть ссылка на ролевой центр [!INCLUDE [prod_short](includes/prod_short.md)]. Вы можете проверить тип страницы, используя панель проверки страницы в веб-клиенте в [!INCLUDE [prod_short](includes/prod_short.md)]. Дополнительные сведения о проверке страниц см. в разделе [Проверка страниц](across-inspect-page.md).
- Ссылка нацелена на страницу, которая (на техническом уровне) не связана с исходной таблицей в [!INCLUDE [prod_short](includes/prod_short.md)]. Вы можете проверить, содержит ли страница исходную таблицу, используя панель проверки страницы в веб-клиенте в [!INCLUDE [prod_short](includes/prod_short.md)]. Дополнительные сведения о проверке страниц см. в разделе [Проверка страниц](across-inspect-page.md). 
- Teams не поддерживает предварительный просмотр ссылок в некоторых функциях. Например, когда вы открываете окно чата, вы участвуете в собрании или являетесь гостем в другой организации.
- Teams молча отказывается от попытки отобразить карточку через 15 секунд, например, из-за проблем с сетью.
- Teams не может развернуть ссылку, если вы уже вставили ссылку в то же поле для создания сообщения и удалили карточку.

Ссылка также должна содержать всю необходимую информацию, чтобы найти запись и отобразить соответствующую карточку. Эта информация включает:

- Имя среды, путем включения его в URL-путь. Если вы не укажете имя среды, Teams предполагает, что вы пытаетесь достичь среды с именем "Производство".
- Название компании, используя параметр *company=*
- Идентификатор страницы, используя параметр *page=*
- Закладка для записи с помощью параметра *bookmark=*

Например:

`https://businesscentral.dynamics.com/?environmentname=Production&company=CRONUS%20USA%2C%20Inc.&page=21&dc=0&bookmark=21%3bEgAAAAJ7BTEAMAAwADAAMA%3d%3d`

Технические подробности об URL-адресах [!INCLUDE [prod_short](includes/prod_short.md)] см. в разделе [URL-адрес веб-клиента](/dynamics365/business-central/dev-itpro/developer/devenv-web-client-urls) в справке для разработчиков и ИТ-специалистов [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="the-card-is-displayed-in-the-message-compose-box-but-selecting-the-details-button-does-nothing"></a>Карточка отображается в поле для создания сообщения, но нажатие кнопки "Сведения" ничего не делает 

После того как ссылка будет преобразована в карточку в окне создания сообщения, вы должны отправить сообщение в чат, прежде чем сможете использовать кнопку **Сведения**.

## <a name="the-details-window-opens-but-shows-an-error-before-details-are-shown"></a>Окно сведений открывается, но перед отображением сведений отображается ошибка

Эта проблема может быть вызвана двумя причинами: отсутствие разрешений в [!INCLUDE [prod_short](includes/prod_short.md)] или настройки браузера (при использовании Teams в браузере).

1. Проверьте свои разрешения в [!INCLUDE [prod_short](includes/prod_short.md)].

    Чтобы просмотреть сведения для карточки, [!INCLUDE [prod_short](includes/prod_short.md)] проверяет вашу лицензию и разрешения на просмотр этой конкретной записи и страницы в конкретной компании и среде. Если у вас нет прав на какое-либо из этих действий, стандартные сообщения об ошибках [!INCLUDE [prod_short](includes/prod_short.md)] о разрешениях появляются в окне сведений. 

    Дополнительные сведения о разрешениях см. в разделе [Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)

2. Проверьте настройки своего браузера, если используете Teams в браузере.

    - Блокировщик всплывающих окон в вашем браузере должен быть отключен или настроен так, чтобы разрешать всплывающие окна из доменов *businesscentral.dynamics.com* или *bc.dynamics.com*. Для получения информации о разрешении всплывающих окон для [!INCLUDE [prod_short](includes/prod_short.md)] см. раздел [Настройка вашего браузера](across-browser-settings.md#popup).
    - Ваш браузер должен иметь доступ к локальному хранилищу файлов cookie и настроек во время вашей работы.
    - Избегайте использования просмотра в гостевом или частном режиме без необходимости, потому что они удаляют или блокируют определенный контент в некоторых браузерах.

    Дополнительные сведения о минимальных требованиях к браузеру см. в разделе [Минимальные требования для использования [!INCLUDE [prod_short](includes/prod_short.md)]](product-requirements.md#browsers) 

## <a name="im-having-problems-with-the-camera-or-location-in-teams"></a>У меня проблемы с камерой или местоположением в Teams 

Когда используются функции [!INCLUDE [prod_short](includes/prod_short.md)] в окне сведений, которым требуется доступ к вашему местоположению или камере устройства, вы должны сначала дать свое согласие на доступ Teams к этим возможностям устройства.  

- Для Teams в браузере убедитесь, что настройки вашего браузера разрешают доступ к камере и местоположению для https://teams.microsoft.com. 

- Для Teams для iOS или Android убедитесь, что настройки вашего устройства разрешают доступ к камере и местоположению для мобильного приложения Teams. 

Для получения справки об изменении этих настроек см. раздел [Моя камера не работает в Teams](https://support.microsoft.com/office/my-camera-isn-t-working-in-teams-9581983b-c6f9-40e3-b0d8-122857972ade?ns=msftteams&version=16&ui=en-us&rs=en-us&ad=us) в службе поддержки Microsoft.

Приложение [!INCLUDE [prod_short](includes/prod_short.md)] не поддерживает местоположение в классическом приложении Teams. Для получения дополнительной информации о местоположении см. раздел [Вопросы и ответы по Teams](teams-faq.md#location).

Некоторые браузеры, например новый Microsoft Edge, позволяют выбрать камеру устройства, которую следует использовать, если ваше устройство поддерживает несколько камер. 

## <a name="teams-displays-mixed-languages-for-my-cards-and-card-details"></a>В Teams отображаются разные языки для моих карточек и сведений карточек

Чтобы карточки и сведения карточек постоянно отображались на одном языке в Teams, язык вашего клиента Teams и язык, который вы используете в веб-клиенте [!INCLUDE [prod_short](includes/prod_short.md)], должны совпадать.

- Чтобы узнать об изменении языка в Teams, см. раздел [Изменение настройки в Teams](https://support.microsoft.com/en-us/office/change-settings-in-teams-b506e8f1-1a96-4cf1-8c6b-b6ed4f424bc7) в службе поддержки Microsoft. 

- Чтобы узнать об изменении языка в [!INCLUDE [prod_short](includes/prod_short.md)], см. раздел [Изменение основных настроек — язык](ui-change-basic-settings.md#language).

Для получения дополнительной информации о том, как языки работают между Teams и [!INCLUDE [prod_short](includes/prod_short.md)], см. раздел [Вопросы и ответы по Teams](teams-faq.md#language).

## <a name="i-edited-a-field-in-the-details-window-but-my-change-wasnt-saved"></a>Я отредактировал поле в окне сведений, но мои изменения не были сохранены

Изменения, которые вы вносите в поле в окнах сведений, автоматически сохраняются, когда вы покидаете поле. Прежде чем закрыть окно после изменения поля, обязательно нажмите клавишу TAB или щелкните/коснитесь за пределами поля.

## <a name="a-new-tile-appeared-in-the-app-launcher-how-do-i-remove-it"></a>На панели средства запуска приложений появилась новая плитка. Как ее удалить?

Когда вы просматриваете свои приложения на домашней странице Office 365 (https://home.office.com) или в средстве запуска приложений, появится новая плитка под названием «Соединитель службы интеграции Business Central Teams после установки приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Teams. Эта плитка сама по себе не представляет ценности и может быть безопасно скрыта.

Как администратор, у которого есть разрешения на администрирование Azure Active Directory, вы можете скрыть плитку, выполнив следующие действия:

1. Войдите в [центр администрирования Azure Active Directory](https://aad.portal.azure.com/).
2. Выберите **Корпоративные приложения**, затем выберите **Соединитель службы интеграции Business Central Teams**.
3. Выберите **Свойства**, затем установите **Отображается для пользователей** как **Нет**.
4. Нажмите **Сохранить**.

> [!NOTE]
> Пройдет некоторое время, прежде чем это изменение вступит в силу.


## <a name="see-also"></a>См. также

[Обзор интеграции [!INCLUDE [prod_short](includes/prod_short.md)] и Microsoft Teams](across-teams-overview.md)  
[Установка приложения [!INCLUDE [prod_short](includes/prod_short.md)] для Microsoft Teams](across-install-app-for-teams.md)  
[Вопросы и ответы по Teams](teams-faq.md)  
[Разработка для интеграции Teams](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]